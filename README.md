# ansible-course
    - Installation - ( Nginx)
### ANSIBLE COMMANDS

RUN: `ansible-playbook -i <your inventory file or location> < your playbook > -u < user > --private-key < private key name/location > -vv`

` -vvv `Causes Ansible to print more debug messages.Adding multiple -v will increase the verbosity, the builtin plugins currently evaluate up to -`vvvvvv`. A reasonable level to start is `-vvv`,
connection debugging might require `-vvvv`.


### ANSIBLE VAULT

RUN: `ansible-vault < encrypt/decrypt > < file name >` to encrypt or decrypt a sesnstive data playbook
RUN: `ansible-vault < encrypt/decrypt > --vault-id dev@prompt < file name >` to encrypt or decrypt a sesnstive data playbook to a speciic environment eg. `dev`
RUN: `ansible-playbook < playbook >  --vault-password-file < password file >` this alows you to pass a password from a file.
