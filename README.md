# Install Apache Tomcat 9 on Enterprise Linux 8 and 9

Ansible Playbook to automate Tomcat 9 installation on Oracle Enterprise Linux 8, Red Hat Enterprise Linux 8 and CentOS Stream 8.
Ansible Playbook to automate Tomcat 9 installation on Oracle Enterprise Linux 9, Red Hat Enterprise Linux 9 and CentOS Stream 9.

## Tomcat version: 9 (9.0.65) and Java openjdk version: 1.8.0_342

  9.0.65 Most stable tomcat 9 version
  
## Ansible version: [core 2.12.2]

Tomcat package used link: https://tomcat.apache.org/download-90.cgi

This Playbook also works on all sub versions of OEL 8, RHEL 8 and CentOS Stream 8.

This Playbook also works on all sub versions of OEL 9, RHEL 9 and CentOS Stream 9.

## How to use this playbook

1. Download the repository
2. move only the tomcat_install.yml playbook and vars/variables.yml to your ansible environment.
3. edit the vars/variables.yml file according to your environment.

  Here you need to mention your inventory hostnames or inventory groupnames
  
    Example for a inventory hosts:- host: webservera.example.com
    
    Example for inventory groups:- host: sandbox
    
    you can also mention multiple groups and hosts
    
      host: servera.example.com
      
    These pacakges are basic that are required by the tasks to perform actions
    
    packages:
      - tar # to extract archive files
      - wget # to download war files from remote loations
      
    This will be your tomcat installation location, don't change this if you're not sure.
    
      tomcat_location: /opt/
    
### To this run playbook

   >_#: ansible-playbook tomcat_install.yml
