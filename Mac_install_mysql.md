# Resolving MySQL Installation Issues on macOS Using Homebrew

This document focuses on common issues faced during the installation and setup of MySQL 8.0 on macOS using Homebrew and their solutions.

---

## **Problem 1: Authentication Plugin Error**

### Error
ERROR 2059 (HY000): Authentication plugin ‘caching_sha2_password’ cannot be loaded
### Solution
1. Start MySQL in safe mode:
   ```bash
   sudo /usr/local/opt/mysql@8.0/bin/mysqld_safe --skip-grant-tables &
   
2.	Log in without a password:
     ```bash
     mysql -u root

3.	Update the root user:
    ```bash
    ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'your_password';
    FLUSH PRIVILEGES;

4. Restart MySQL:
    ```bash
    brew services restart mysql@8.0

## **Problem 2: Socket File Issues**
### Solution
1.	Check for the socket file:
     ```bash
     ls -l /usr/local/var/mysql/mysql.sock
     
2. If missing, restart MySQL:
    ```bash
    brew services restart mysql@8.0
    ls -l /usr/local/var/mysql/mysql.sock
     
3.	Then create a symbolic link:
   	  ```bash
      sudo ln -s /usr/local/var/mysql/mysql.sock /tmp/mysql.sock


## **Problem 3: Old MySQL Version Conflicts**
After installing MySQL 8.0, an older version like MySQL 5.6 is still being used.
### Solution
1.	Remove old MySQL binaries:
     ```bash
     brew uninstall mysql
     sudo rm -rf /usr/local/var/mysql
     sudo rm -rf /usr/local/etc/my.cnf

2.	Reinstall MySQL 8.0:
     ```bash
     brew install mysql@8.0
     brew link --overwrite mysql@8.0
 
3. Update the PATH to use MySQL 8.0 binaries:
      ```bash
      export PATH="/usr/local/opt/mysql@8.0/bin:$PATH"
  
4.Make it persistent:
     ```bash
     echo 'export PATH="/usr/local/opt/mysql@8.0/bin:$PATH"' >> ~/.zshrc
     source ~/.zshrc
