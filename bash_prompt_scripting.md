su 
apt-get install cowsay <-(you will get errors, that is okay, it will still install)
apt-get install fortune
/usr/games/fortune | /usr/games/cowsay
cd ~
nano .bashrc

to create colored cow prompt, insert this line at the end of your .bashrc
PS1="(\$( /usr/games/fortune | /usr/games/cowsay -n)\[\e[1;36m\]\d \[\e[1;32m\]\t \[\e[1;33m\]\u@\[\e[1;35m\]\h:\w\$\[\e[0;31m\] "
