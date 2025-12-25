# 🗓️ DAY 3 – Linux Fundamentals (Part 1)

Platform: **TryHackMe**  
Room: **Linux Fundamentals Part 1**

---

## 🎯 Objectives
- Understand basic Linux commands
- Learn file structure and navigation
- Understand file permissions and ownership
- Practice creating users and changing access

---

## 📂 Basic Linux Commands
# (Your existing commands like pwd, ls, cd, etc.)
# Keep your explanations here

---

## 🔐 File Permissions
# (Your existing explanations for chmod, chown, etc.)

---

## 🛠️ Hands-on Tasks
# (Existing tasks like creating users, testing files, changing permissions)

---

## Commands + Explanations
### pwd
Prints the current working directory, showing exactly where you are.

### ls
Lists files and directories.
- `ls -l` → shows permissions, owner, size, modification date
- `ls -a` → includes hidden files

### cd
Changes the current directory.
- `cd ..` → move up one directory
- `cd ~` → go to home directory
- `cd /` → go to root directory

### chmod
Changes file permissions.
- Example: `chmod 700 file.txt` → owner full access, others none

### chown
Changes file ownership.
- Example: `sudo chown alice:alice file.txt` → sets owner and group to 'alice'

### touch
Creates a new empty file.
- Example: `touch secret.txt`

### mkdir
Creates a new directory.
- Example: `mkdir notes`

### su
Switches user accounts to test access.
- Example: `su alice`

## Services in Linux

### What services do
Services are background programs that run automatically.
They handle system tasks such as:
- Scheduling jobs (cron)
- Logging (rsyslog)
- Networking
- Time synchronization

They usually start at boot and run without user interaction.

### Identifying running services
I used:
systemctl list-units --type=service --state=running

This showed all active services on the system.

### Stopping and restarting a service
I worked with the cron service.

To stop it:
sudo systemctl stop cron

While cron was stopped, scheduled jobs did not run.

To restart it:
sudo systemctl start cron

After restarting, scheduled tasks worked again.

### Why attackers care about services
Attackers care about services because:
- Services often run with high privileges
- Vulnerable services can give attackers persistence
- Attackers can disable services to hide activity
- Misconfigured services can be exploited for privilege escalation
