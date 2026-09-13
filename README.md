NickTonks_Astrophotography Seestar Station Copy & Organiser Tool (v1.2)

A lightweight Windows HTA/Batch utility designed to detect ZWO Seestar devices on your local network (Station Mode or Direct Access) and automatically copy, sort, and organize your astrophotography files using Windows Robocopy.

Features

Dual Connection Modes: Supports both Home Wi-Fi (Station Mode dynamic IPs) and Direct Access Mode (standard static IP).

Automated & Manual Discovery: Automated subnet scanning via Ping/DNS or manual IP validation for quick targeting.

Organized Folder Structure: Automatically categorizes files into subfolders by target name:

[Destination]\[Target Name]\Lights (.fit, .fits)

[Destination]\[Target Name]\Video (.mp4, .avi)

[Destination]\[Target Name]\JPEGS (.jpg, .jpeg)

Robocopy Engine: Fast, incremental transfers that skip existing files and save detailed per-device log files (Seestar_X.log).

Transfer Controls: Simple controls to start, pause, and resume ongoing transfer jobs.

Automatic Registry Cleanup: Configures SMB guest authentication settings (AllowInsecureGuestAuth) during runtime and offers to revert them to standard Windows defaults upon exit.

System Requirements & Prerequisites

OS: Windows 10 / 11 (requires Administrator privileges to modify SMB guest auth registry keys).

Dependencies: Microsoft HTML Application (mshta.exe), PowerShell, Windows Script Host (WScript.Shell), and Robocopy.

Network: PC and Seestar telescope must be on the same Wi-Fi network (Station Mode) or connected directly to the Seestar Wi-Fi hotspot.

How to Use

Launch the Application: Run the script file (.bat or .hta). Accept the Administrator prompt (UAC) to allow registry configuration for SMB access.

Landing Page: Review connection modes, network scanning options, and the disclosure details, then click Launch Transfer Tool.

Discover Devices:

Click Run Automatic Scan to sweep your local network for active Seestar devices, or

Click Add Manual IPs to directly enter a known IP address (e.g., 192.168.1.150 or 10.0.0.1).

Choose Destination Folder: Click Browse... in Section 3 to choose where your astrophotography files will be saved.

Select File Types: Filter which formats to copy (FITs, Video, Images).

Start Transfer: Click Start Transfer. The app will launch File Explorer to your destination and display real-time logs in the status window.

Exit: Click Close and Exit. Select Yes when prompted to revert Windows SMB registry policies back to system defaults.

Network Share Credentials

If Windows prompts for network credentials when accessing the Seestar share (\\<IP>\EMMC Images):

Username: guest

Password: (leave blank)

Author & Socials

Author: Nick Tonks

Instagram: @NICKTONKS_ASTROPHOTOGRAPHY
