## Frequently used Linux Commands

---

### 1. File & Directory Management Commands

| Command          | Description                                                                                            |
| :--------------- | :----------------------------------------------------------------------------------------------------- |
| **cd**           | Changes the current working directory. Example: `cd /home/user`                                        |
| **mv**           | Moves or renames files and directories. Example: `mv file.txt /tmp/`                                   |
| **cp**           | Copies files or directories. Example: `cp file.txt backup.txt`                                         |
| **pwd**          | Prints the current working directory (shows where you are).                                            |
| **less**         | Views a file one screen at a time (scroll up/down). Example: `less /etc/passwd`                        |
| **ls**           | Lists files and directories. Example: `ls -l` for detailed view.                                       |
| **more**         | Displays text one screen at a time (similar to `less`). Example: `more file.txt`                       |
| **find**         | Searches for files and directories in a directory hierarchy. Example: `find /home -name "*.txt"`       |
| **vi, cat**      | `vi` opens a file in the text editor; `cat` displays file content. Example: `cat file.txt`             |
| **grep**         | Searches for patterns in files. Example: `grep "error" logfile.txt`                                    |
| **mkdir**        | Creates a new directory. Example: `mkdir new_folder`                                                   |
| **tar**          | Archives multiple files into one file (and extracts them). Example: `tar -cvf archive.tar file1 file2` |
| **rm**           | Removes (deletes) files or directories. Example: `rm file.txt` or `rm -r folder/`                      |
| **gzip, gunzip** | Compresses (`gzip`) or decompresses (`gunzip`) files. Example: `gzip file.txt` → `file.txt.gz`         |

---

### 2. Network Management Commands

| Command           | Description                                                                                                                                                                               |
| :---------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **curl** / **wget**   | Used to download files or interact with web servers. `curl` supports more protocols and APIs (e.g., REST calls). Example: `curl https://example.com`, `wget https://example.com/file.zip` |
| **ip** / **ifconfig** | Displays or configures network interfaces. `ip` is the modern replacement for `ifconfig`. Example: `ip addr show` or `ifconfig eth0`                                                      |
| **netstat**       | Displays active network connections, listening ports, and routing tables. Example: `netstat -tuln`                                                                                        |
| **ssh**           | Securely connects to a remote machine via the command line (Secure Shell). Example: `ssh user@192.168.1.10`                                                                               |
| **ftp**           | Transfers files between systems using the File Transfer Protocol. Example: `ftp ftp.example.com`                                                                                          |
| **ping**          | Tests connectivity to another network host and measures response time. Example: `ping google.com`                                                                                         |
| **telnet**        | Connects to remote hosts on specific ports (used for testing). Example: `telnet example.com 80`                                                                                           |

---

### 3. Process Management Commands

| Command  | Description                                                                                                                           |
| :------- | :------------------------------------------------------------------------------------------------------------------------------------ |
| **ps**   | Displays information about active processes. Common usage: `ps aux` (shows all processes with details like PID, user, and CPU usage). |
| **kill** | Terminates a process by its **PID (Process ID)**. Example: `kill 1234` or force kill using `kill -9 1234`.                            |

---

### 4. User Management Commands

| Command    | Description                                                                                                                             |
| :--------- | :-------------------------------------------------------------------------------------------------------------------------------------- |
| **id**     | Displays the user ID (**UID**), group ID (**GID**), and group memberships of the current or specified user. Example: `id` or `id tejas` |
| **whoami** | Shows the **current logged-in username**. Example: `whoami`                                                                             |
| **passwd** | Changes the **user password**. Example: `passwd` (for current user) or `sudo passwd username` (for another user)                        |
| **su**     | Switches to another user account or the **superuser (root)**. Example: `su root`                                                        |
| **sudo**   | Executes a command with **superuser (root)** privileges temporarily. Example: `sudo apt update`                                         |

----

### 5. Application Management Commands

| Command             | Description                                                                                                                                                                                                   |
| :------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **which**           | Shows the **full path** of a command or executable. Helps determine where a command is located. Example: `which python` → `/usr/bin/python`                                                                   |
| **yum / dnf / apt** | **Package managers** used to install, update, and remove software. </br>• `yum` and `dnf` → for RHEL/CentOS/Fedora </br>• `apt` → for Ubuntu/Debian. </br>Example: `sudo apt install nginx` or `sudo dnf update` |
| **systemctl**       | Controls and manages **systemd services** (start, stop, enable, disable, check status). Example: `sudo systemctl status ssh` or `sudo systemctl restart nginx`                                                |

----

### 6. Environment Variables Commands

| Command      | Description                                                                                                                               |
| :----------- | :---------------------------------------------------------------------------------------------------------------------------------------- |
| **env**      | Displays all **environment variables** or runs a command in a modified environment. Example: `env` or `env VAR=value command`             |
| **printenv** | Prints the **value of specific environment variables**. Example: `printenv PATH`                                                          |
| **export**   | Sets or makes an environment variable available to **child processes**. Example: `export JAVA_HOME=/usr/lib/jvm/java-17-openjdk`          |
| **source**   | Executes commands from a file in the **current shell session** (commonly used to load environment variables). Example: `source ~/.bashrc` |

---

### 7. Console & Output Management Commands

| Command     | Description                                                                                                                                    |
| :---------- | :--------------------------------------------------------------------------------------------------------------------------------------------- |
| **cat**     | Displays the **contents of a file**, combines multiple files, or creates new ones. Example: `cat file.txt` or `cat file1 file2 > combined.txt` |
| **clear**   | Clears the **terminal screen**. Example: `clear`                                                                                               |
| **echo**    | Prints text or variable values to the terminal. Example: `echo "Hello, World!"` or `echo $PATH`                                                |
| **history** | Displays a **list of previously executed commands**. Example: `history` or `!45` (to rerun command
#45) |

---

### 8. System Control Commands

| Command      | Description                                                                          |
| :----------- | :----------------------------------------------------------------------------------- |
| **poweroff** | Shuts down the system safely and powers it off immediately. Example: `sudo poweroff` |
| **reboot**   | Restarts the system gracefully. Example: `sudo reboot`                               |

---

### Some Other userful Commands

| Command                   | Description                                                                                                                                                                                   |
| :------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **systemctl**             | Controls and manages **systemd services** — start, stop, restart, enable, disable, or check service status. Example: `sudo systemctl restart nginx`                                           |
| **df**                    | Displays **disk space usage** for all mounted filesystems. Example: `df -h` (shows human-readable format)                                                                                     |
| **du**                    | Shows **disk usage** of files and directories. Example: `du -sh /var/log`                                                                                                                     |
| **free**                  | Displays **memory (RAM and swap)** usage. Example: `free -h`                                                                                                                                  |
| **chmod**                 | Changes **file or directory permissions**. Example: `chmod 755 script.sh`                                                                                                                     |
| **chown**                 | Changes **file or directory ownership** (user and/or group). Example: `sudo chown tejas:tejas file.txt`                                                                                       |
| **awk**, **cut**, **sed** | Text-processing commands: <br>• **awk** – pattern scanning and data extraction. <br>• **cut** – extracts sections from text lines. <br>• **sed** – stream editor for search/replace in files. |
| **ln**                    | Creates **links** between files. Example: `ln file.txt link.txt` (hard link), `ln -s /path/file link` (symbolic link).                                                                        |
| **nohup**                 | Runs a command immune to hangups (keeps running even after logout). Example: `nohup ./script.sh &`                                                                                            |
| **crontab**               | Schedules **recurring tasks** using the cron daemon. Example: `crontab -e` to edit scheduled jobs.                                                                                            |

---