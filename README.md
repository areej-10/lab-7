# lab-7
Below is a comprehensive README.md template for Lab 7, based on the provided document content which covers environment variables, system scripts, and security configurations.

Lab 7: Environment Variables, Shell Scripts, and Security Configuration
📖 Overview
This lab focuses on managing Linux environment variables, creating persistent system configurations, and securing server access using firewalls and SSH key-based authentication.

🛠 Task List & Documentation
Task 1: Exploring Environment Variables
Used basic Linux commands to inspect existing environment variables.


Commands: printenv, grep.


Deliverables: task1_printenv_all.png, task1_grep_shell_home_user.png.

Task 2: Temporary Variable Export & Scope
Observed the scope of temporary variables and their behavior across shell restarts.


Key Concept: Exporting DB_* variables.


Deliverables: task2_exports_all.png, task2_echoes_all.png, task2_printenv_grep_db.png, task2_after_restart_checks.png.

Task 3: Persistence via .bashrc
Configured DB_* variables to persist for a specific user by modifying the local bash configuration.


File Modified: ~/.bashrc.


Deliverables: task3_bashrc_added.png, task3_source_and_verification.png, task3_after_restart_persistent.png.

Task 4: System-wide Variables & Custom PATH
Implemented global environment variables and custom scripts that execute upon login.


Key Actions: * Editing /etc/environment for system-wide variables.

Creating a welcome script and modifying the PATH.


Deliverables: task4_etc_environment_after.png, task4_echo_class_and_path.png, task4_welcome_run_dot.png, task4_bashrc_source_and_welcome.png.

Task 5: Firewall Management (UFW)
Managed network traffic by blocking and allowing SSH connections.


Tool: Uncomplicated Firewall (UFW).


Deliverables: task5_ufw_enable_and_status.png, task5_ufw_deny_22_and_status.png, task5_ssh_attempt_blocked.png, task5_ssh_success_after_allow.png.

Task 6: SSH Key-Based Authentication
Configured secure, passwordless login from a Windows client to the Linux server.


Key Steps: * Generated Ed25519/RSA keys on Windows.

Managed authorized_keys and known_hosts.

Verified passwordless login using identity files.


Deliverables: task6_windows_sshkey_and_list.png, task6_server_add_key_and_show.png, task6_ssh_passwordless_login.png, task6_ssh_with_identity_file.png.

📂 Project Structure
Lab7/
├── scripts/
│   └── welcome.sh         # Custom login script
├── config/
│   ├── .bashrc            # Local user configuration
│   └── /etc/environment   # Global system variables
└── screenshots/           # All task verification images
📝 Requirements
Linux Server (Ubuntu/Debian recommended for UFW).

SSH Client (Windows PowerShell/CMD or Linux terminal).

Root or sudo privileges
