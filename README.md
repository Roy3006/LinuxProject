# LinuxProject

## Overview
`sysopctl` is a custom command-line tool designed to simplify system administration tasks on Linux systems. It provides an easy interface to manage system services, monitor processes, analyze logs, and handle backups. This project is ideal for Linux administrators or users who want streamlined control over system operations.

---

## Features

### General Commands
- **Help Menu**: Display usage instructions.
  ```bash
  sysopctl --help
  ```
- **Version Information**: Show the current version of the tool.
  ```bash
  sysopctl --version
  ```

### System Operations
- **Manage Services**:
  - List active services:
    ```bash
    sysopctl service list
    ```
  - Start a service:
    ```bash
    sysopctl service start <service-name>
    ```
  - Stop a service:
    ```bash
    sysopctl service stop <service-name>
    ```
- **View System Load**:
  Display current system load averages:
  ```bash
  sysopctl system load
  ```
- **Check Disk Usage**:
  Show disk usage statistics by partition:
  ```bash
  sysopctl disk usage
  ```
- **Monitor Processes**:
  Monitor real-time process activity:
  ```bash
  sysopctl process monitor
  ```
- **Analyze Logs**:
  Summarize recent critical log entries:
  ```bash
  sysopctl logs analyze
  ```
- **Backup Files**:
  Backup files or directories to a default or specified location:
  ```bash
  sysopctl backup <path>
  ```

---

## Installation

### Clone the Repository
Clone this repository to your local system:
```bash
git clone <repository-url>
cd <repository-folder>
```

### Make the Script Executable
After cloning, make the script executable:
```bash
chmod +x sysopctl
```

### Add to PATH
To use `sysopctl` globally, move it to a directory in your PATH:
```bash
sudo mv sysopctl /usr/local/bin/
```

To verify, run:
```bash
sysopctl --help
```
You should see the help menu displayed.

---

## Example Usage

1. **List all active services:**
   ```bash
   sysopctl service list
   ```
2. **Start the `nginx` service:**
   ```bash
   sysopctl service start nginx
   ```
3. **Check system load averages:**
   ```bash
   sysopctl system load
   ```
4. **Backup a directory:**
   ```bash
   sysopctl backup /path/to/directory
   ```
5. **Analyze recent critical logs:**
   ```bash
   sysopctl logs analyze
   ```

---

## Contributing
We welcome contributions to improve the tool! If you have suggestions or find bugs, please open an issue or submit a pull request.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
