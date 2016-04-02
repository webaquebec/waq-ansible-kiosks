# WAQ Ansible Kiosks 

> Setup the cluster of raspberry pi for displays at Web à Québec with Ansible

## Setup

Setup your hosts address in `hosts` with the URL to display as `kiosk_url` and optionally `rotate` the screen.

Rotate options (http://elinux.org/RPiconfig) È

```
display_rotate=0        Normal
display_rotate=1         90 degrees
display_rotate=2        180 degrees
display_rotate=3        270 degrees
display_rotate=0x10000  horizontal flip
display_rotate=0x20000  vertical flip
```

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
