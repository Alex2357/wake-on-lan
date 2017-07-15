Role Name
=========

Enables wake-on-lan.

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

