# WAQ Ansible Kiosks 

> Setup the cluster of raspberry pi for displays at Web à Québec with Ansible

## Setup

Setup your hosts address in `hosts`.

You can set the kiosks URL to display as `kiosk_url` in `playbook.yml`.

Each host will open the URL with a query string with the hostname ex: 

    http://google.com/?kiosk=qcumpi-4

## Quick start

Run ansible with ask for password first time :

    ansible-playbook playbook.yml -i hosts --ask-pass

Then you can skip pass since authorized keys are setup :

    ansible-playbook playbook.yml -i hosts

# Credits

Jean-Philippe Doyle & Web à Québec.

Thanks to the authors of the following articles for the basis of my setup :

- https://www.danpurdy.co.uk/web-development/raspberry-pi-kiosk-screen-tutorial/
- http://www.stinebaugh.info/ansible-playbook-to-create-a-minimal-headless-raspberry-pi/
- https://sendgrid.com/blog/complete-guide-set-raspberry-pi-without-keyboard-mouse/
