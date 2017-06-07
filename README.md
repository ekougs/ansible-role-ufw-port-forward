Ansible role: ufw-port-forward
=========

An ansible role that enables port forwarding with ufw

Requirements
------------

ufw installed on the server

Role Variables
--------------

The list of ports forward settings
It is required

    ufw_port_forward_settings

An example is available in the example playbook below  
All fields are required because used 

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
        - role: ekougs.ufw-port-forward
      vars:
        - ufw_port_forward_settings:
            - src_interface: enp0s3
              src_ip: 10.0.2.15
              src_port: 80
              dest_ip: 127.0.0.1
              dest_port: 8080

License
-------

MIT / BSD

Author Information
------------------

[Pascal Ekouaghe](https://www.linkedin.com/in/pascal-ekouaghe-93972028/)
