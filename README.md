Automated Tasks
=========

Automate some stuff

* Backup Site Files & Databases
* Ship Backups To Google Cloud Storage
* Set Lifecycle Of Offsite Files

In the works

* Scan for malware
* Run security scans on server
* Check integrity of WP files
* Alerts (email + sms)

Props to A5hleyRich for the base of this - https://github.com/A5hleyRich/simple-automated-tasks

Requirements
------------

* Google Cloud Storage
* Google Compute Engine Instance
* Trellis - https://github.com/roots/trellis/

Role Variables
--------------


Dependencies
------------


Example Playbook
----------------

Add this at the end of the Trellis server.yml file:

    roles:
         - { role: automated-tasks, tags: [automated-tasks] }

License
-------

MIT

Author Information
------------------

https://github.com/RiFi2k/
