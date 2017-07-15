Role Name
=========

Enables wake-on-lan. Doesn't require WOL to be configured using ethtool.
Tested this role it works on 16.04.01 without it. So, you don't need anything like
what done here https://github.com/ansible-roles/ansible-role-wol/blob/master/tasks/main.yml

Requirements
------------

Implemented for Ubuntu. Requires some minor tweaks for other Linux'es.

Role Variables
--------------

usb_autosuspend: 0|1. 0 - default role value.

Dependencies
------------

No dependencies as of now

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: Alex2357.wake-on-lan}

    - hosts: servers
      roles:
         - { role: Alex2357.wake-on-lan, usb_autosuspend: 1 }

License
-------

BSD

