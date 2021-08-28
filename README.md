# local-dev-playbook

Ansible playbook for installing local development tools

## Install Homebrew

`https://brew.sh/`

### Install Ansible

`brew install ansible`

## Run

For dry run suffix any of the following with `--check`

### Install all

`ansible-playbook -K -i inventory playbook.yml`

### Install aliases only

`ansible-playbook -K -i inventory playbook.yml --tags aliases`

### Install all kubernetes tools

`ansible-playbook -K -i inventory playbook.yml --tags kubernetes`

### Install helm only

`ansible-playbook -K -i inventory playbook.yml --tags helm`
