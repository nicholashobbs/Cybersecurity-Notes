# Cybersecurity Notes

## Conventions

This file should be built as follows - start hard and jump to easy, but also cover things progressively as you go. Start with a high level description of what something is, then move on to more detail as you go. First create a complete listing of the things which you now know and want to learn before the end of class, and then transform it into a complete lesson plan whereby students are initially introduced to everything and told the capabilities of different tools - as time goes by they will be introduced and gradually exposed to the deeper levels of these tools.

`[]` - refers to something that should be replaced by any user-specified value
`<>` - contains a list of possible options, such as flags 

## General Linux

### Basic Commands

`pwd` - print working directory (where are you in the filesystem)
`sudo` - do this action as the root user - use `sudo -i` to change your identity to sudo
`[command] !!` - prepend command to prior command - useful when you forget to `sudo` previous command with `sudo !!`
`cd [directory]` -  move to directory
`ls <-la>` - list files in current directory. Option l is for a 'long' listing, which shows permissions and other details, a shows all files, including those which begin with . which are usually hidden.
`Tab` - use tab-completion to complete a name based on what you have typed so far. If there are more than one option, tab twice to list available options
`ln /file/path /link/path` - creates a hard link from file path to link path
`mkdir [directory]` - create directory - `rmdir` to remove
`rm` - remove a file
`mv /file /here` - moves file to here. I must be missing something because it never seems to work properly for me
`cp /this/file /to/here` - copy this file to here
`touch file` - create file
`man program` - shows the manual for program
`head file` - shows the first 10 lines of a file
`tail` - shows the last 10 lines of a file
`echo text` - prints text to terminal
`chmod ###` - change permissions where #1 refers to owner, #2 refers to user's group, #3 refers to everyone, and possible values range from 0-7. Read permissions are 4, write permissions are 2, execute permissions are 1. Can be written as 7=rwx, 6=rw-, 5=r-x, 4=r--, 3=-wx, 2=-w-, 1=--x, 0=---.
`[user] passwd` - change user's password
`useradd` - create a user - `userdel` to delete
`top` - shows what processes are running and other details
`this | that` - 'pipes' the output from this into the command that
`>` - same as pipe??
`this >> file` - appends this to file 
`<` - backwards pipe??
`1>` - redirects STDIN
`2>` - redirects STDOUT
`0>` - redirects STDERR
`this && that` does that iff this completes succesfully
`this || that` does this or that
`wc <-l>` - gives a word count, where the option l counts lines
`ip` - contains a variety of tools for information about internet connection - link for setting up/down interfaces, addr for displaying current setup, etc
`find / -name this` - a basic tool for finding things in linux file system, this syntax finds a file called name. Other options include `-wholename`, which searches for directories in addition to files themselves
`grep` - a much more powerful tool for searching - option -r allows you to recursively search a directory for files containing a string
`awk` - another utility for finding things in linux which in its simples form can print something , e.g. `awk {print} /this/file` prints this file, `awk /match/ /in/here prints lines with match in here, `/^match/` prints lines which begin with match
`sed` - allows you to modify a file from command line automatically - more on this later
`kill process` - a utility for killing processes which are running - priority can be set with numbers - e.g. `kill 9 process` is the most harsh version which kills the process no matter what
`sort` - sorts things by lines or other ways depending on options
`less` - allows you to scroll through output longer than the screen - often used as `do this | less` so you can read all the output created by do this
`cat file` - outputs the contents from file
`clear` - clears the terminal so you can start at the top again rather than continually being pushed to the bottom
`history` - shows you the last 500 commands you have done - you can set this to more by:


### Hotkeys

`CTRL+A` - jump to beginning of line
`CTRL+E` - jump to the end of the line
`CTRL+L` - same as `clear`, etc`

### Filesystem

### vim



### Searching

### Hard Drive Utilities and Partitioning

### Compiling and Installing

### Updates

### Backups

### SSH Plans

### Networking Tools

#### TCP/IP

#### Physical Networking

#### IP Routing

#### DNS

#### SSO

#### Email

#### Web Hosting

#### Cloud Computing

#### Security

#### Performance Analysis

#### Monitoring

#### Virtualization

### tmux

Ctrl + b +

	% vertical " horizontal split
	o switch pane
	x kill pane
	+ make pane into window	
	Hold Ctrl + b + [arrow key] to resize pane

	c create window
	, name window
	& kill window
	[#] switch to window #

## Pentesting Tools

### nmap

nmap [flags] filename ip.ad.dre.ss:port

## Kali

### Recon-ng 

### Shodan

### Dmitry, Sparta, Netdiscover, Zenmap

### Metasploit

### Meterpreter

### AV Bypass

### Privelege Escalation

### Packet Capture

### MITM

### Social Engineering

### BeEF

### Password Cracking

### Wireless Network Attacks

### Mutillidae

### Maintaining Access

### Post Exploitation

### Payloads

## Web App Hacking

### OWASP Top 10

### OTGv4

### Info Gathering

### Mapping Application 

### Organization Tools and Techniques

### Types of Attack

#### Open Redirect

#### HTTP Parameter Pollution

#### Cross Site Request Forgery

#### HTML Injection

#### CRLF Injection

#### XSS

#### Template Injection

#### SQLi

#### SSRF

#### XXE

#### Remote Code Execution

#### Buffer Overflow

#### Subdomain Takeover

#### Race Conditions

#### IDOR

#### OAuth

#### Application Logic Vulnerabilities

## Security+

### Security Basics

### Identity and Access Management

### Networking

### Securing Networks

### Securing Hosts and Data

### Threats and Vulnerabilities

### Advanced Attacks

### Risk Management

### Controls to Protect Assets

### Cryptography and PKI

### Policies

## Map of Bug Bounty Methodology

## Web Architecture Section

## Ippsec Notes

## Next Steps

### Automation

### Machine Learning Applications

