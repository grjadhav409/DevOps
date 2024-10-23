### Linux Cheat Sheet for DevOps



---

#### **1. Basic Navigation & File Management**

| Command          | Description                                |
|------------------|--------------------------------------------|
| `pwd`            | Print current working directory            |
| `ls -l`          | List files with detailed info              |
| `cd /path`       | Change directory                          |
| `touch filename` | Create an empty file                      |
| `mkdir dirname`  | Create a directory                        |
| `rm -rf dir`     | Remove a directory (use with caution!)     |
| `cp file1 file2` | Copy a file                               |
| `mv file1 file2` | Move or rename a file                     |
| `cat filename`   | View file content                         |
| `less filename`  | View content page by page                 |

---

#### **2. User & Permission Management**

| Command               | Description                                       |
|-----------------------|---------------------------------------------------|
| `whoami`              | Show current logged-in user                       |
| `sudo command`        | Run command as superuser                          |
| `chmod 755 filename`  | Change file permissions                           |
| `chown user:group file`| Change file owner and group                      |
| `useradd username`     | Add a new user                                    |
| `passwd username`      | Set or change user password                       |
| `groups username`      | List user groups                                  |

---

#### **3. Process Management**

| Command            | Description                               |
|--------------------|-------------------------------------------|
| `ps -ef`           | Show all running processes                |
| `top`              | Display system tasks and resource usage   |
| `htop`             | Interactive process viewer (if installed) |
| `kill PID`         | Terminate a process by its PID            |
| `killall process`  | Terminate all instances of a process      |
| `systemctl status service` | Check the status of a service       |
| `systemctl restart service` | Restart a service                  |

---

#### **4. Network & Connectivity**

| Command                   | Description                                   |
|---------------------------|-----------------------------------------------|
| `ifconfig`                | Display network interfaces (deprecated)       |
| `ip addr`                 | Display IP addresses and interfaces           |
| `ping hostname`           | Test connectivity to a host                   |
| `netstat -tuln`           | Show listening ports and services             |
| `ss -tuln`                | Faster alternative to netstat                 |
| `scp user@host:/path/file`| Secure copy file from remote server           |
| `ssh user@hostname`       | Securely connect to a remote machine          |
| `curl -I URL`             | Check HTTP headers of a URL                   |
| `traceroute hostname`     | Trace route to a host                         |

---

#### **5. Disk & File System Management**

| Command              | Description                                   |
|----------------------|-----------------------------------------------|
| `df -h`              | Show disk space usage                        |
| `du -sh /path`       | Check directory size                         |
| `mount /dev/sda1 /mnt` | Mount a file system                        |
| `umount /mnt`        | Unmount a file system                        |
| `fdisk -l`           | List disk partitions                         |
| `mkfs.ext4 /dev/sda1`| Format partition as ext4                     |
| `lsblk`              | List block devices (disks, partitions)       |

---

#### **6. Package Management**

##### **Debian/Ubuntu-based:**
| Command                        | Description                          |
|---------------------------------|--------------------------------------|
| `apt update`                    | Update package index                |
| `apt upgrade`                   | Upgrade installed packages          |
| `apt install package_name`      | Install a package                   |
| `apt remove package_name`       | Remove a package                    |

##### **RHEL/CentOS-based:**
| Command                         | Description                          |
|----------------------------------|--------------------------------------|
| `yum update`                     | Update all packages                 |
| `yum install package_name`       | Install a package                   |
| `yum remove package_name`        | Remove a package                    |

---

#### **7. Log Management**

| Command                   | Description                                  |
|---------------------------|----------------------------------------------|
| `tail -f /var/log/syslog`  | View real-time log updates                   |
| `tail -n 100 logfile`      | Show last 100 lines of a log                 |
| `grep "keyword" logfile`   | Search logs for a specific keyword           |
| `journalctl -xe`           | View system logs (journald)                 |

---

#### **8. Security & Firewall**

| Command                      | Description                                 |
|------------------------------|---------------------------------------------|
| `ufw enable`                 | Enable UFW firewall                         |
| `ufw allow 22/tcp`           | Allow SSH (port 22)                         |
| `ufw status`                 | Show firewall status                        |
| `firewalld-cmd --add-service=http` | Allow HTTP through firewall          |
| `ssh-keygen`                 | Generate SSH key pair                       |
| `ssh-copy-id user@host`      | Copy SSH key to remote server               |

---

#### **9. Backup & Sync**

| Command                                      | Description                                |
|----------------------------------------------|--------------------------------------------|
| `rsync -av /source /destination`            | Sync files/directories                     |
| `tar -czvf backup.tar.gz /path`             | Create a compressed archive                |
| `tar -xzvf backup.tar.gz`                   | Extract a compressed archive               |

---

#### **10. DevOps-Specific Tools**

| Command                   | Description                                |
|---------------------------|--------------------------------------------|
| `docker ps`               | List running Docker containers             |
| `docker-compose up`       | Start Docker containers using Compose      |
| `kubectl get pods`        | List Kubernetes pods                       |
| `kubectl apply -f config.yml` | Deploy app to Kubernetes cluster        |
| `ansible-playbook site.yml` | Run an Ansible playbook                   |
| `vagrant up`              | Start a virtual machine via Vagrant        |

---
