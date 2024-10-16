
ARK Cheat Detector
===========================

A batch script developed to detect well-known cheats and hacks related to ARK: Survival Evolved on Windows systems. This tool is designed to scan for cheat files, processes, network activities, and suspicious registry entries commonly associated with ARK cheats, including those used for duping exploits via RDP (Remote Desktop Protocol).

Features

- Detects Well-Known ARK Cheats: Searches for cheat files, processes, and registry entries related to popular ARK hacks like "unleashed", "headshot", "addicted", and others, including RDP-related exploits.
- Duping Detection: Includes detection of cheats or exploits that utilize RDP services for duping in ARK.
- Comprehensive Scan: Scans critical system directories, running processes, network connections, registry, and even WinRAR’s recent files for evidence of cheats.
- PowerShell Enhanced Checks: Utilizes PowerShell commands for deeper process and file analysis.
- Windows Defender Scan: Checks Windows Defender's protection history for cheat-related alerts.
- Detailed Logging: Creates a detailed log of the scan results on your desktop for review.

Prerequisites

- Windows OS: This script is designed for Windows systems.
- Administrator Privileges: Running the script as an administrator is recommended to ensure full system access.
- PowerShell: PowerShell must be available on your system (pre-installed on most Windows versions).

How to Use

1. Download the Script: Clone or download the script from this repository.

   ```bash
   git clone https://github.com/your-username/ark-cheat-detection-script.git
   ```

2. Run the Script: Double-click the `ark-cheat-detection.bat` file or run it from a command prompt with administrative privileges.

3. Check Results: The scan results will be saved in a log file on your desktop called `cheat_scan.log`.

Script Overview

- **Log Initialization**: The script initializes a log file with headers containing system details such as PC name and current date/time.
  
- **File Search**: Scans directories like `C:\Program Files`, `AppData`, and `Downloads` for known ARK cheat files including `arkinjector`, `HSLoader.exe`, and others, including RDP-related exploits.

- **Process Search**: Monitors running processes for ARK cheat-related activity, including those associated with Remote Desktop Protocol (RDP) services for duping.

- **Network Connections**: Checks for cheat-related terms in current network connections using `netstat`, especially those related to RDP usage.

- **Registry Check**: Searches specific registry keys for cheat entries, commonly used by ARK cheats and duping exploits via RDP.

- **WinRAR History**: Scans WinRAR's recent files for ARK cheats stored in archives.

- **PowerShell Checks**: Executes PowerShell commands to perform deeper scans of processes and file systems for ARK cheats, including RDP-based tools for duping.

- **Windows Defender Scan**: Checks Windows Defender logs for cheat-related activities, including RDP services.

Well-Known ARK Cheats Detected

The script is designed to detect a range of well-known ARK cheats, including but not limited to:
- **arkinjector**
- **proofcore**
- **ring-1**
- **headshot**
- **primal**
- **unleashed**
- **addicted**
- **RDP-related terms** such as `RDPCheck.exe`, `rdpwup.exe`, and other Remote Desktop Protocol exploits used for duping.
- and more.

Customization

- **Search Paths**: You can modify the `searchPaths` variable in the script to scan specific directories on your system.
- **Search Terms**: Add or remove terms in the `searchTerms` list to detect specific ARK cheats or RDP-based duping exploits.

Example Log Output

An example of the output stored in the log file:

```
==========================================
        ARK Cheat Detection Script
==========================================
Developed by: ThunderDoesDev
Version: 1.0
==========================================
Date: 10/16/2024 Time: 14:22:56.00
PC Name: My-PC
==========================================
[INFO] Searching for cheat files...
[ALERT] Cheat detected: arkinjector found in C:\Users\User\AppData\Local\Temp\
[INFO] Checking for suspicious processes...
[ALERT] Cheat process detected: HSLoader.exe
[ALERT] Cheat process detected: RDPCheck.exe
[INFO] Checking network connections...
...
[INFO] Scan complete. Check C:\Users\User\Desktop\cheat_scan.log for details.
```

License

This project is licensed under the APACHE License - see the [LICENSE](LICENSE) file for details.

## Support

For support, issues, or enhancements, please open an issue in this repository or join our discord support server.

[Join Support Server](https://discord.gg/thunderdoesdev)
