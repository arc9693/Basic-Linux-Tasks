# Solution 1:
 
- mkdir Music
- mkdir Audio

- for i in {1..10}; do
  touch "song${i}.mp3"
done

- mv song*.mp3 Music/
- ln -s "$(pwd)/Music" Audio

# Solution 2:

- sudo groupadd sysadmin
- sudo useradd -G manager -m bob
- sudo useradd -G manager -m rob
- sudo useradd -m max
- echo 'linux123' | sudo passwd --stdin bob
- echo 'linux123' | sudo passwd --stdin rob
- echo 'linux123' | sudo passwd --stdin max

# Solution 3:

- sudo usermod --shell /bin/false max 
- sudo chage --expiredate $(date -d "+30 days" +%Y-%m-%d) max
- sudo passwd --expire bob

# Solution 4:

- sudo mkdir  /home/manager
- sudo chown :manager /home/manager
- sudo chmod 770 /home/manager
- sudo chmod g+s /home/manager

# Solution 5:

- sudo useradd -u 4223 gabriel
- sudo passwd gabriel

# Solution 6:

- sudo tar -cjvf /tmp/var/archive.tar.bz2 /etc/hosts
     # -c = Create 
     # -j = Compress archive using "bzip2"
     # -v = Verbose mode
     # -f = Spacify file name

# Solution 7:

- grep "udp" /etc/services > udp_services.txt


# Solution 8:

- top / htop


# Solution 9:

- vi /etc/bashrc
- alias stat='/bin/uptime'
- source ~/.bashrc


# Solution 10:

- vim example.txt {To create file}
- press "i" to get into INSERT mode.
- Highlight the line you want to delete, then hit "dd" or "D".
- press ":q!" to quit without saving.
- press ":wq" to write and quit.


# Solution 11:

- sudo firewall-cmd --get-default-zone
- firewall-cmd --set-default-zone=dmz
- firewall-cmd --list-all-zones > zones.txt


# Solution 12:

- sudo firewall-cmd --add-port=8080/tcp --permanent 
- sudo firewall-cmd --reload
- netstat -tuln >> zones.txt {t=TCP & u=UDP}


# Solution 13:

- sudo firewall-cmd --zone=public --add-forward-port=port=80:proto=tcp:toport=8080 --permanent
- sudo firewall-cmd --reload


# Solution 14:

- sudo vim /etc/apt/sources.list
- {Locate the lines corresponding to the repository you want to change (e.g., main, universe, multiverse, etc.), and replace the existing mirror URL with the URL of your desired mirror.}
Example = In Ubuntu and want to change the mirror for the main repository.
- deb http://archive.ubuntu.com/ubuntu/ latest main
> Make sure to replace "latest" with actual Ubuntu version.

-------------------------------------------{}--------------------------------------------------

# Thanks for your time. If you like it then please do support me so that i can get a job to start with. Thanks again. Be healthy and have fun!












