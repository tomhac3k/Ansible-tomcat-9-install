tomcat9install
=========

Fresh Tomcat 9 (9.0.65) Most stable tomcat 9 version Install on Enterprise Linux 8 and Enterprise Linux 9

Requirements
------------

Ansible version: 2.8

Tomcat package used link: https://tomcat.apache.org/download-90.cgi

This Playbook also works on all sub versions of OEL 8, RHEL 8 and CentOS Stream 8.
This Playbook also works on all sub versions of OEL 9, RHEL 9 and CentOS Stream 9.

Role Variables
--------------

Here you need to specify the tomcat installation location.

    tomcat_location: /opt

Dependencies
------------
No Dependencies

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: Install Tomcat 9
      hosts: servers
      roles:
         -  role: tomcat9install
            vars:
              tomcat_location: /opt

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
