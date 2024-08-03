# BSD

Here’s a comprehensive list of commands for FreeBSD and OpenBSD, labeled as such.

# FreeBSD Commands

## System Information

- **Check FreeBSD version:**
  ```bash
  uname -a
  ```

- **Get detailed system information:**
  ```bash
  sysctl -a
  ```

- **List installed packages:**
  ```bash
  pkg info
  ```

- **Check hardware details:**
  ```bash
  pciconf -l
  ```

## Package Management

- **Install a package:**
  ```bash
  pkg install packagename
  ```

- **Update installed packages:**
  ```bash
  pkg update
  pkg upgrade
  ```

- **Remove a package:**
  ```bash
  pkg delete packagename
  ```

- **Search for a package:**
  ```bash
  pkg search packagename
  ```

## File and Directory Management

- **List files and directories:**
  ```bash
  ls
  ```

- **Change directory:**
  ```bash
  cd directoryname
  ```

- **Create a directory:**
  ```bash
  mkdir directoryname
  ```

- **Remove a directory:**
  ```bash
  rmdir directoryname
  ```

- **Copy files:**
  ```bash
  cp sourcefile destinationfile
  ```

- **Move files:**
  ```bash
  mv sourcefile destinationfile
  ```

- **Delete files:**
  ```bash
  rm filename
  ```

- **Find files:**
  ```bash
  find /path/to/search -name "filename"
  ```

- **Search for text within files:**
  ```bash
  grep "searchtext" filename
  ```

## System Monitoring and Management

- **Check disk usage:**
  ```bash
  df -h
  ```

- **Check disk space usage by directory:**
  ```bash
  du -sh /path/to/directory
  ```

- **List all running processes:**
  ```bash
  ps aux
  ```

- **Monitor system performance:**
  ```bash
  top
  ```

- **View system logs:**
  ```bash
  less /var/log/messages
  ```

- **Check network configuration:**
  ```bash
  ifconfig
  ```

- **List all network interfaces:**
  ```bash
  ifconfig -a
  ```

## User and Permissions Management

- **List all users:**
  ```bash
  pw usershow username
  ```

- **Add a new user:**
  ```bash
  pw useradd username -m -s /bin/sh -h 0
  ```

- **Delete a user:**
  ```bash
  pw userdel username
  ```

- **Change file permissions:**
  ```bash
  chmod permissions filename
  ```

- **Change file ownership:**
  ```bash
  chown owner:group filename
  ```

## System Maintenance

- **Run disk repair:**
  ```bash
  fsck -y
  ```

- **Verify disk structure:**
  ```bash
  gpart show
  ```

- **Update the FreeBSD system:**
  ```bash
  freebsd-update fetch
  freebsd-update install
  ```

- **Check system status and health:**
  ```bash
  systat
  ```

## Networking

- **Ping a host:**
  ```bash
  ping hostname
  ```

- **Trace route to a host:**
  ```bash
  traceroute hostname
  ```

- **View network routing table:**
  ```bash
  netstat -rn
  ```

- **Manage network interfaces:**
  ```bash
  ifconfig interface
  ```

## Security

- **Check for open ports:**
  ```bash
  netstat -an
  ```

- **View firewall settings (ipfw):**
  ```bash
  ipfw list
  ```

- **View security logs:**
  ```bash
  less /var/log/security
  ```

## Miscellaneous

- **Generate a system report:**
  ```bash
  sysctl -a
  ```

- **Reboot the system:**
  ```bash
  shutdown -r now
  ```

---

# OpenBSD Commands

## System Information

- **Check OpenBSD version:**
  ```bash
  uname -a
  ```

- **Get detailed system information:**
  ```bash
  sysctl -a
  ```

- **List installed packages:**
  ```bash
  pkg_info
  ```

- **Check hardware details:**
  ```bash
  dmesg | less
  ```

## Package Management

- **Install a package:**
  ```bash
  pkg_add packagename
  ```

- **Update installed packages:**
  ```bash
  pkg_add -u
  ```

- **Remove a package:**
  ```bash
  pkg_delete packagename
  ```

- **Search for a package:**
  ```bash
  pkg_info -Q packagename
  ```

## File and Directory Management

- **List files and directories:**
  ```bash
  ls
  ```

- **Change directory:**
  ```bash
  cd directoryname
  ```

- **Create a directory:**
  ```bash
  mkdir directoryname
  ```

- **Remove a directory:**
  ```bash
  rmdir directoryname
  ```

- **Copy files:**
  ```bash
  cp sourcefile destinationfile
  ```

- **Move files:**
  ```bash
  mv sourcefile destinationfile
  ```

- **Delete files:**
  ```bash
  rm filename
  ```

- **Find files:**
  ```bash
  find /path/to/search -name "filename"
  ```

- **Search for text within files:**
  ```bash
  grep "searchtext" filename
  ```

## System Monitoring and Management

- **Check disk usage:**
  ```bash
  df -h
  ```

- **Check disk space usage by directory:**
  ```bash
  du -sh /path/to/directory
  ```

- **List all running processes:**
  ```bash
  ps aux
  ```

- **Monitor system performance:**
  ```bash
  top
  ```

- **View system logs:**
  ```bash
  tail -f /var/log/messages
  ```

- **Check network configuration:**
  ```bash
  ifconfig
  ```

- **List all network interfaces:**
  ```bash
  ifconfig -a
  ```

## User and Permissions Management

- **List all users:**
  ```bash
  getent passwd
  ```

- **Add a new user:**
  ```bash
  useradd username
  ```

- **Delete a user:**
  ```bash
  userdel username
  ```

- **Change file permissions:**
  ```bash
  chmod permissions filename
  ```

- **Change file ownership:**
  ```bash
  chown owner:group filename
  ```

## System Maintenance

- **Run disk repair:**
  ```bash
  fsck -y
  ```

- **Verify disk structure:**
  ```bash
  disklabel -p
  ```

- **Update the OpenBSD system:**
  ```bash
  syspatch
  ```

- **Check system status and health:**
  ```bash
  systat
  ```

## Networking

- **Ping a host:**
  ```bash
  ping hostname
  ```

- **Trace route to a host:**
  ```bash
  traceroute hostname
  ```

- **View network routing table:**
  ```bash
  netstat -rn
  ```

- **Manage network interfaces:**
  ```bash
  ifconfig interface
  ```

## Security

- **Check for open ports:**
  ```bash
  netstat -an
  ```

- **View firewall settings (pf):**
  ```bash
  pfctl -sr
  ```

- **View security logs:**
  ```bash
  tail -f /var/log/authlog
  ```

## Miscellaneous

- **Generate a system report:**
  ```bash
  sysctl -a
  ```

- **Reboot the system:**
  ```bash
  reboot
  ```

This list covers essential commands for managing FreeBSD and OpenBSD systems. These commands will help you perform a variety of tasks from system administration and file management to network configuration and security monitoring.
