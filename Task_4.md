Configure and testing linux(UFW) firewall rules

step 1:
install ufw(uncompilated firewall)

cmd: sudo apt install ufw -y

step 2:
on root use below command to enable ufw

cmd: sudo ufw enable

step 3:
set firewall rule of port 23 to deny

cmd: sudo ufw denhy 23/tcp

set firewall rule allow to port 22/tcp

step 4:
check the firewall rules status

cmd: sudo ufw status numbered

step 5:
try connecting to both the ports and note the output

cmd: telnet localhost 23

Troubleshoot: for connection being refused in port 22
* intall ssh server using (sudo apt install ssh)
* sudo systemctl start ssh - to start the ssh service in your local machine

images included:

1. t4_denied_tcp_23.png
2. t4_firewall_rule_update.png
3. t4_firewall_status.png
4. t4_ssh_connection.png
