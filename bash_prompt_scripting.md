use su to get to root.  then install fortune and cowsay
```
su 
apt-get install cowsay <-(you will get errors, that is okay, it will still install)
apt-get install fortune
/usr/games/fortune | /usr/games/cowsay
```
get out of root by typing 'exit' then cd to your home dir using '~' and open your .bashrc using nano

```
exit
cd ~
nano .bashrc
```
At the bottom of your bash.rc paste one of the promts from your terminal.  For example:

```
#to create colored cow prompt, insert this line at the end of your .bashrc
PS1="(\$( /usr/games/fortune | /usr/games/cowsay -n)\[\e[1;36m\]\d \[\e[1;32m\]\t \[\e[1;33m\]\u@\[\e[1;35m\]\h:\w\$\[\e[0;31m\] "
```
Save using F2 and then open a new terminal to see if your changes persisted.
Upload your .bashrc to github
