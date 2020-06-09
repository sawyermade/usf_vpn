# USF VPN Setup

## Ubuntu 18.04 / 20.04 LTS x64 Install
```bash
# Clone repo and enter director
git clone https://github.com/sawyermade/usf_vpn
cd usf_vpn

# Install package
sudo dpkg -i linux/GlobalProtect_deb-5.1.1.0-17.deb && sudo apt install -f -y

# Initialize portal, should have connection error
globalprotect connect --portal vpn.usf.edu

# Enter credentials, netid & password then it connects
globalprotect

# After connecting, youll see >> where you type quit
quit

# Disconnect
globalprotect disconnect 

# Reconnect, shouldnt ask for credentials
globalprotect connect
```

## Certificate Error Fix Ubuntu
```bash
# Remove .GlobalProtect
rm -rf ~/.GlobalProtect

# Connect
globalprotect connect
```

## Aliases
```bash
alias vu='globalprotect connect'
alias vd='globalprotect disconnect'
alias vs='globalprotect status'
```
