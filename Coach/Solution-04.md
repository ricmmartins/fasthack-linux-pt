# Desafio 04 - Conteúdo do arquivo - Guia do Coach

[<Solução anterior](./Solution-03.md) - **[Home](./README.md)** - [Próxima solução >](./Solution-05.md)

## Notas e Orientações
1. Exiba as primeiras 10 linhas de `/etc/resolv.conf`

`student@vm01:~$ head -10 /etc/resolv.conf`

```bash
# This file is managed by man:systemd-resolved(8). Do not edit.
#
# This is a dynamic resolv.conf file for connecting local clients to the
# internal DNS stub resolver of systemd-resolved. This file lists all
# configured search domains.
#
# Run "resolvectl status" to see details about the uplink DNS servers
# currently in use.
#
# Third party programs must not access this file directly, but only through the
```

2. Exiba as últimas 5 linhas de `/etc/crontab`

`student@vm01:~$ tail -5 /etc/crontab`

```bash
17 * * * * root cd / && run-parts --report /etc/cron.hourly
25 6 * * * root test -x /usr/sbin/anacron || ( cd / && run-parts --report /etc/cron.daily )
47 6 * * 7 root test -x /usr/sbin/anacron || ( cd / && run-parts --report /etc/cron.weekly )
52 6 1 * * root test -x /usr/sbin/anacron || ( cd / && run-parts --report /etc/cron.monthly )
#
```

3. Use cat para criar um arquivo chamado `count.log` que se parece com este

    One<br>
    Two<br>
    Three<br>
    Four<br>
    Five

```bash
cat > count.log
One
Two
Three
Four
Five 
```

4. Use cp para fazer um backup deste arquivo para `count.bkp`

`student@vm01:~$ cp count.log count.bkp`

5. Use cat para fazer um backup deste arquivo salvando como cat-count.log

`student@vm01:~$ cat count.log > cat-count.log`

6. Exibir cat-count.log, mas com todas as linhas na ordem inversa

`student@vm01:~$ tac cat-count.log`

```bash
Five
Four
Three
Two
One
```

7. Use `more` para exibir `/etc/selinux/semanage.conf`

`student@vm01:~$ more /etc/selinux/semanage.conf`

8. Use ls para encontrar o maior arquivo em /var/log

`student@vm01:~$ ls -lS /var/log`

```bash
total 5676
-rw-r-----  1 syslog    adm             1066712 Apr 10 00:00 auth.log.1
-rw-r-----  1 syslog    adm              980087 Apr  9 23:37 kern.log.1
-rw-r-----  1 syslog    adm              928447 Apr 11 16:47 auth.log
-rw-rw----  1 root      utmp             594816 Apr 11 15:15 btmp
-rw-r-----  1 syslog    adm              452142 Apr 11 00:00 syslog.1
-rw-r-----  1 syslog    adm              407078 Apr 11 16:43 kern.log
-rw-r-----  1 syslog    adm              389805 Apr 11 16:46 syslog
-rw-r--r--  1 syslog    adm              307950 Apr  7 00:29 cloud-init.log
-rw-rw-r--  1 root      utmp             293460 Apr 11 15:19 lastlog
-rw-r--r--  1 root      root             191434 Apr 11 16:37 waagent.log
-rw-r-----  1 syslog    adm              137907 Apr  8 00:00 syslog.4.gz
-rw-r-----  1 syslog    adm               50636 Apr 10 00:00 syslog.2.gz
-rw-r-----  1 syslog    adm               44039 Apr  9 00:00 syslog.3.gz
-rw-r--r--  1 root      adm               38987 Apr  7 00:28 dmesg
-rw-r--r--  1 root      adm               38847 Apr  6 15:03 dmesg.0
-rw-r--r--  1 root      root              33526 Apr  8 00:51 dpkg.log
-rw-rw-r--  1 root      utmp              11520 Apr 11 15:19 wtmp
-rw-r-----  1 root      adm                7717 Apr  7 00:29 cloud-init-output.log
drwxr-xr-x  2 root      root               4096 Apr  8 00:51 apt
drwx------  3 root      root               4096 Apr  6 15:05 azure
drwxr-xr-x  2 _chrony   _chrony            4096 Aug 25  2020 chrony
drwxr-xr-x  2 root      root               4096 Feb  8 17:14 dist-upgrade
drwxr-sr-x+ 3 root      systemd-journal    4096 Apr  6 15:02 journal
drwxr-xr-x  2 landscape landscape          4096 Apr  7 00:24 landscape
drwx------  2 root      root               4096 Apr  6 15:02 private
drwxr-x---  2 root      adm                4096 Apr  7 05:13 unattended-upgrades
-rw-r--r--  1 root      root               2290 Apr 11 13:35 ubuntu-advantage-timer.log
-rw-r--r--  1 root      root                383 Apr  4 21:57 alternatives.log

O -S classifica por tamanho de arquivo, o maior primeiro
