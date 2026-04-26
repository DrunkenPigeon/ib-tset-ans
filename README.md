# ib-tset-ans
ib tset ans
МДК 01.01


1)-


2) cd /etc/
   cat passwd
   Ответ: 25


3)file /var/data/mystery.dat
Ответ: gzip compressed data


4)uname -m 
Ответ: x86_64


5)grep -c '/bin/bash' /etc/passwd
Ответ: 7 ?


6)free -m (округлить)
Ответ: 4096 


7) hostname --fqdn или cd /etc
   cat hosts
Ответ: ad73d9a22d9b или ad73d9a22d9b server.domain.local ?


8) cat /var/log/auth.log
Ответ: 192.168.1.50:14


9) sudo systemctl status auditd
    sudo systemctl status rsyslog
Ответ: active;active


10) groupadd restricted_users
    usereadd analyst
    chgrp restricted_users /srv/confidential
    chmod 3750 /srv/confidential
    Ответ: drwxr-s--T


11) cd /etc/apache2
    cd sites-enabled
    cat default.conf
Ответ: 1 (т.к некоректный IP)

12) -

13) cat /etc/ssh/sshd_config_broken
Ответ: 15;PermitRootLogin;no

МДК 01.02

1) Ответ: 3НФ
   
2) service postgresql status
Ответ: online

3) pg_config ---version или psql -V
Ответ: 14.20

4) sudo systemctl status postgresql или service postgresql status
Ответ: online

5)  Ответ: admin@company.local,backup@company.local

6)  -

7)  cat company_db.sql
Ответ: 12

8) mysqldump -u dbuser -p security_db > /tmp/backup_security.sql
   cd /tmp
   du -h backup_security.sql
   Ответ: /tmp/backup_security.sql;4 (не принимает)

9) -

10) cat company.db.sql
Ответ: 2;orders;employees

МДК 01.03

1) Ответ: транспортный

2) ifconfig или ip a show eth0
Ответ: 172.21.0.9  (не принимает)

3) Ответ: 10.20.30.5
   
4) cat /eth/resolv.conf
Ответ: 127.0.0.11

5) netstat -nt | awk '{print $6}' | sort uniq -c | grep -E "ETABLISHED|LISTEN"
Ответ: 2;6

6) ping -C 5 192.168.1.
Ответ: 0%;0,3

7) Ответ: 5

8) Ответ: ip route add 10.10.10.0/24 via 192.168.1.254

9) ip link add link eth0 name eth.100 type vlan id 100
Ответ:eth0.100

10) Ответ:987;00:15:5d:00:12:24

МДК 01.04

1) конфиденциальность

2) lsb_release -a
Ответ: smolensk

3) nginx -v
Ответ: 1.18.0

4) Ответ: 80

5) ausearch -m USER_AUTH | grep -c "^type=" Ответ: 5

6) Ответ: 3;default,api.local,admin.local

7) Ответ: auditctl -w /etc/passwd -p wa;active

8) Ответ: auth required pam_faillock.so deny=5 unlock_time=600

9) Ответ: 10:15:33;SSL_do_handshake() failed

10) Отвте: worker;50.00,512

МДК 01.05

1) Ответ: В

2) ip route
Ответ: 172.21.0.1

3) cd /etc/
   cat hostname
Ответ: 48

4) uptime
Ответ: 48

5) traceroute 8.8.8.8 Мой ответ: 8;192.168.0.1

6) -

7) Ответ: 2025-06-15

8) Ответ: ip addr add 10.20.30.40/24 dev eth1

9) Ответ: ip route add 10.10.10.0/24 via 192.168.100.254;success

10) Ответ: 10.8.0.2;192.168.100.10

11) Ответ: 8


МДК 01.06
1) Ответ: контроллер

2) ?


3) Ответ: HIGH

4) Ответ: active

5) cd /home/student/gpio/gpio17
   cat direction
   cat value
Ответ: in; 1

6) Ответ: 7;2

7) cat skud.log
   Ответ: 5

8) Ответ: stty -F /dev/ttySO 9600 cs8 -parenb -cstopb

9) Ответ: on-failure;network.target (полностью совпадает с примером из задания)

10) Ответ: 4800;9600 (смотреть файл)

11) Ответ: 5;3


МДК 02.02 
1) Ответ: симметричный

2) sudo su
   sha256sum /etc/passwd
   Ответ:
   
3) sha256sum /etc/hostname
Ответ: 8a82b80586f6dea

4) sudo su
   gpg -c --passphrase CryptoPass123 --output /home/student/secret.txt.gpg /home/student/secret.txt                                                                      после выбрать <Cancel>
   stat -c %s /home/student/secret.txt.gpg
   Ответ: secret.txt.gpg;109 или 97 (оба верные)

5) Ответ: shred -vfz -n 3 //home/student/confidential.dat

6) base64 -d message.enc
Ответ: flag{crypto_master}

7) openssl x509 -enddate -noout -in /etc/ssl/cert5/server.crt
Ответ: 2027-06-15

8) Ответ: openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/ssl/private/server.key -out /etc/ssl/certs/server.crt -subj "/CN=secure.local"

9) Ответ: cryptsetup luksOpen /dev/sda1 secure_data

10) Ответ: req -x509 -newkey rsa:4096 -days3650

11) Ответ: openssl enc -aes-356-cbc -salt -in file.txt -out file.enc


МДК 02.01 
1) systemctl status clamav-daemon
Ответ: active

2) cat /home/student/firewall/iptables_rules.txt
Ответ: ACCEPT;6

3) Ответ: 8

4) Ответ: 8

5) Ответ: shadow

6) Ответ: iptables -A INPUT -p tcp 443 -j ACCEPT

7) Ответ: 10.0.0.55;admin;48

8) Ответ: 5;3600

МДК 03.01
1) Ответ: виброакустический

2) Ответ: шумовая

3) Ответ: 4

МДК 03.02
1) Ответ: инфракрасный

2) cat /var/log/skud/events.csv
Ответ: 2

3) cat /var/lib/skud/access_control.db
Ответ: 65204


МДК 03.03
1) Ответ: 22
   
2) cat /opt/ctf/configs/network.json
  Ответ: 22

3)cat /opt/ctf/configs/network.json
 Ответ: 45

