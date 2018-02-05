# workstation_build
## General Notes
### pip conf
 * linux locatoin $HOME/.conf/pip/pip.conf
 * mac os location $HOME/Library/Application Support/pip/pip.conf

## Mac Specific Notes
 - xcode has to be installed first (xcode-select --install)
 - install brew version of python 2 and 3
 - install ansible
 - run playbook
### Mac Playbook Thoughts
 - Install Homebrew
   - This should be handled by geerlingguy's homebrew role
 - use brew to install
   - git
   - vim
   - macvim (replace built-in vim)
   - spotify
### Steps
1. Install xcode
`xcode-select --install`
2. Install pip
`sudo easy_install pip`
3. Install ansible
`sudo pip install ansible`
4. Clone repo locally
`git clone https://github.com/kas21/workstation_build.git ~/Projects/workstation_build`
5. Run ansible galaxy
`ansible-galaxy install -r requirements.yml`
6. Run ansible playbook
`ansible-playbook main.yml`

