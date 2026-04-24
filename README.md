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

3) pg_config ---version
Ответ: 14.20

4) sudo systemctl status postgresql
Ответ: -

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
