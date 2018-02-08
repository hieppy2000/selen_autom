# 1. Install Cygwin with openssh
     - Add PATH=C:\cygwin\bin
     - Right click on cygwin program and select Run As Admministrator
     - from prompt type: ssh-host-config
     - Should StrictModes be used? (yes/no) no
     - Query: Do you want to install sshd as a service?
       - Query: (Say "no" if it is already installed as a service) (yes/no) yes
     - Enter the value of CYGWIN for the daemon: [] ntsec
     - Do you want to use a different name? (yes/no) no
     - Create new privileged user account 'DESKTOP-5NF0IB2\cyg_server' (Cygwin name: 'cyg_server')? (yes/no) yes
     - Info: Entering no password will exit the configuration.
        - Query: Please enter the password:
        - Query: Reenter:

     
# 2. Open Cygwin shell and if you don' have a group or password, then enter commands: (optional, may not need this step if step 1 is working fine)
    - mkgroup > /etc/group
    - create passwd command: mkpasswd -cl > /etc/passwd
    - export CYGWIN='ntsec tty'
    - chmod +rw /etc/group
    - chmod +rw /etc/passwd
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
    - Note that this step needs to do before run "net start sshd" service



