## Install Dependencies

Install the curl and other required packages for Ruby on Rails installation.

``sudo apt update``

``sudo apt install -y curl gnupg2 dirmngr git-core zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev software-properties-common libffi-dev``

## Install Node.js

Rails need a Javascript runtime for application development in Linux. So, for that, we will install the LTS version of Node.js (v12.x).

``curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -``

``sudo apt install -y nodejs``

Install Yarn

Add the Yarn repository in case if you want to install the Yarn package manager to manage packages.

``curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -``

``echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list``

Install Yarn with the below command.

``sudo apt update && sudo apt install -y  yarn``

Install Ruby
Using rbenv (Recommended)

```cd
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL```

``rbenv install 2.7.1``

``rbenv global 2.7.1``

``ruby -v``
