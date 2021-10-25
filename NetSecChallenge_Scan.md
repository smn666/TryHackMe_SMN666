# Nmap 7.91 scan initiated Mon Oct 25 04:19:24 2021 as: nmap -p- -vv -oN NetSecChallengeScan 10.10.209.231

Increasing send delay for 10.10.209.231 from 0 to 5 due to 64 out of 212 dropped probes since last increase.

Nmap scan report for 10.10.209.231

Host is up, received syn-ack (0.23s latency).

Scanned at 2021-10-25 04:19:24 EDT for 3305s

Not shown: 65529 closed ports

Reason: 65529 conn-refused

PORT      STATE SERVICE      REASON

22/tcp    open  ssh          syn-ack

80/tcp    open  http         syn-ack

139/tcp   open  netbios-ssn  syn-ack

445/tcp   open  microsoft-ds syn-ack

8080/tcp  open  http-proxy   syn-ack

10021/tcp open  unknown      syn-ack


Read data files from: /usr/bin/../share/nmap

# Nmap done at Mon Oct 25 05:14:29 2021 -- 1 IP address (1 host up) scanned in 3305.73 seconds
