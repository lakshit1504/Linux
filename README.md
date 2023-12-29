Overview
internsctl is a custom Linux command designed to streamline various system-related tasks. This  script provides functionalities for user management, CPU information retrieval, memory information retrieval, and detailed file information extraction. The script aims to simplify common tasks through a user-friendly command-line interface.

Features
User Management
Create a User


internsctl user create <username>
This command creates a new user with login access and a home directory. Replace <username> with the desired username.




internsctl user list [--sudo-only]
List all regular users or users with sudo permissions. Use the --sudo-only option to list only users with sudo permissions.

System Information
CPU Information


internsctl cpu getinfo
Display detailed CPU information using the lscpu command.

Memory Information


internsctl memory getinfo
Retrieve memory information using the free command.

File Information
Get File Information


internsctl file getinfo [options] <file-name>
Obtain detailed information about a file. Options include:

--size, -s: Print file size.
--permissions, -p: Print file permissions.
--owner, -o: Print file owner.
--last-modified, -m: Print last modified time.
Usage
Installation
Clone the repository to your local machine:



git clone https://github.com/your-username/internsctl.git
cd internsctl
Make the script executable:



chmod +x internsctl
Execution
Run the command with desired options:



./internsctl [options]
Replace [options] with the desired command and arguments as specified in the Features section.

Documentation
For detailed documentation on command usage, refer to the manual page:



man ./internsctl
Contribution
Feel free to contribute to the development of internsctl. Fork the repository, make your changes, and submit a pull request.
