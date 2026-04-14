# Important Links

| __  | Link | Comments |
| ------------- | ------------- | ------------- |
| Document |  https://docs.google.com/document/d/10HKnMvShzkg1FF78EwkO-9p4NnpKe9Tdz9i3_IIvXyI/edit?pli=1&tab=t.0 | |
| Putty | https://the.earth.li/~sgtatham/putty/latest/w64/putty.exe | |
| RoboShop Monolith | https://github.com/raghudevopsb89/roboshop-monolith/blob/main/README.md | |
| RoboShop MicroServices | https://github.com/raghudevopsb89/roboshop-microservices/blob/main/00-overview.md | |


## Image gallery VM.

1. Launch VM with RHEL10
2. Run the following commands

```shell
sed -i -e '/SELINUX=/ c SELINUX=disabled' /etc/selinux/config
systemctl disable firewalld
curl https://raw.githubusercontent.com/learndevopsonline/azure-public-gallery/refs/heads/main/rhel-9/files/ps1.sh -o /etc/profile.d/ps1.sh
chmod ugo+x /etc/profile.d/ps1.sh
reboot
```
3. Shutdown VM
4. Capture to gallery.
