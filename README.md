This repository contains Ansible playbooks for routine tasks which I typically carry out on a fresh VM to make working on it more convenient.

To run the provisioning playbook:

- Set the environment variables `HOST` and `SSH_USER` to the host and username
  of the machine to be provisioned.

- Run the following commands (make sure you don't forget the comma after `${HOST}` if you type it manually):
  ```
  pipenv install
  pipenv run ansible-playbook -i ${HOST}, --user=${SSH_USER} provision.yml
  ```
