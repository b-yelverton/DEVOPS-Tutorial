# Self-Study Curriculum: Mastering Linux System Administration and DevOps Tools

Welcome to your self-paced learning journey towards mastering Linux system administration and essential DevOps tools. This curriculum is divided into seven comprehensive phases, each focusing on key areas to build your skills progressively.

---

## Table of Contents

- [Phase 1: Linux Fundamentals & Basic System Administration](#phase-1-linux-fundamentals--basic-system-administration)
  - [1. Set Up Your Linux Environment](#1-set-up-your-linux-environment)
  - [2. Master Basic Linux Commands](#2-master-basic-linux-commands)
  - [3. Monitor System Performance](#3-monitor-system-performance)
  - [4. Remote Access with SSH](#4-remote-access-with-ssh)
  - [5. Automate Backups with rsync](#5-automate-backups-with-rsync)
- [Phase 2: Docker & Containerization](#phase-2-docker--containerization)
  - [1. Install Docker and Docker Compose](#1-install-docker-and-docker-compose)
  - [2. Deploy Your First Docker Container](#2-deploy-your-first-docker-container)
  - [3. Set Up a Media Server](#3-set-up-a-media-server)
  - [4. Use Docker Compose for Multi-Container Applications](#4-use-docker-compose-for-multi-container-applications)
  - [5. Access Services Remotely](#5-access-services-remotely)
- [Phase 3: Automation & Scripting](#phase-3-automation--scripting)
  - [1. Develop Bash Scripts](#1-develop-bash-scripts)
  - [2. Schedule Tasks with Cron](#2-schedule-tasks-with-cron)
  - [3. Monitor and Restart Docker Containers](#3-monitor-and-restart-docker-containers)
  - [4. Manage Logs and Alerts](#4-manage-logs-and-alerts)
- [Phase 4: Networking & Secure Remote Access](#phase-4-networking--secure-remote-access)
  - [1. Secure SSH Configuration](#1-secure-ssh-configuration)
  - [2. Implement a Reverse Proxy](#2-implement-a-reverse-proxy)
  - [3. Set Up VPN Access](#3-set-up-vpn-access)
  - [4. Firewall Management](#4-firewall-management)
- [Phase 5: Version Control & CI/CD Pipelines](#phase-5-version-control--cicd-pipelines)
  - [1. Initialize Git Repositories](#1-initialize-git-repositories)
  - [2. Create a CI/CD Pipeline](#2-create-a-cicd-pipeline)
  - [3. Automate Docker Container Updates](#3-automate-docker-container-updates)
  - [4. Backup and Version Control Configurations](#4-backup-and-version-control-configurations)
- [Phase 6: Cloud Storage & Backup Solutions](#phase-6-cloud-storage--backup-solutions)
  - [1. Set Up rclone for Cloud Storage](#1-set-up-rclone-for-cloud-storage)
  - [2. Automate Cloud Backups](#2-automate-cloud-backups)
  - [3. Implement Versioning and Archiving](#3-implement-versioning-and-archiving)
  - [4. Test Backup Restoration](#4-test-backup-restoration)
- [Phase 7: Configuration Management & Documentation](#phase-7-configuration-management--documentation)
  - [1. Install and Configure Ansible](#1-install-and-configure-ansible)
  - [2. Enforce Consistency with Ansible](#2-enforce-consistency-with-ansible)
  - [3. Document Your Setup](#3-document-your-setup)
  - [4. Version Control Ansible Playbooks](#4-version-control-ansible-playbooks)
- [Additional Resources and Tips](#additional-resources-and-tips)

---

## Phase 1: Linux Fundamentals & Basic System Administration

**Objective**: Establish a solid foundation in Linux by setting up a Linux environment and mastering essential commands and system monitoring tools.

### 1. Set Up Your Linux Environment

- **Install a Linux Distribution**:
  - Download and install **Ubuntu** or a Linux distribution of your choice on your laptop using a bootable USB drive.
- **Configure the System**:
  - Set up a user account.
  - Choose disk partitioning options.
  - Install essential packages during the installation process.

### 2. Master Basic Linux Commands

- **Filesystem Navigation**:
  - Learn commands like `pwd`, `ls`, `cd`, `mkdir`, `cp`, and `rm`.
- **File Permissions and Ownership**:
  - Understand how to use `chmod` and `chown` to manage permissions.
- **Process Management**:
  - Get familiar with `ps`, `top`, and `htop` to monitor system processes.

### 3. Monitor System Performance

- **System Monitoring Tools**:
  - Install tools like `htop` and `df` to check CPU usage, memory usage, and disk space.
- **Log Management**:
  - Learn to read system logs using `journalctl` and explore logs in `/var/log/`.

### 4. Remote Access with SSH

- **Install OpenSSH**:
  - Enable remote access by installing OpenSSH on your server.
- **Secure Access Setup**:
  - Configure SSH keys for passwordless login.
  - Test remote connections from another device, such as your MacBook.

### 5. Automate Backups with rsync

- **File Synchronization**:
  - Use `rsync` to synchronize files between your seedbox and laptop.
- **Scheduled Backups**:
  - Set up cron jobs to automate regular backups.

---

## Phase 2: Docker & Containerization

**Objective**: Learn how to use Docker and Docker Compose to deploy and manage containerized applications.

### 1. Install Docker and Docker Compose

- **Docker Installation**:
  - Install Docker Engine on your Linux server.
- **Verify Installation**:
  - Run a test container using the `hello-world` image.

### 2. Deploy Your First Docker Container

- **Pull an Image from Docker Hub**:
  - Download a Docker image relevant to your interests.
- **Manage Containers**:
  - Use `docker run`, `docker ps`, and `docker stop` to manage containers.

### 3. Set Up a Media Server

- **Choose a Media Server**:
  - Select **Jellyfin** or **Plex**.
- **Configure the Container**:
  - Map appropriate volumes and ports.
  - Ensure accessibility via a web browser.

### 4. Use Docker Compose for Multi-Container Applications

- **Create a `docker-compose.yml` File**:
  - Define multiple services in one file.
- **Manage Services**:
  - Use `docker-compose up` and `docker-compose down` to control your applications.

### 5. Access Services Remotely

- **Firewall Configuration**:
  - Adjust settings to allow external access.
- **Test Accessibility**:
  - Access your services from your MacBook or other devices.

---

## Phase 3: Automation & Scripting

**Objective**: Automate routine tasks using bash scripting and cron jobs to enhance efficiency.

### 1. Develop Bash Scripts

- **Automate Synchronization**:
  - Write scripts to automate `rsync` operations.
- **Learn Bash Scripting Basics**:
  - Understand variables, conditionals, and loops.

### 2. Schedule Tasks with Cron

- **Set Up Cron Jobs**:
  - Use `crontab -e` to schedule your scripts.
- **Automate Regular Tasks**:
  - Schedule backups, updates, and other routine tasks.

### 3. Monitor and Restart Docker Containers

- **Health Checks**:
  - Write scripts to monitor container status.
- **Automatic Restarts**:
  - Restart containers if they stop unexpectedly.

### 4. Manage Logs and Alerts

- **Log Rotation**:
  - Use tools like `logrotate` to manage log files.
- **Set Up Alerts**:
  - Configure notifications for critical system events.

---

## Phase 4: Networking & Secure Remote Access

**Objective**: Configure secure networking to enable safe remote access to your server and services.

### 1. Secure SSH Configuration

- **Enhance Security**:
  - Disable password-based login.
  - Use SSH key authentication.
- **Modify `sshd_config`**:
  - Change the default port.
  - Restrict user access.

### 2. Implement a Reverse Proxy

- **Install Nginx or Traefik**:
  - Set up a reverse proxy to manage incoming requests.
- **Enable SSL/TLS**:
  - Obtain SSL certificates from Let's Encrypt.
  - Configure HTTPS for secure connections.

### 3. Set Up VPN Access

- **Choose a VPN Solution**:
  - Install **WireGuard** or **Tailscale**.
- **Configure VPN**:
  - Allow access to services on your local network securely.

### 4. Firewall Management

- **Install and Configure UFW or iptables**:
  - Set up a firewall to control traffic.
- **Define Rules**:
  - Allow only trusted connections.

---

## Phase 5: Version Control & CI/CD Pipelines

**Objective**: Use Git for version control and set up CI/CD pipelines to automate deployments.

### 1. Initialize Git Repositories

- **Track Configurations and Scripts**:
  - Use Git to version control your `docker-compose.yml`, bash scripts, and other configuration files.
- **Remote Repository Setup**:
  - Host your repositories on GitHub or GitLab.

### 2. Create a CI/CD Pipeline

- **Select a CI/CD Tool**:
  - Use **GitHub Actions** or **GitLab CI**.
- **Automate Testing and Deployment**:
  - Configure pipelines to test and deploy code upon commits.

### 3. Automate Docker Container Updates

- **Update Strategy**:
  - Write scripts or use tools like **Watchtower** to pull new images and restart containers.
- **Continuous Deployment**:
  - Implement automatic deployment of updates.

### 4. Backup and Version Control Configurations

- **Version Critical Files**:
  - Keep track of changes in configuration files.
- **Rollback Capability**:
  - Ensure you can revert to previous versions if needed.

---

## Phase 6: Cloud Storage & Backup Solutions

**Objective**: Implement cloud backups to ensure data redundancy and accessibility.

### 1. Set Up rclone for Cloud Storage

- **Configure Cloud Providers**:
  - Connect to services like Google Drive, Dropbox, or Amazon S3.
- **Data Synchronization**:
  - Use `rclone sync` to mirror directories to the cloud.

### 2. Automate Cloud Backups

- **Backup Scripts**:
  - Write scripts to automate cloud backups.
- **Scheduled Cloud Sync**:
  - Use cron jobs to run backups regularly.

### 3. Implement Versioning and Archiving

- **Data Retention Policies**:
  - Set up versioning to retain historical file versions.
- **Storage Management**:
  - Monitor and manage cloud storage usage.

### 4. Test Backup Restoration

- **Disaster Recovery Drills**:
  - Practice restoring data from backups.
- **Verify Data Integrity**:
  - Ensure backups are complete and uncorrupted.

---

## Phase 7: Configuration Management & Documentation

**Objective**: Use Ansible for configuration management and maintain thorough documentation of your setup.

### 1. Install and Configure Ansible

- **Environment Inventory**:
  - Define an inventory file for your servers.
- **Write Ansible Playbooks**:
  - Automate tasks like package installations and service configurations.

### 2. Enforce Consistency with Ansible

- **Create Reusable Roles**:
  - Develop roles for common configurations.
- **Apply Configurations**:
  - Use playbooks to enforce consistent settings across systems.

### 3. Document Your Setup

- **Use Markdown**:
  - Document procedures, configurations, and troubleshooting steps.
- **Maintain Documentation**:
  - Keep records updated with any changes made.

### 4. Version Control Ansible Playbooks

- **Track Changes**:
  - Use Git to manage your Ansible scripts.
- **Collaborate and Share**:
  - If desired, share your repositories for feedback or contributions.

---

## Additional Resources and Tips

- **Supplementary Learning**:
  - Utilize online courses and tutorials on platforms like Coursera, Udemy, or YouTube.
- **Join Communities**:
  - Participate in forums like Stack Overflow, Reddit's [r/linuxadmin](https://www.reddit.com/r/linuxadmin/), or the Docker Community Forums.
- **Hands-On Practice**:
  - Apply your skills by working on personal projects or contributing to open-source.
- **Stay Updated**:
  - Follow blogs, podcasts, or newsletters related to Linux, DevOps, and system administration.
- **Set Goals and Deadlines**:
  - Create a study schedule to keep yourself accountable.

---

**By following this structured curriculum, you'll progressively build a comprehensive skill set in Linux system administration and modern DevOps practices. Good luck on your self-study journey!**

---

### Tips for Converting to a GitHub Wiki

- **Page Structure**:
  - Each phase can be a separate wiki page for better organization.
  - Link pages using relative paths for easy navigation.
- **Images and Diagrams**:
  - Add relevant images or diagrams to enhance understanding.
- **Code Snippets**:
  - Use fenced code blocks for commands and scripts:

    ```bash
    # Example of a bash command
    sudo apt-get update
    ```

- **Internal Links**:
  - Use `[Link Text](Page-Name)` to link between wiki pages.

---

Feel free to copy and paste this Markdown content into your GitHub Wiki. The formatting should render beautifully, providing an aesthetically pleasing and well-organized structure for your self-study curriculum.
