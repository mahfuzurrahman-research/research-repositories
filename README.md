cd ~/Documents

if [ ! -d "research-repositories/.git" ]; then
  git clone https://github.com/mahfuzurrahman-research/research-repositories.git
fi

cd research-repositories

git pull origin main

pbpaste > README.md

git add README.md

git commit -m "Update research repositories portfolio README"

git push origin main