# WAQ Kiosks setup with Ansible 

> Setup the cluster of raspberry pi for the displays at Web à Québec.

## Setup

Set hostnames or IPs in `hosts` file.

Specify the URL to display for each host with `kiosk_url=`.

Specify the display orientation with `rotate=`. 
(See rotate options here)[http://elinux.org/RPiconfig].

## Running Ansible

Run Ansible with ask for password first time :

    ansible-playbook playbook.yml -i hosts --ask-pass

Then you can skip pass since authorized keys are setup :

    ansible-playbook playbook.yml -i hosts

# Credits

Jean-Philippe Doyle & Web à Québec.

Thanks to the authors of the following articles for the basis of my setup :

- https://www.danpurdy.co.uk/web-development/raspberry-pi-kiosk-screen-tutorial/
- http://www.stinebaugh.info/ansible-playbook-to-create-a-minimal-headless-raspberry-pi/
- https://sendgrid.com/blog/complete-guide-set-raspberry-pi-without-keyboard-mouse/
