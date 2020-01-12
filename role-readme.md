Role Name
=========

This role configure Timezone and NTP servers

Example Playbook
----------------

Example how to use this role:

    - hosts: all
      roles:
        - {role: ansible-role-ntp, timezone: Europe/Brussels, ntp.server: time.google.com}

License
-------

See license.md

Author Information
------------------

Florian Furlanetto - ffurlanetto@adneom.com
