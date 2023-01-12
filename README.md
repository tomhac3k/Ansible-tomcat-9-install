tomcat9install
=========

Fresh Tomcat 10 (10.0.27) Most stable tomcat 9 version Install on Enterprise Linux 8 and Enterprise Linux 9

Requirements
------------

Ansible version: 2.8

Tomcat package used link: https://tomcat.apache.org/download-10.cgi

This Role also works on all sub versions of OEL 8, RHEL 8 and CentOS Stream 8.

This Role also works on all sub versions of OEL 9, RHEL 9 and CentOS Stream 9.

Role Variables
--------------

Here you need to specify the tomcat installation location.

    tomcat_location: /opt/

Dependencies
------------
No Dependencies

Example Playbook
----------------

How to use this Role in your Playbook

    - name: Install Tomcat 10
      hosts: servers
      roles:
         -  role: tomcat10install
            vars:
              tomcat_location: /opt

Expected Result
---------------

    TASK [tomcat10install : Display Installation complete Message] 
    ok: [oel9.example.com] => {
    "msg": "Tomcat 10 Installation Complete on oel9.example.com"

License
-------

BSD

Author Information
------------------

    Mohammed Tahmeed
    RHCSA 7, RHCSA 8, RHCE 8
