# WAQ Ansible Kiosks 

> Setup the cluster of raspberry pi for displays at Web à Québec with Ansible

## Quick start

Setup your hosts address in `hosts`.

Run ansible with ask for password first time :

    ansible-playbook playbook.yml -i hosts --ask-pass

Then you can skip pass since authorized keys are setup :

    ansible-playbook playbook.yml -i hosts

# Credits

Thanks to the authors of the following articles :

https://www.danpurdy.co.uk/web-development/raspberry-pi-kiosk-screen-tutorial/
http://www.stinebaugh.info/ansible-playbook-to-create-a-minimal-headless-raspberry-pi/
https://sendgrid.com/blog/complete-guide-set-raspberry-pi-without-keyboard-mouse/