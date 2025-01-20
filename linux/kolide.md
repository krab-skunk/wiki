```bash
apt-get install -y dkms libelf-dev linux-headers-$(uname -r) build-essential

cp -R /media/cdrom0 /tmp
Cd /tmp/cdrom0
chmod +x install
./install

——

Configured SSH

Apt install vim
apt remove libreoffice-*
apt autoremove
apt autoclean


—
dpkg --add-architecture amd64
Apt-get update
apt install chromium
apt install python3-virtualenv
apt install snapd
snap install aws-cli --classic

curl -sSO https://downloads.1password.com/linux/tar/stable/aarch64/1password-latest.tar.gz
sudo tar -xf 1password-latest.tar.gz
sudo mkdir -p /opt/1Password
sudo mv 1password-*/* /opt/1Password

sudo /opt/1Password/after-install.sh

——
apt-get install clamav clamav-daemon
——
apt-get install binutils:amd64
Downloaded kolide via Okta 
dpkg -i /home/steve-heslouin/Downloads/kolide-launcher.deb
-—
Apt install kubectx 
apt-get install -y apt-transport-https ca-certificates curl gnupg

curl -fsSL https://pkgs.k8s.io/core:/stable:/v1.32/deb/Release.key | gpg --dearmor -o /etc/apt/keyrings/kubernetes-apt-keyring.gpg
chmod 644 /etc/apt/keyrings/kubernetes-apt-keyring.gpg 
echo 'deb [signed-by=/etc/apt/keyrings/kubernetes-apt-keyring.gpg] https://pkgs.k8s.io/core:/stable:/v1.32/deb/ /' | tee /etc/apt/sources.list.d/kubernetes.list
chmod 644 /etc/apt/sources.list.d/kubernetes.list
Apt update
Apt install kubectl
—
Install omzsh
apt install zsh git curl 
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"	
—

apt install network-manager-openvpn
apt-get install network-manager-openvpn-gnome

Open nm-connection-editor (GUI)
And to have splitting, make sure you add for ex 10.100.0.0 / 255.255.0.0 without 3rd arg 
Or edit the oven file to remove the 3rd arg (vpn_gateway)

—

 wget https://storage.googleapis.com/chrome-for-testing-public/131.0.6778.139/linux64/chromedriver-linux64.zip
Unzip chromedriver-linux64.zip
apt install libglib2.0-dev:amd64 libnss3:amd64 libxcb1:amd64
./chromedriver 
```

——
## If rosetta stop working (that switch from using rosetta to using qemu)
```bash
sudo apt update
sudo apt install binfmt-support qemu-user-static
```

