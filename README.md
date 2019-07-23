Hostname
========

Use this role to set a server's hostname. It allows using the server's EC2 `Name` tag, if the server is an AWS server.

Role Variables
--------------

### Required Variables

None currently.

### Other Default variables are listed below:

    # The server's hostname. This defaults to the hostname defined in `ansible_hostname`.
    server_hostname: "{{ ansible_hostname }}"

    # Set to `true` if you want the role to use the server's EC2 Name tag as the hostname.
    hostname_from_ec2_Name_tag: false

    # Set to `false` if you would like cloudinit to replace the hostname when launching the instance
    hostname_cloud_init_preserve_hostname: true


Requirements
------------

 - boto

License
-------

Apache 2

Authors
-------

Update by [Ona Engineering](https://ona.io)

