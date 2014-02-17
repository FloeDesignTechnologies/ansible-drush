ansible-drush
========

Ansible role to install Drush.

Example usage:

    - role: drush
      drushrc:
        root: /var/www
        uri: www.example.com

Role Variables
--------------

* **drushrc**: The content of the global Drush configuration file (/etc/drush/drushrc.php) as a dict.

Requirements
------------

* The php-pear role is used to install PEAR, discover the Drush's channel and install Drush.

License
-------

Apache v2

Author Information
------------------

Pierre Buyle <buyle@pheromone.ca>