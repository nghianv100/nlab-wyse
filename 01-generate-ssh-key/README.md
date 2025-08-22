# Add SSH key để truy cập vào máy vừa cài đặt

```
~ ssh-copy-id vannghia@10.0.0.82
/usr/bin/ssh-copy-id: INFO: Source of key(s) to be installed: ssh-add -L
/usr/bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
/usr/bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
vannghia@10.0.0.82's password:
Permission denied, please try again.
vannghia@10.0.0.82's password:

Number of key(s) added:        1

Now try logging into the machine, with: "ssh 'vannghia@10.0.0.82'"
and check to make sure that only the key(s) you wanted were added.
```

# Cập nhật package manager

```
apt update
```
