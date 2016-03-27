# osx-dev-environment

## Setting up an ansible script for my development environment

After a clean install of OSX El Capitan:

- Install Homebrew
  - Open Terminal and paste: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
- Install Ansible
  - Open Terminal and paste: `brew install ansible`
- Clone repo
  - Open Terminal and paste: `git clone https://github.com/lechegaray/osx-dev-environment.git`
  - Move into the cloned directory: `cd osx-dev-environment`
  - Run ansible command: `ansible-playbook osx-dev-environment.yml -i hosts`
    - You may need to insert your administrator password at some point.  This is a one time deal.
    - Microsoft Office has a bad habit for failing randomly, rerun the script and it should work.
    - Remember that Ansible is idempotent, it will not redownload or reinstall anything if it is present.
