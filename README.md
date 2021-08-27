# local-dev-playbook

Ansible playbook for installing local development tools

## Install Homebrew

`https://brew.sh/`

### Install Ansible

`brew install ansible`

## Run

Install all tools

`ansible-playbook -K -i inventory playbook.yml`

Install kubernetes tools only

`ansible-playbook -K -i inventory playbook.yml --tags kubernetes`

Create aliases only

`ansible-playbook -K -i inventory playbook.yml --tags aliases`
