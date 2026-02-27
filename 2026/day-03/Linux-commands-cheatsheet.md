# User management Commands in Linux

# lets say username is vibs

# Create User with its home directory

sudo useradd  -m vibs  

# Create user with specific shell

sudo useradd -m -s /user/bin/bash  vibs

# Delete user

sudo userdel <username>    sudo userdel vibs

# delete user with its home directory

sudo userdel  -r vibs

# change / Create password for the user

Sudo passwd vibs

# lock user

Sudo passwd -l vibs

# unlock user 

sudo passwd -u vibs

# create a group

sudo groupadd devteam


# modify user

sudo usermod -aG docker vibs    -- this allows user to run docker because user has been added to group docker

sudo usermod -aG sudo vibs  --- user added to sudo group and user has admin access now

newgrp <group name>   -- To refresh a group

# Change file owner

sudo chown <user> <file>

# change owner and group

sudo chown user:group <File name>

# Check current user

whoami

# check user details

id vibs

# Switch user

Su devuser


# important files

/etc/passwd    -- keeps user information

/etc/shadow    -- keeps encypted password

/etc/group     -- keeps group information


# File management











