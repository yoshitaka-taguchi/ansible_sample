useradd ansible

passwd ansible

visudo
%wheel        ALL=(ALL)       NOPASSWD: ALL

usermod -aG wheel ansible

ssh-copy-id ansible@xxxxx

ansible-playbook -i inventory/develop/hosts test.yml
