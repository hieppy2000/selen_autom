1 - Install Cygwin with openssh
2 - Open Cygwin shell and if you don' have a group or password, then enter commands:
    - mkgroup > /etc/group
    - create passwd command: mkpasswd -cl > /etc/group
    - export CYGWIN='ntsec tty'
    - chmod +rw /etc/group
    - chmod +rw /etc/passd
    - chmod 0755 /var
    - ssh-host-config


