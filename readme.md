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
python3 -m venv .venv
source .venv/bin/activate
git switch main
git reset --hard
git clean -fd
git pull origin main
./run_rl_swarm.sh
``````


