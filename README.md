# ssh-aktor

**ssh-aktor** is a small bash script designed to simplify the process of creating a new user with SSH key authentication on a Linux system. This script automates the creation of a new user, generates SSH key pairs, sets up the necessary directory structure, and provides instructions for testing the SSH key.

## Prerequisites

- This script must be run with sudo privileges.
- Ensure you have basic knowledge of working with SSH keys and user management on Linux.

## Usage

To use **ssh-aktor**, follow these steps:

1. Clone this repository or download the `ssh-aktor` script.
2. Make the script executable with the command: `chmod +x ssh-aktor`.
3. Run the script with sudo and provide a username as an argument. For example:
   ```bash
   sudo ./ssh-aktor <username>
   ```
   Replace `<username>` with the desired username for the new user.

## Features

- Automatically creates a new user with SSH key authentication.
- Generates a random password for the new user.
- Creates the necessary directory structure and sets appropriate permissions.
- Copies the generated private key to the sudo user's home directory for easy access.
- Provides instructions for testing the SSH key.

## Example

```bash
sudo ./ssh-aktor coderunner
```

This command creates a new user with the username `coderunner`. It generates an SSH key pair for this user and provides instructions on how to test the SSH key.

## Note

- It's recommended to review the generated SSH key and ensure it's securely handled.
- For production environments, consider additional security measures and user management practices.

Feel free to contribute to this project or report any issues on GitHub. Your feedback is highly appreciated!
