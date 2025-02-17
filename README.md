# SUID3NUM
[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)
[![python](https://img.shields.io/badge/python-2.7-blue.svg)](https://www.python.org/downloads/)
[![python](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/)
[![Open Source Love](https://badges.frapsoft.com/os/mit/mit.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)

**A standalone python script which utilizes python's built-in modules to find SUID bins, separate default bins from custom bins, cross-match those with bins in GTFO Bin's repository & auto-exploit those, all with colors! ( ͡ʘ ͜ʖ ͡ʘ)**

[![asciicast](https://asciinema.org/a/273928.svg)](https://asciinema.org/a/273928)

### Description
A standalone script supporting both python2 & python3 to find out all SUID binaries in machines/CTFs and do the following
- List all Default SUID Binaries (which ship with linux/aren't exploitable)
- List all Custom Binaries (which don't ship with packages/vanilla installation)
- List all custom binaries found in GTFO Bin's (This is where things get interesting)
- Try and exploit found custom SUID binaries which won't impact machine's files

Why This? 
- Because LinEnum and other enumeration scripts only print SUID binaries & GTFO Binaries, they don't seperate default from custom, which leads to severe head banging in walls for 3-4 hours when you can't escalate privs :) 

### Output
<a href="https://github.com/Anon-Exploiter/SUID3NUM/blob/master/output.m" target="_blank">SUID 3NUM's Sample Output</a>

### Works on 

- Python (2.6-7.*)
- Python (3.6-7.*)

### Download & Use

	wget https://raw.githubusercontent.com/Anon-Exploiter/SUID3NUM/master/suid3num.py --no-check-certificate && chmod 777 suid3num.py
	curl -k https://raw.githubusercontent.com/Anon-Exploiter/SUID3NUM/master/suid3num.py --output suid3num.py && chmod 777 suid3num.py
	
### Tested on

- Pop! OS 18.04 LTS
- Ubuntu 18.04 LTS
- Nebula
- Kali Linux (PWK VM)
 
### Usage

***Initializing Script***

	python suid3num.py

***Doing Auto Exploitation of found custom SUID binaries***

	python suid3num.py -e

### Output

<img src="https://i.imgur.com/FME2USf.gif" />

### Auto Exploitation of SUID Bins

[![asciicast](https://asciinema.org/a/273929.svg)](https://asciinema.org/a/273929)

### Note 
<pre><code>Please run the script after going through what it does & with prior knowledge of SUID bins.
P.S ~ Don't run with `-e` parameter, if you don't know what you're doing!
</code></pre>

### Thanks
<code>
Shoutout to Zeeshan Sahi & Bilal Rizwan for their ideas and contribution. 

Also, thanks to [Cyrus](https://github.com/cyrus-and) for [GTFO Bins](https://gtfobins.github.io/) <3 </code>

<code>
Let me know, what you think of this script at [@syed__umar](https://twitter.com/@syed__umar) ≧◡≦
</code>
