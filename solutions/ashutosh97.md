### Task 1

```
mkdir ~/test
cd ~/test
touch song{1..10}.mp3
ls
ln -s ~/audio ~/music
```

### Task 2

```
sudo groupadd sysadmin
sudo useradd -G sysadmin bob
sudo useradd -G sysadmin rob
sudo useradd -a -G sysadmin bob -p linux123
sudo useradd -G sysadmin bob -p linux123
sudo useradd -G sysadmin rob -p linux123
sudo passwd bob
sudo passwd rob
sudo useradd -G sysadmin max -p linux123
```
