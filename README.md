Automated Tasks
=========

Automate some stuff

* Backup Site Files & Databases
* Save Local Backups
* Ship Backups To Google Cloud Storage (Optional)
* Ship Backups To AWS S3 (Optional)
* Set Lifecycle Of Files

If you want to use Google Cloud Storage or AWS S3 for backing up files off-site you need to manually install
and authenticate before-hand or else this role will fail. Instruction for each service
linked below.
It is important to make sure these instruction are done on the remote server and the authentication commands are
performed by the "web_user" set up in Trellis.
(default user is 'web' for production and staging unless you changed it)

#### Google Cloud Storage
https://cloud.google.com/sdk/docs/quickstart-debian-ubuntu

Initalize (must do this logged in as 'web' or make sure settings are global for all users) -
https://cloud.google.com/sdk/docs/initializing

#### AWS S3
https://github.com/aws/aws-cli

### In the works

* Scan for malware
* Run security scans on server
* Check integrity of WP files
* Alerts (email + sms)

Requirements
------------

* Trellis - https://github.com/roots/trellis/

Role Variables
--------------

See defaults/main.yml


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

Props
-----

https://github.com/A5hleyRich/simple-automated-tasks

Author Information
------------------

https://github.com/RiFi2k/
