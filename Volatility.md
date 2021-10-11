TryHackMe Volatility Write-up
=============================

#Created by SMN666

#Learn how to perform memory forensics with Volatility!

#Task1 : Intro

#No answer needed.

#Task2 : Obtaining Memory Samples

# What memory format is the most common?

# .raw

#The Window's system we're looking to perform memory forensics on was turned off by mistake. What file contains a compressed memory image?

#hiberfil.sys

#How about if we wanted to perform memory forensics on a VMware-based virtual machine?

#.vmem

#Task3 : Examining our patient

#Running the imageinfo command in Volatility will provide us with a number of profiles we can test with, however, only one will be correct. We can test these profiles using the pslist command, validating our profile selection by the sheer number of returned results. Do this now with the command `volatility -f MEMORY_FILE.raw --profile=PROFILE pslist`. What profile is correct for this memory image?

#WinXPSP2x86

#Take a look through the processes within our image. What is the process ID for the smss.exe process? If results are scrolling off-screen, try piping your output into less:

#368

#It's fairly common for malware to attempt to hide itself and the process associated with it. That being said, we can view intentionally hidden processes via the command `psxview`. What process has only one 'False' listed?

#crss.exe

#In addition to viewing hidden processes via psxview, we can also check this with a greater focus via the command 'ldrmodules'. Three columns will appear here in the middle, InLoad, InInit, InMem. If any of these are false, that module has likely been injected which is a really bad thing. On a normal system the grep statement above should return no output. Which process has all three columns listed as 'False' (other than System)?

#crss.exe

#Injected code can be a huge issue and is highly indicative of very very bad things. We can check for this with the command `malfind`. Using the full command `volatility -f MEMORY_FILE.raw --profile=PROFILE malfind -D <Destination Directory>` we can not only find this code, but also dump it to our specified directory. Let's do this now! We'll use this dump later for more analysis. How many files does this generate?

#12

#Now that we've seen all of the DLLs running in memory, let's go a step further and pull them out! Do this now with the command `volatility -f MEMORY_FILE.raw --profile=PROFILE --pid=PID dlldump -D <Destination Directory>` where the PID is the process ID of the infected process we identified earlier (questions five and six). How many DLLs does this end up pulling?

#12 

#Task 4 : Post Actions:

#What malware has our sample been infected with? You can find this in the results of VirusTotal and Hybrid Anaylsis. 

#Cridex

#Task 5 : Extra Credit: 

#No answer needed.

#The End ..2/5/2021
