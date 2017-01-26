# steps for new droplet

given will have added ssh key through DO control pannel, will still
need a password for the first login. To do so, go to the console and
click `reset root password`

get email

reset, ssh in, then create user devin

```
sudo adduser devin
passwd devin
```

add password


### give root access

```
sudo visudo
```

add line below `root ALL...`

```
devin ALL=(ALL:ALL) ALL
```

### For centos

add devin to `wheel`- has sudo by default

```
usermod -aG wheel devin
```
