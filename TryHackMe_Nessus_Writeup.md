
TryHackMe Nessus Room Write-up
==============================

#Created by SMN666

#Task 1 : Introduction
No answer needed.

#Task 2 : Installation
No answer needed.

#Task 3 : Navigation Scans

#What is the name of the button which is used to launch a scan?
#New Scan

#What side menu option allows us to create custom templates?
#policies 

#What menu allows us to change plugin properties such as hiding them or changing their severity?
#plugin rules

#In the 'Scan Templates' section after clicking on 'New Scan', what scan allows us to see simply what hosts are alive?
#host discovery

#One of the most useful scan types, which is considered to be 'suitable for any host'?
#basic network scan

#What scan allows you to 'Authenticate to hosts and enumerate missing updates'?
#Credentialed Patch Audit

#What scan is specifically used for scanning Web Applications? 
#web application tests

#Task 4 : Scanning!

#Create a new 'Basic Network Scan' targeting the deployed VM. What option can we set under 'BASIC' (on the left) to set a time for this scan to run? This can be very useful when network congestion is an issue.
#schedule

#Under 'DISCOVERY' (on the left) set the 'Scan Type' to cover ports 1-65535. What is this type called?
#port scan (all ports)

#What 'Scan Type' can we change to under 'ADVANCED' for lower bandwidth connection?
#Scan low bandwidth links

#After the scan completes, which 'Vulnerability' in the 'Port scanners' family can we view the details of to see the open ports on this host?
#Nessus SYN scanner

#What Apache HTTP Server Version is reported by Nessus?
#2.4.99

#Task 4 :  Scanning a Web Application!

#What is the plugin id of the plugin that determines the HTTP server type and version?
#10107

#What authentication page is discovered by the scanner that transmits credentials in cleartext?
#login.php

#What is the file extension of the config backup?
#.bak

#Which directory contains example documents? (This will be in a php directory)
#/external/phpids/0.6/docs/examples/

#What vulnerability is this application susceptible to that is associated with X-Frame-Options?
#ClickJacking















