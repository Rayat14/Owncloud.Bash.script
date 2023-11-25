# ownCloud Installation Script

This script automates the installation of ownCloud on your server, providing you with a self-hosted file sync and share solution. Before running the script, please ensure that your server meets the prerequisites.

## Prerequisites

1. **Operating System:** The script is designed for Debian-based systems.
2. **Root Access:** Ensure that you have root access or sudo privileges.

## Usage

1. **Download the Script:**

   ```bash
   wget https://path-to-your-script/owncloud-install.sh
   ```

2. **Make the Script Executable:**

   ```bash
   chmod +x owncloud-install.sh
   ```

3. **Run the Script as Root:**

   ```bash
   sudo ./owncloud-install.sh
   ```

4. **Follow the Prompts:**

   - The script will prompt you to enter the MySQL database password during the installation.

5. **Access ownCloud:**

   - Once the script completes, ownCloud should be accessible at `http://your_server_ip/owncloud`.

## Additional Information

This script not only installs ownCloud but also incorporates some basic security measures for enhanced protection:

- **HTTP Strict Transport Security (HSTS):** Ensures secure connections by enforcing the use of HTTPS.
- **X-Content-Type-Options, X-Frame-Options, and X-XSS-Protection headers:** Enhance browser security by preventing certain types of attacks.
- **Disabling Directory Listing:** Prevents Apache from showing the contents of directories.

## Important Notes

- Review the script before execution to ensure it aligns with your server and security requirements.
- Replace 'your_password' with a strong password for the MySQL database user.
- Regularly update both your system and ownCloud installation to ensure security.
