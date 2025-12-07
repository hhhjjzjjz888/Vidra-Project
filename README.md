sudo apt update
sudo apt upgrade -y
pkg install tsu -y

# Install Boxvidra Emulator (package)
sudo apt install Boxvidra -y

sudo boxvidra
bash boxvidra.sh
sudo apt update
sudo apt install docker -y
sudo apt install docker-compose -y
mkdir dockercomp
cd dockercomp
wget -O windows10.yml https://example.com/windows10.yml
sudo docker-compose -f windows10.yml up
BOXVIDRA-PROJECT/
 ├── boxvidra.sh             # Emulator launcher script
 ├── install.sh              # Termux auto-installer
 ├── windows10.yml           # Windows 10 Docker YAML
 ├── dockercomp/             # Docker workspace
 ├── README.md               # Documentation
 └── assets/                 # Emulator support files
