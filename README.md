## Efihelper
Efihelper program, works as boot manager assistant on Debian and Ubuntu based systems.


## Dependencies
- Systemd (optional (if systemdboot method selected))
- Lsb-release
- Efibootmgr


## Install
```
git clone (this repo)

cd debianefistubhelper

sudo install -Dm755 ./efihelper /usr/local/bin/efihelper
```

## Usage
#### Initial setup:
sudo efihelper first 


#### Install new kernel entry:
```sudo efihelper install $(uname -r)```
or
```sudo efihelper install 5.14.15-xanmod1```


#### Remove kernel entry:
```sudo efihelper remove $(uname -r)```
or
```sudo efihelper remove 5.14.15-xanmod1```


## Changelog
```
v1.1 : Added systemdboot support
 |-> : Some variables fixed
 \-> : Script cleaned
```
