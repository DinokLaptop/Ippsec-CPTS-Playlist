# IppSec CPTS Prep Wordlists And Web Commands
### By DinokLaptop


<br />
<br />


# Table of Contents
- **Enumeration**
  - [Directory Enumeration Wordlists](#Directory-Enumeration-Wordlists)
  - [Sub-Domain Enumeration Wordlists](#Sub-Domain-Enumeration-Wordlists)
- **Commands**
  - [Sub-Domain Enumeration Commands](#Sub-Domain-Enumeration-Commands)
  - [Backup Enumeration Commands](#Backup-Enumeration-Commands)
  - [Wordpress Plugin Enumeration Commands](#Wordpress-Plugin-Enumeration-Commands)
- [Every Wordlist](#Every-Wordlist)
- [Every Command](#Every-Command)


<br />
<br />


## Directory Enumeration Wordlists

|	Folder	|	Name Of Wordlist	|	# Of Times Used	|	Video URL	|	File Location	|
|	:---:	|	:---:	|	:---:	|	:---:	|	:---:	|
|	seclists	|	`raft-small-words.txt`	|	3	|	https://youtu.be/z5pdizHDvt8 <br /> https://youtu.be/V_CkT7xyiCc <br /> https://youtu.be/N2ahkarb-zI	|	`/usr/share/wordlists/seclists/Discovery/Web-Content/raft-small-words.txt`	|
|	dirbuster	|	`directory-list-2.3-medium.txt`	|	1	|	https://youtu.be/iyYqgseKUPM	|	`/usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt`	|


<br />
<br />


## Sub-Domain Enumeration Wordlists

|	Folder	|	Name Of Wordlist	|	# Of Times Used	|	Video URL	|	File Location	|
|	:---:	|	:---:	|	:---:	|	:---:	|	:---:	|
|	seclists	|	`bitquark-subdomains-top100000.txt`	|	1	|	https://youtu.be/AJc53DUdt1M	|	`/usr/share/wordlists/seclists/Discovery/DNS/bitquark-subdomains-top100000.txt`	|
|	seclists	|	`subdomains-top1million-5000.txt`	|	1	|	https://youtu.be/vsgPsMZx59w	|	`/usr/share/wordlists/seclists/Discovery/DNS/subdomains-top1million-5000.txt`	|


<br />
<br />


## Sub-Domain Enumeration Commands

|	Command	|	What It Does	|	Video URL	|	Note	|
|	:---:	|	:---:	|	:---:	|	:---:	|
|	`ffuf -u <URL> -H "Host: FUZZ.<DOMAIN.HTB>" -w /usr/share/wordlists/SecLists/DNS/bitquark-subdomains-top100000.txt`	|	Sub-Domain brute-force search	|	https://youtu.be/AJc53DUdt1M	|		|


<br />
<br />


## Backup Enumeration Commands

|	Command	|	What It Does	|	Video URL	|	Note	|
|	:---:	|	:---:	|	:---:	|	:---:	|
|	`gobuster dir --url <URL> -w <WORDLIST> -db`	|	Appends common backup extentions to the wordlist entries	|	https://youtu.be/p8mIdm93mfw 	|	This video explains the backup appending: https://youtu.be/JpzREo7XLOY?t=1447 <br /> This is his fix: https://github.com/IppSec/gobuster	|


<br />
<br />


## Wordpress Plugin Enumeration Commands

|	Command	|	What It Does	|	Video URL	|	Note	|
|	:---:	|	:---:	|	:---:	|	:---:	|
|	`wpscan --url <URL> --detection-mode aggressive --plugins-detection aggressive`	|	Brute-force search of every plugin	|	https://youtu.be/Alx5KQWq7ZM	|	It is slow, but worth it	|


<br />
<br />


# Every Wordlist

|	Folder	|	Name Of Wordlist	|	# Of Times Used	|	Video URL	|	File Location	|
|	:---:	|	:---:	|	:---:	|	:---:	|	:---:	|
|	seclists	|	`raft-small-words.txt`	|	3	|	https://youtu.be/z5pdizHDvt8 <br /> https://youtu.be/V_CkT7xyiCc <br /> https://youtu.be/N2ahkarb-zI	|	`/usr/share/wordlists/seclists/Discovery/Web-Content/raft-small-words.txt`	|
|	dirbuster	|	`directory-list-2.3-medium.txt`	|	1	|	https://youtu.be/iyYqgseKUPM	|	`/usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt`	|
|	seclists	|	`bitquark-subdomains-top100000.txt`	|	1	|	https://youtu.be/AJc53DUdt1M	|	`/usr/share/wordlists/seclists/Discovery/DNS/bitquark-subdomains-top100000.txt`	|
|	seclists	|	`subdomains-top1million-5000.txt`	|	1	|	https://youtu.be/vsgPsMZx59w	|	`/usr/share/wordlists/seclists/Discovery/DNS/subdomains-top1million-5000.txt`	|


<br />
<br />


# Every Command

|	Command	|	What It Does	|	Video URL	|	Note	|
|	:---:	|	:---:	|	:---:	|	:---:	|
|	`wpscan --url <URL> --detection-mode aggressive --plugins-detection aggressive`	|	Brute-force search of every plugin	|	https://youtu.be/Alx5KQWq7ZM	|	It is slow, but worth it	|
|	`ffuf -u <URL> -H "Host: FUZZ.<DOMAIN.HTB>" -w /usr/share/wordlists/SecLists/DNS/bitquark-subdomains-top100000.txt`	|	Sub-Domain brute-force search	|	https://youtu.be/AJc53DUdt1M	|		|
|	`gobuster dir --url <URL> -w <WORDLIST> -db`	|	Appends common backup extentions to the wordlist entries	|	https://youtu.be/p8mIdm93mfw 	|	This video explains the backup appending: https://youtu.be/JpzREo7XLOY?t=1447 <br /> This is his fix: https://github.com/IppSec/gobuster	|




<!-- 
Table template
|		|		|		|		|
|	:---:	|	:---:	|	:---:	|	:---:	|
-->
