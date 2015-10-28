Role Name
=========

This configures remote logging to Papertrail (papertrailapp.com). Secure transmission with TLS will always be set up.

Requirements
------------

Currently this is only tested on CentOS7 that uses rsyslogd for syslog. Support
for other systems can be added by pull requests.

Role Variables
--------------

`papertrail_host:` URL and port provided by Papertrail. This can be found at https://papertrailapp.com/systems/setup when logged in.

Dependencies
------------

None

Example Playbook
----------------
    - hosts: servers
      roles:
         - role: Firehed.papertrail
           papertrail_host: logs.papertrailapp.com:12345

License
-------

MIT
