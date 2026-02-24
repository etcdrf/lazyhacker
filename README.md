# lazyhacker

Lazyhacker is a bash-based automation tool designed mainly for HackTheBox, handling all the boring introductory recon for you.  
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
- Creation of a directory with the box's name to save all the outputs
- Check for the requirements
- All scans run simultaneously to save time
- Detection of the redirect domain
- Update of the /etc/hosts with all the found domains after user confirmation

## Requirements
- [ffuf](https://github.com/ffuf/ffuf)
- [seclists](https://github.com/danielmiessler/SecLists)
- [jq](https://github.com/jqlang/jq)
