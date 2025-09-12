# 1. Generate SSH Key

## Add SSH key vào máy vừa cài đặt

```
~ ssh-copy-id vannghia@labkeeper.nlab.lan
/usr/bin/ssh-copy-id: INFO: Source of key(s) to be installed: ssh-add -L
/usr/bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
/usr/bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
vannghia@labkeeper.nlab.lan's password:
Permission denied, please try again.
vannghia@labkeeper.nlab.lan's password:

Number of key(s) added:        1

Now try logging into the machine, with: "ssh 'vannghia@labkeeper.nlab.lan'"
and check to make sure that only the key(s) you wanted were added.
```

## Gán quyền sudo cho user quản trị viên (non-root)

```
~ su # switch to root user
~ apt update && apt install sudo
~ sudo usermod -aG sudo vannghia
~ groups vannghia # Verify the account has been added to sudo group
vannghia : vannghia cdrom floppy sudo audio dip video plugdev users netdev
```

# Install Ansible

```
sudo apt update && sudo apt install ansible
```

