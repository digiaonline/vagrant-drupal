# vagrant-drupal

Vagrant environment for Drupal projects.

# Installation

Perform the following steps to set up your environment:

- Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads), [Vagrant](http://www.vagrantup.com/downloads.html) and [Ansible](http://docs.ansible.com/intro_installation.html)
- Clone this template to e.g. ```~/projects/vagrant-drupal```
- Create a repository for your project and clone it to your computer
- Copy this template by running ```cp -R ../vagrant-drupal/* .``` in the project root (correcting the path if necessary)
- Run ```vagrant up``` to create the virtual machine
- Point your browser to ```http://localhost:1234``` to see your site
- If everything worked you can now push your changes

# Troubleshooting

- If you get an error related to mismatching vbhost versions install the [vbguest plugin](https://github.com/dotless-de/vagrant-vbguest) by running ```vagrant plugin install vagrant-vbguest``` and try again
