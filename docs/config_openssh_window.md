# 1. Install Cygwin with openssh
# 2. Open Cygwin shell and if you don' have a group or password, then enter commands:
    - mkgroup > /etc/group
    - create passwd command: mkpasswd -cl > /etc/group
    - export CYGWIN='ntsec tty'
    - chmod +rw /etc/group
    - chmod +rw /etc/passd
    - chmod 0755 /var
    - ssh-host-config
            - should restrictmodes be used? no
            - Should privilege sepratioin be used? yes
            - New local account 'sshd'? yes
            - enter the value of CYGWIN daemon? sshd
            - Do you want to use a different name? no
            - Create a new privileged user account 'cyg_server'? no
            - Do you wan tot proceed anyway? yes
     - Command to start sshd
         - net start sshd
         - net stop sshd
# 3.  Change "CYGWIN sshd" service in window to local system
    - In window, open sevices application and right click to open properties page of "CYGWIN sshd" service
    - Select Logon tab, and enable "Local System account" and enable "Allow with desktop"



