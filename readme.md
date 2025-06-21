GITBASH
```
ssh-keygen -t rsa -f ~/.ssh/F -C "F"
```
```
cd /c/Users/akhil66222/.ssh/

```
```
cat F.pub
```
```
ssh -i F F@IP
```

STARTING THE GENSYN NODE
```
sudo swapoff -a
sudo rm -f /swapfile

sudo fallocate -l 8G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile

swapon --show
free -h

echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab
```
```
sudo rm /var/lib/dpkg/lock-frontend
sudo rm /var/cache/apt/archives/lock
```
```
sudo apt update && sudo apt install -y
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && sudo apt update && sudo apt install -y yarn
```
```
curl -sSL https://raw.githubusercontent.com/ABHIEBA/Gensyn/main/node.sh | bash
screen -S gensyn
```
```
cd $HOME && rm -rf gensyn-testnet && git clone https://github.com/zunxbt/gensyn-testnet.git && chmod +x gensyn-testnet/gensyn.sh && ./gensyn-testnet/gensyn.sh
``````
LOGIN WITH EMAIL AND CLOSE THE NEW TERMINAL......GO BACK TO OLD TERMINAL....FAST COPY ORG ID 

COPY 3 WORD NAME AND PEER ID FROM SAME LINE COMMAND .... SAVE BOTH IN TXT

COMMAND WILL RUN 

PRESS CTRL+A+D
``````
[ -f backup.sh ] && rm backup.sh; curl -sSL -O https://raw.githubusercontent.com/AbhiEBA/gensyn1/main/backup.sh && chmod +x backup.sh && ./backup.sh
``````
BACKUP ALL THREE

PRESS CTRL+C TO CLOSE
``````
screen -ls
``````
``````
screen -r CODE
``````
CHECK ON  GENSYN TG BOT GIVING YOUR NODE ID, IF THE WALLET IS NOT SHOWING 0000 IF ITS SHOWING, REDO NODE PROCESS FROM START
