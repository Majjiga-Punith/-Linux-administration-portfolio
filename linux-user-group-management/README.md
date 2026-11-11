# Project 1: Linux User and Group Management

## Overview

In this project, I practised managing users, groups, file ownership, and permissions in Linux.

The goal was to create a small company-style environment where two users, Alex and Maria, could work together through a shared directory.

## Environment

- Operating system: Ubuntu 26.04 LTS
- Environment: WSL2
- Shell: Bash

## What I practised

- Creating Linux groups and user accounts
- Setting passwords for users
- Understanding primary and supplementary groups
- Adding users to supplementary groups
- Checking user and group information
- Creating and managing shared directories
- Changing file ownership and permissions
- Using the setgid permission on a directory
- Testing access and file sharing between users

## Project setup

I created a group called `IT` and two user accounts:

- `alex`
- `maria`

Both users were added to the `IT` group.

I created the shared directory:

`/srv/it-share`

The directory was configured with:

- Owner: `alex`
- Group: `IT`
- Permissions: `2770`

The setgid permission ensures that new files and directories created inside inherit the directory's group, `IT`.

## Collaboration test

I tested the shared directory by logging in as both users.

Alex and Maria were able to create files in the shared directory. I also tested appending text to a file created by the other user.

The tests confirmed that both users could collaborate through the shared directory.

## What I learned

This project helped me understand the difference between a file's owner and group, and how Linux decides who can access a file or directory.

I also learned that:

- A user's primary group is not necessarily the same as their supplementary groups.
- Directory permissions control access to the directory itself.
- The setgid bit on a directory helps new files inherit the intended group.
- `sudo` is needed for administrative operations when the current user does not have the required privileges.
- Small command mistakes are useful opportunities to understand how Linux works.

## Commands and reference

I will include a separate PDF reference guide with the commands used in this project, their explanations, and useful notes.

## Project status

Practical work completed. Documentation and publication to GitHub are in progress.
