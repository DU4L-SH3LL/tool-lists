# Tool List

Here you can find some useful tools to solve a CTF. Feel free to add some tools!

## Categories

1. [Forensic](#forensic)
2. [Misc](#misc)
3. [Crypto](#crypto)
4. [Reverse](#reverse)
5. [OSINT](#osint)


## Forensic

### Binwalk

Binwalk is a tool for searching binary files like images and audio files for embedded files and data.

<details><summary><b>Usefull commands</b></summary>
    ```sh
    binwalk file        Displays the embedded data in the given file 
    binwalk -e file     Displays and extracts the data from the given file
    ```
</details>

### Exiftool

Sometimes important stuff is hidden in the metadata of the image or the file , exiftool can be very helpful to view the metadata of the files.

<details><summary><b>Usefull commands</b></summary>
    ```sh
    exiftool "file"     shows the metadata of the given file
    ```
</details>

## Misc

## Crypto

Whatever happen, google is your friend. There are a lot cryptography tools online. Some of good tool are made offline like OpenSSL.



<details><summary><b>Classic cipher / Simple decoder online tool:</b></summary>
- hallo
- welt
</details>



<details><summary><b>Modern cryptography:</b></summary>
- https://gchq.github.io/CyberChef/ - All in one tool
- https://crackstation.net/ - Crack hash
- Cryptool
- John the Ripper 
- Hashcat

Cracking compressed file:
- John the Ripper
    ```sh
    john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt
    ```
- fcrackzip 
    ```sh
    fcrackzip -D -u -p rockyou.txt  filename.zip
    ```
- Hashcat 
    
</details>

## Reverse

### [Ghidra](https://ghidra-sre.org/)

Ghidra is a Software Reverse Engineering (SER) Framework developed by the NSA. Features include a disassembler (binary data -> ASM), decompiler (ASM -> C), a debugger (with GDB) and a scripting interface.

### [GDB](https://www.gnu.org/software/gdb/download/)

The Gnu-Debugger is a debugger for Linux, allowing you to examine the program at runtime. With [GEF](https://github.com/hugsy/gef) (GDB Enhanced Features) you get a nicer output and easier command syntax.

### [x64dbg](https://x64dbg.com/)

A (spiritual) successor to the classic OllyDbg, allowing you to debug x86/x64 binaries on windows.

### [pwntools](https://github.com/Gallopsled/pwntools)

A very useful python package which makes exploit development quick and easy for CTFs.

### [radare2](https://github.com/radareorg/radare2)

A unix x86/x64 disassembler

### [ApkTool](https://ibotpeaches.github.io/Apktool/)

A tool for Android reverse engineering, can decompile an .apk file.


### [Fiddler](https://www.telerik.com/fiddler)

A network proxy allowing you to intercept HTTP(S) traffic and read it. This can be useful if you want to find out what API an Android App talks to, simply point your Android proxy to Fiddler and you will see all the traffic.

### [Detect It Easy](https://github.com/horsicq/Detect-It-Easy)

A tool which helps you identify data about an executable, e.g. tools used for obfuscation and compiler and linker data.


## OSINT

## Exploit

- Burp Suite: https://portswigger.net/burp
- Nmap: https://nmap.org/
- Gobuster: https://github.com/OJ/gobuster
- Exploit-db: https://www.exploit-db.com/
- Metasploit: https://www.metasploit.com/
- Hydra: https://github.com/vanhauser-thc/thc-hydra
- Zed Attack Proxy: https://www.zaproxy.org/
