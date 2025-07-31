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
sudo apt install ufw -y
sudo ufw allow 22
sudo ufw allow 3000/tcp
sudo ufw enable
```
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
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash - && sudo apt update && sudo apt install -y nodejs
screen -S gensyn
```
```
git clone https://github.com/gensyn-ai/rl-swarm.git
cd rl-swarm
```
```
python3 -m venv .venv
source .venv/bin/activate
sed -i 's/rewards = torch.tensor(rewards)/rewards = torch.tensor([[r, 0.0] if isinstance(r, (int, float)) else r for r in rewards])/g' .venv/lib/python3.12/site-packages/genrl/trainer/grpo_trainer.py
pip install --force-reinstall transformers==4.51.3 trl==0.19.1
./run_rl_swarm.sh
``````

LOGIN WITH EMAIL
```
wget -q https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-linux-amd64.deb
sudo dpkg -i cloudflared-linux-amd64.deb
cloudflared tunnel --url http://localhost:3000
```

```
Gensyn/Qwen2.5-0.5B-Instruct
```

ERROR WANDB:
``````
deactivate 
rm -rf .venv
``````
``````
python3 -m venv .venv
source .venv/bin/activate
``````
``````
./run_rl_swarm.sh
``````
UPDATE:
``````
git stash
git pull
bash run_rl_swarm.sh
``````
VERSION CHECK:
``````
git describe --tags
``````
BACKUP:
``````
[ -f backup.sh ] && rm backup.sh; curl -sSL -O https://raw.githubusercontent.com/AbhiEBA/gensyn1/main/backup.sh && chmod +x backup.sh && ./backup.sh
``````
ROLEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEEE:
``````
cd ~
wget https://go.dev/dl/go1.24.0.linux-amd64.tar.gz
sudo rm -rf /usr/local/go
sudo tar -C /usr/local -xzf go1.24.0.linux-amd64.tar.gz
 
# Set environment variables
echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc
echo 'export GOPATH=$HOME/go' >> ~/.bashrc
echo 'export PATH=$PATH:$GOPATH/bin' >> ~/.bashrc
source ~/.bashrc
 
# Verify Go installation
go version
``````
``````
go install github.com/Deep-Commit/gswarm/cmd/gswarm@latest
gswarm
``````
