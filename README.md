Logrotate
=========

[![Build Status](https://travis-ci.org/ome/ansible-role-logrotate.svg)](https://travis-ci.org/ome/ansible-role-logrotate)
[![Ansible Role](https://img.shields.io/ansible/role/41884.svg)](https://galaxy.ansible.com/ome/logrotate/)

Customise log-rotation.


Role Variables
--------------

All variables are optional, see `defaults/main.yml`:
- `logrotate_interval`: Rotate logs at this interval (default `weekly`)
- `logrotate_backlog_size`: Number of historic log files to keep (default `12`)
- `logrotate_compress`: If True compress historic log files (default `True`)


Example Playbook
----------------

    - hosts: localhost
      roles:
      - role: ome.logrotate
        logrotate_backlog_size: 52


Author Information
------------------

ome-devel@lists.openmicroscopy.org.uk
