# IppSec CPTS Prep Wordlists, Web commands

<br />

|	Folder	|	Name of wordlist	|	# of times used	|	Video URL	|
|	:---:	|	:---:	|	:---:	|	:---:	|
|	seclists	|	raft-small-words.txt	|	3	|	https://youtu.be/z5pdizHDvt8 <br /> https://youtu.be/V_CkT7xyiCc <br /> https://youtu.be/N2ahkarb-zI	|
|	dirbuster	|	directory-list-2.3-medium.txt	|	1	|	https://youtu.be/iyYqgseKUPM	|
|	seclists	|	bitquark-subdomains-top100000.txt	|	1	|	https://youtu.be/AJc53DUdt1M	|
|	seclists	|	subdomains-top1million-5000.txt	|	1	|	https://youtu.be/vsgPsMZx59w	|

<!-- 
|		|		|		|		|
|		|		|		|		|
|		|		|		|		|
-->

<br />
<br />

|	Nice commands	|	What it does	|	Video URL	|
|	:---:	|	:---:	|	:---:	|
|	wpscan --url **url** --detection-mode aggressive --plugins-detection aggressive	|	Brute-force search of every plugin	|	https://youtu.be/Alx5KQWq7ZM	|
|	ffuf -u **url** -H "Host: FUZZ.**domain.local**" -w /usr/share/wordlists/SecLists/DNS/bitquark-subdomains-top100000.txt	|	Sub-Domain brute-force search	|	https://youtu.be/AJc53DUdt1M	|
|	***I NEED TO TRY THIS LATER TODAY*** gobuster dir --url **url** -w **wordlist** -d	|	Appends common backup extentions to the wordlist entries	|	https://youtu.be/p8mIdm93mfw <br /> https://github.com/IppSec/gobuster <br /> https://youtu.be/JpzREo7XLOY?t=1447	|

<!-- 
|		|		|		|
|		|		|		|
-->
