# USF VPN SETUP JUNO PULSE

## Website
https://www.net.usf.edu/vpn/Linux/

## Ubuntu 18.04
```
# Clone repo
git clone https://github.com/sawyermade/usf_vpn.git

# Install Pulse and Deps
cd usf_vpn/
sudo dpkg -i ps-pulse-linux.deb
sudo bash /usr/local/pulse/PulseClient.sh install_dependency_packages
sudo bash /usr/local/pulse/PulseClient.sh
sudo apt install libwebkitgtk-1.0-0
```

## Run Pulse
```
1. Hit Super, type pulse, and hit enter.
2. Click the plus sign to add a connection
3. Enter "USF VPN" for the Name
4. Enter "https://vpn.usf.edu" for the URL
5. Click "Save"
5. Click Connect
```