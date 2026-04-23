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
burger
