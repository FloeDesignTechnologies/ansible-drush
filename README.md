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

License
-------

Apache v2

Author Information
------------------

Pierre Buyle <buyle@pheromone.ca>