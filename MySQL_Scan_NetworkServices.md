# Nmap 7.70 scan initiated Fri Oct 22 00:40:34 2021 as: nmap -T4 -A -oN MySQL_Scan_NetworkServices 10.10.106.194

Nmap scan report for 10.10.106.194

Host is up (0.25s latency).

Not shown: 998 closed ports

PORT     STATE SERVICE VERSION

22/tcp   open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.3 (Ubuntu Linux; protocol 2.0)

| ssh-hostkey: 

|   2048 06:36:56:2f:f0:d4:a4:d2:ab:6a:43:3e:c0:f9:9b:2d (RSA)

|   256 30:bd:be:28:bd:32:dc:f6:ff:28:b2:57:57:31:d9:cf (ECDSA)

|_  256 f2:3b:82:4a:5c:d2:18:19:89:1f:cd:92:0a:c7:cf:65 (ED25519)

3306/tcp open  mysql   MySQL 5.7.29-0ubuntu0.18.04.1

| mysql-info:

|   Protocol: 10

|   Version: 5.7.29-0ubuntu0.18.04.1

|   Thread ID: 3

|   Capabilities flags: 65535

|   Some Capabilities: ConnectWithDatabase, SupportsTransactions, Speaks41ProtocolOld, Support41Auth, Speaks41ProtocolNew, DontAllowDatabaseTableColumn, FoundRows, IgnoreSigpipes, SupportsLoadDataLocal, IgnoreSpaceBeforeParenthesis, InteractiveClient, SupportsCompression, SwitchToSSLAfterHandshake, LongPassword, ODBCClient, LongColumnFlag, SupportsMultipleResults, SupportsMultipleStatments, SupportsAuthPlugins

|   Status: Autocommit

|   Salt: m\x0B6\x1CEm3](Ug\x03E\x07[<%?-9

|_  Auth Plugin Name: 96

No exact OS matches for host (If you know what OS is running on it, see https://nmap.org/submit/ ).

TCP/IP fingerprint:

OS:SCAN(V=7.70%E=4%D=10/22%OT=22%CT=1%CU=33325%PV=Y%DS=2%DC=T%G=Y%TM=617240

OS:E7%P=x86_64-pc-linux-gnu)SEQ(SP=105%GCD=1%ISR=107%TI=Z%CI=Z%II=I%TS=A)SE

OS:Q(SP=105%GCD=2%ISR=107%TI=Z%CI=Z%TS=A)OPS(O1=M508ST11NW7%O2=M508ST11NW7%

OS:O3=M508NNT11NW7%O4=M508ST11NW7%O5=M508ST11NW7%O6=M508ST11)WIN(W1=F4B3%W2

OS:=F4B3%W3=F4B3%W4=F4B3%W5=F4B3%W6=F4B3)ECN(R=Y%DF=Y%T=40%W=F507%O=M508NNS

OS:NW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%

OS:DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%

OS:O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%

OS:W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(R=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%

OS:RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=N%T=40%CD=S)

Network Distance: 2 hops

Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

TRACEROUTE (using port 143/tcp)

HOP RTT       ADDRESS

1   258.50 ms 10.8.0.1

2   258.58 ms 10.10.106.194


OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .

# Nmap done at Fri Oct 22 00:41:12 2021 -- 1 IP address (1 host up) scanned in 38.14 seconds
