# Guacamole Remote Desktop Gateway
Guacamole Install Script

Installation Video -> https://www.youtube.com/watch?v=pZYuEYwBL5s

You can download -> http://sourceforge.net/projects/guacamoleinstallscript/

1- A Bare metal or a Virtual machine Server.

2- CentOS 7 (fresh install) minimal version is good.

3- Internet Connection.

4- As root execute the following:

        wget http://sourceforge.net/projects/guacamoleinstallscript/files/CentOS/guacamole-install-script.sh
        
        chmod +x guacamole-install-script.sh
        
        ./guacamole-install-script.sh
        
5- Follow the Install Wizard.

6- Added below line  this file
           vim /etc/guacamole/guacamole.properties
           
        # Properties used by BasicFileAuthanticationProvider
        basic-user-mapping: /etc/guacamole/user-mapping.xml
        
7- selinux settings
        cat /etc/selinux/config
 
        # This file controls the state of SELinux on the system.
        # SELINUX= can take one of these three values:
        #     enforcing - SELinux security policy is enforced.
        #     permissive - SELinux prints warnings instead of enforcing.
        #     disabled - No SELinux policy is loaded.
        SELINUX=disabled
        
