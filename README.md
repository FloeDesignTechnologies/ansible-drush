ansible-drush
=============

Ansible role to configure [Drush](https://github.com/drush-ops/drush).

Example usage:

    - role: drush
      drushrc:
        root: /var/www
        uri: www.example.com

By default, the role does not install Drush. The **drush_pear_install_enabled** can be used to install Drush using PEAR.

Role Variables
--------------

* **drushrc**: The content of the global Drush configuration file (/etc/drush/drushrc.php) as a dict.
* **drush_pear_install_enabled**: Whenever to install Drush as a PEAR package, Defaults to ```false```.

Requirements
------------

* If **drush_pear_install_enabled** is ```true```, the php-pear role is required.

TODOs
-----

* Installation of Drush following the [INSTALL - MANUAL](https://github.com/drush-ops/drush) instructions.
* Setup drush.complete.sh for bash completion.
* Setup sites aliases.

License
-------

Apache v2

Author Information
------------------

Pierre Buyle <buyle@pheromone.ca>