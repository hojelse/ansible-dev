# Ansible dev config
Ansible config for personal development desktop

- Get noreply email https://github.com/settings/emails
- Generate key `ssh-keygen -t rsa -C "account@mydomain.com"`
- Add `cat ~/.ssh/id_rsa.pub` to https://github.com/settings/keys

```
sudo apt update
sudo apt install git
mkdir repo
cd repo
git clone git@github.com:hojelse/dotfiles
git clone git@github.com:hojelse/ansible-dev
cd ~
ln -s ~/repo/dotfiles/.gitconfig ~/.gitconfig
```

```
sudo apt install ansible
sudo ansible-pull -U https://github.com/hojelse/ansible-dev.git
```

## TODO
- gnome scroll direction natural
- before installing dotnet:
```
wget https://packages.microsoft.com/config/ubuntu/22.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
rm packages-microsoft-prod.deb
```
- `sudo apt remove ibus` to fix ctrl+. in vscode
- install docker
