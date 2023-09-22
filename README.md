# Terraform Beginner Bootcamp 2023

## Semantic Versioning :mage:
This project is going to utlize semanctic versioning for its tagging.
[semver.org](https://semver.org/)

The general format:
**MAJOR.MINOR.PATCH**, eg. `1.0.1`
MAJOR version when you make incompatible API changes
MINOR version when you add functionality in a backward compatible manner
PATCH version when you make backward compatible bug fixes

**Resources**
Install Terraform  --> https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli
Reason: instructions have changed due to gpg keyring changes. the original gitpod.yml bash so we needed refer to the latest install cli instructions
while fixing the Terraform CLI gpg deprecition issues we noticed that bash scripts steps needed more code. decided to create a bash script (./bin/instal_terraform_cli.sh) to install the the Terraform CLI

Shebang (Unix) --> https://en.wikipedia.org/wiki/Shebang_(Unix)
linux permissions --> chmod --> https://en.wikipedia.org/wiki/Chmod
Check linux distribution --> https://www.tecmint.com/check-linux-os-version/#:~:text=The%20best%20way%20to%20determine,on%20almost%20all%20Linux%20systems.
Workspace Lifecycle - Gitpod Docs --> https://www.gitpod.io/docs/configure/workspaces/tasks

**Commands**
ls -la show hidden files
ls -la ./bin content of hiden file
ex: ls -la ./bin
total 4
drwxr-xr-x 2 gitpod gitpod  38 Sep 22 14:02 .
drwxr-xr-x 4 gitpod gitpod 113 Sep 22 13:53 ..
-rw-r--r-- 1 gitpod gitpod 683 Sep 22 14:05 install_terraform_cli.sh

**chmod**
The main parts of the chmod permissions:
For example: rwxr-x---
Each group of three characters define permissions for each class:
the three leftmost characters, rwx, define permissions for the User class (i.e. the file owner).
the middle three characters, r-x, define permissions for the Group class (i.e. the group owning the file)
the rightmost three characters, ---, define permissions for the Others class. In this example, users who are not the owner of the file and who are not members of the Group (and, thus, are in the Others class) have no permission to access the file.