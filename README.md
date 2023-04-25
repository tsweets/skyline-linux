# skyline-linux

When running locally try

ansible-playbook skyline-linux.yml -i hosts -c local

ansible-playbook skyline-linux.yml -i hosts -c local  --extra-vars "PASSWORD"



# TODO:
- [ ] Docker Molecule Image for Fedora
- [x] Package/Install Nord Theme
- [X] Install Zafiro Icons
- [X] tony roll with avatar
- [X] Java role
- [ ] DevOps role
    - [X] Ansible
    - [X] Molecule
    - [ ] Terraform
    - [ ] Packer
- [ ] Intellij Ulitmate based off of Community Spec
- [ ] Python role
- [X] Docker Roll
- [ ] k3s role
- [ ] zeal docs
- [ ] spotify
- [ ] steam
- [ ] skype (is there a zoom?)
- [ ] uberwriter (md editor)
- [ ] inkscape
- [ ] atom editor
- [ ] filezilla
- [ ] lollypop
- [ ] authenticator
- [ ] DB Dev
    - [ ] MySQL
    - [ ] Sqqueler
    - [ ] MySQL Workbench
    - [ ] Postgres
- [ ] GitG
- [ ] Meld (Diff Tool)
- [ ] Bitwarden/enpass
- [ ] LSD (LS Delux)
- [ ] httpie
- [ ] jq
- [ ] Gnmoe Sushi (Preview for Nautlius)
- [ ] Timeshift
- [X] Chrome
- [ ] Alacritty
- [ ] Tilix
- [ ] Geary

##### Collections & Roles Installed
ansible-galaxy collection install ansible.posix
ansible-galaxy install gantsign.visual-studio-code

### Manual Installs
1. Oh My zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

2. Krew (kubectl plugin manager)
https://krew.sigs.k8s.io/docs/user-guide/quickstart/
then: 
kubectl krew install ctx
kubectl krew install ns

3. k3d
wget -q -O - https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash
then:
k3d cluster create mycluster

4. Nord Gnome Terminal Profile
https://github.com/nordtheme/gnome-terminal

5. Synology Drive Client
https://copr.fedorainfracloud.org/coprs/emixampp/synology-drive/

6. Bitwarden (Flathub)

## Running Ansible without typing in the vault password all the damn time
1. Create a file ~/.ansible/ansible-pass (Shuld be just a one liner with the password)
2. export ANSIBLE_VAULT_PASSWORD_FILE=~/.ansible/ansible-pass pointing to this file   ANSIBLE_VAULT_PASSWORD_FILE=~/.ansible/ansible-pass

