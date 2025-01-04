+++
author = "Dog"
title = "Linux useful command"
date = "2024-01-04"
description = "Exampleas of linux command."
tags = [
    "Linux",
    "Bash"
]
categories = [
    "Linux",
]
series = ["Linux Guide"]
aliases = ["migrate-from-jekyl"]
image = "ubuntu-z6rtxbp6rijb53hx.jpg"
+++


## Linux 
Linux commands for working with users: overview and benefits

> Use "sudo" before command for start command as root

Example
```bash
sudo adduser username
```
> Use commands in a structured way, like: command parameter value<br>

```bash
 rm -rf /some/dir
```

## Work with users and groups
   Command | Description
-----------|------
    adduser username\userdel username | Provides a controlled environment for each user, allows you to personalize access and avoid confusion in work. The command creates\Deletes a new user
    passwd username | Updates the password for a user. An administrator can use this command to force a password change in case of a compromise. Benefits: Maintains system security by regularly changing passwords and restoring user access.
    usermod -aG groupname username | Adds a user to a group to manage their access rights.
    who | displays logged in users
    id username | shows the user's UID, GID, and groups.
    sudo groupadd groupname | Creates a new group to organize users by shared roles or access

## Work with file and dir


   Command | Description
--------|------
    mkdir new_directory | Create new dir
  mv old_name new_name | Move to other dir
  cp file.txt /path/to/directory/ | Copy files or use with parametrs -r for copy dir
  rm file.txt | Delete files or use with paremetr -r for remove dir
  ls | Show list of files on dir. Better use with parametrs like ls -la for more info
  find /path -name "*.txt" | Search for files according to specified criteria 