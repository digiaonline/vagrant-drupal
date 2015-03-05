# vagrant-drupal

Vagrant environment for Drupal projects.

# Installation

Perform the following steps to set up your environment:

- Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads), [Vagrant](http://www.vagrantup.com/downloads.html) and [Ansible](http://docs.ansible.com/intro_installation.html)
- Run ```vagrant up``` to create the virtual machine
- All done! Point your browser to ```http://localhost:1337``` to see your site

# Troubleshooting

- If you get an error related to mismatching vbhost versions install the [vbguest plugin](https://github.com/dotless-de/vagrant-vbguest) by running ```vagrant plugin install vagrant-vbguest``` and try again
