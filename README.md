# hypermodern-python-iitt

Create /etc/wsl.conf as explained before with that :

[network]
generateResolvConf = **false**
1 . Rename link /etc/resolv.conf :
> sudo mv /etc/resolv.conf /etc/resolv.conf.old

2 . Create and edit new resolv.conf file (not a link) :
> sudo vi /etc/resolv.conf

and just add this line (indicate your livebox gateway address / (orange for me)) :

nameserver 192.168.1.1

3 . Don't forget to change authorization :

> sudo chmod 777 /etc/resolv.conf

You should see that :
image
image

4 . close console and reopen it. just type :
exit

5 . Try to update linux (sudo apt update) to check network connection and .... it works well (not before procedure).


pyenv install 3.10.7 
pyenv install 3.9.14 
pyenv install 3.8.14
pyenv local 3.10.7 3.9.14 3.8.14



python3 -m pip install --user pipx
python3 -m pipx ensurepath


Installing collected packages: pyparsing, click, argcomplete, userpath, packaging, pipx
  WARNING: The script userpath is installed in '/home/chris/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
  WARNING: The script pipx is installed in '/home/chris/.local/bin' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-locati

  vi $HOME/.bashrc
  export PATH=/home/chris/.local/bin:$PATH
source $HOME/.bashrc

pipx install poetry
