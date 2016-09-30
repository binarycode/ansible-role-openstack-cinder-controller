Ansible Role: OpenStack Cinder Controller
=========================================

This role installs and configures OpenStack Cinder Controller Node on EL7 system.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`)

    ip_address:

IP address in management network.

    mysql_host: controller
    mysql_password:

MySQL credentials.

    rabbitmq_host: controller
    rabbitmq_user:
    rabbitmq_password:

RabbitMQ credentials.

    keystone_host: controller
    keystone_password:

Keystone credentials for Cinder user.

    keystone_admin_token:

Keystone administration token.

    region: RegionOne

OpenStack region.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
        - binarycode.openstack-cinder-controller

License
-------

BSD

Author Information
------------------

[Igor Sidorov](https://github.com/binarycode)
