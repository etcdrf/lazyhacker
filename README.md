# lazyhacker

Lazyhacker is a bash-based automation tool designed mainly for HackTheBox, handling all the boring introductory reconnaissance for you.  
Just launch the script, brew a coffee, and by the time you’re done, you’ll be ready to hack!

## Performed scans:
- Nmap TCP scan
- Nmap UDP scan
- Directory fuzzing
- Subdomain fuzzing
- Fuzz inside found directories
- Fuzz discovered subdomains

## Usage:
```
$ ./lazyhacker.sh [IP] [BoxName]
Example: ./lazyhacker.sh 10.10.11.221 TwoMillion
```
## Features
- Detection of the redirect domain
- Update of the /etc/hosts with the redirect domain
- Cross checks the subdomains with the user before inserting them into /etc/hosts

## Requirements
- [ffuf](https://github.com/ffuf/ffuf)
- [seclists](https://github.com/danielmiessler/SecLists)
- [jq](https://github.com/jqlang/jq)
