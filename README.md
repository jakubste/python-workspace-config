GIT
===

    sudo apt-get install git

    git config --global user.name "Jakub Stępak"
    git config --global user.email jakub.ste@gmail.com
    git config --global push.default matching

    cat ~/.ssh/id_rsa.pub

jeśli jest puste (nie istnieje): `ssh-keygen`

zawartość `id_rsa.pub` skopiuj i wklej do: `https://bitbucket.org/account/user/TWÓJLOGIN/ssh-keys/` i `https://github.com/settings/ssh`


Python:
======

Instalacja pythona, pipa i virtualenva:

    sudo apt-get install python python-dev python-pip
    
    pip completion --bash >> ~/.bashrc
    source ~/.bashrc
    
    sudo pip install virtualenv
    sudo pip install virtualenvwrapper
    
    export WORKON_HOME=~/.virtualenvs
    mkdir $WORKON_HOME
    echo "export WORKON_HOME=$WORKON_HOME" >> ~/.bashrc
    
    echo "source $HOME/.local/bin/virtualenvwrapper.sh" >> ~/.bashrc
    echo "export PIP_VIRTUALENV_BASE=$WORKON_HOME" >> ~/.bashrc
    source ~/.bashrc

Użycie virtualenva:

    mkvirtualenv test
    deactivate
    workon test
    rmvirtualenv test

PyCharm:
========

Potrzebna będzie java:

    sudo apt-get install default-jdk

Pobierz paczkę ze strony https://www.jetbrains.com/pycharm/download/

Rozpakuj (ja lubię do katalogu bin w katalogu domowym). Potem:

    cd ~/bin/pycharm[tab]/bin/
    ./pycharm.sh

Pycharm spyta się o zrobienie ikonki - zrób sobie. Jak Cię nie zapytał, to masz problem i pogooglaj ;)
Potem go zamknij, żeby zwolnił się terminal - możesz teraz odpalać pycharma jak zwykły program