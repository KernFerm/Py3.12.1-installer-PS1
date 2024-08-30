# Python 3.12.1 Installation Script (PowerShell)

This repository contains a robust PowerShell script designed to install Python 3.12.1 on Windows. The script includes detailed logging functionality, ensuring that each step of the installation process is recorded in a log file created on your desktop.

## Features

- **Automated Installation:** The script automatically downloads and installs Python 3.12.1.
- **Detailed Logging:** All steps of the installation process are logged into a file located in a `Python_Install_Logs` folder on your desktop.
- **Error Handling:** The script checks for errors during the download, installation, and verification processes, logging any issues encountered.
- **Silent Installation:** Python is installed silently with all users having access, and the PATH variable is updated automatically.

## Usage

1. **Download the Script:**

   - Click on the `Install-Python-3.12.1.ps1` file in this repository.
   - Click the "Download" button to save the script to your local machine.

2. **Run the Script:**

   - Navigate to the location where you downloaded the script.
   - Right-click on `Install-Python-3.12.1.ps1` and select `Run with PowerShell`.

3. **Administrative Privileges:**

   - Make sure to run the script with administrator privileges to ensure proper installation and PATH updates.

## Script Breakdown

### Variables

- **$PythonVersion:** Specifies the Python version to install (3.12.1).
- **$LogDir:** Directory where the log file will be stored (on your desktop).
- **$LogFile:** The log file that records the installation process.
- **$InstallerName:** The name of the Python installer file.
- **$InstallerUrl:** The URL from which the Python installer is downloaded.

### Steps

1. **Create Log Directory:** The script first checks if the log directory exists on the desktop. If not, it creates the directory.
2. **Start Logging:** The script begins logging each step.
3. **Download Installer:** The script downloads the Python installer from the official Python website.
4. **Install Python:** The installer is run silently, installing Python for all users and updating the PATH.
5. **Verify Installation:** After installation, the script checks that Python was installed correctly by running `python --version`.
6. **Cleanup:** The installer file is deleted after a successful installation.

## Logging

All log files are stored in the `Python_Install_Logs` folder on your desktop. Each log entry includes a timestamp for easy tracking. The log file provides a detailed report on each step of the installation process, including any errors encountered.

## License

This project is licensed under the MIT License. See the [LICENSE]([LICENSE](https://github.com/KernFerm/Py3.12.1-installer-PS1/blob/main/LICENSE)) file for details.

## Contributing

If you have suggestions or improvements, please feel free to share by contacting me directly.

## Contact

For any questions or issues, please [create a issue](https://github.com/KernFerm/Py3.12.1-installer-PS1/issues).

-----------
-----------
