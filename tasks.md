### Tasks

1. Create 10 files having name songX.mp3 , where X should be 1-10. Move the files to Music directory.Create a symbolic link between Music directoey & Audio directory.
        
2. Create a group named "sysadmin". Create users bob and rob. They should belong to "manager" group as a secondary group. Create a user max who should not be a member of "manager" group. passwd for all users created should be "linux123".

3. User max should have non-interactive shell and the account of max should expire after 30 days. Bob should be prompted to change his password at first login. 

4. Create the Directory "/home/manager" with the following characteristics. Group ownership of "/home/manager" should go to "manager" group. The directory should be have full permission for all members of "manager" group but not to any other users except "root". Files created under "/home/manager" should get the same group ownership is set to the "manager" group.

5. Create the user gabriel with uid 4223 with password "linux123". 

6. Archive /etc/hosts to   /tmp/var/archive.tar.bz2

7. grep all lines containing "udp" from /etc/services and send the output in another file named udp_services.txt

8. Monitor the processes using top command.Sort the display by CPU utilization.

9. Create an alias where stat should run as "/bin/uptime" command. It should persist acrsoss reboots.

10. Create a file using vim text editor.(know to insert, delete and quit vim)

11. Query the current default zone. Set the default zone to "dmz". Get a list of all available zones and send the output to a file zones.txt.

12. Add port 8080/tcp. Verify by listing the ports currently listening or are active and append the output to zones.txt

13. Forward the port 80/tcp to port 8080/tcp.

  > <strong>Note:</strong> All changes should persist across reboots
