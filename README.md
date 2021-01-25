# UBUNTU HACKS

## Change user
``sudo chown user directory/file``

## Install MongoDB Compass
``sudo dpkg -i EnterfileName.deb``

## Install DBeaver

``wget -O - https://dbeaver.io/debs/dbeaver.gpg.key | sudo apt-key add``

``echo "deb https://dbeaver.io/debs/dbeaver-ce /" \ | sudo tee /etc/apt/sources.list.d/dbeaver.list``

``sudo apt update``

``sudo apt install dbeaver-ce``

## Create new file

``touch newfile.txt``

## Install .deb

``sudo dpkg -i package_file.deb``

## Install pip for Python 3

``sudo apt update``

``sudo apt install python3-pip``

``pip3 --version``
