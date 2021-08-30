ansible-role-minidlna
=========

Install and configure MiniDLNA (ReadyMedia)

Requirements
------------

RHEL7 or above

Role Variables
--------------

* `minidlna_port` - port to listen for connections
* `minidlna_network_interface` - network interface to listen on
* `minidlna_ssdp_port` - SSDP port
* `minidlna_media_dirs` - list of media directories, example:

```yaml
minidlna_media_dirs:
  - /mnt/movies
  - /mnt/pictures
```

* `minidlna_friendly_name` - name to display to clients
* `minidlna_db_dir` - path to database directory
* `minidlna_log_dir` - path to log directory
* `minidlna_inotify` - boolean to enable inotify
* `minidlna_strict_dlna` - boolean to enable strict dlna
* `minidlna_notify_interval` notify interval
* `minidlna_serial` - serial
* `minidlna_model_number` - model number
* `minidlna_service_state` - state of minidlnad service
* `minidlna_service_enabled` - boolean to enable/disable minidlnad service on boot

Dependencies
------------

Collections:

* `ansible.builtin`

Example Playbook
----------------

```
- hosts: myhosts
  roles:
    - minidlna
```

License
-------

BSD

Author Information
------------------

Vladimir Vasilev
