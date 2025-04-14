# IP Changer by Hanan Asif

A simple and efficient tool to automatically change your IP address using Tor network at regular intervals.

![Screenshot 2025-04-14 051457](https://github.com/user-attachments/assets/52744188-cefb-43cc-8ec0-8fa256994766)

## Features

- 🔄 Automatic IP rotation at user-defined intervals
- 🛡️ Uses Tor network for secure IP changes
- 🚀 Works on multiple Linux distributions
- ⚡ Easy installation and setup
- ⌛️ Run without installation

## Supported Distributions

- Arch Linux / Manjaro
- Debian / Ubuntu
- Kali Linux
- Parrot OS
- Fedora
- OpenSUSE

## Prerequisites

- Linux-based operating system
- Sudo privileges
- Internet connection
- tor,curl,xxd,fq packages required

## Run without Installation
1. Clone the repository:
```bash
git clone https://github.com/thehananasif/ip-changer.git
cd ip-changer
```

2. Make the installation script executable:
```bash
chmod +x ip-changer.sh
```

3. Run the installation script:
```bash
sudo ./ip-changer.sh
```

4. Follow the on-screen instructions to set your desired IP change interval.
## Setup for service

1. Clone the repository:
```bash
git clone https://github.com/thehananasif/ip-changer.git
cd ip-changer
```

2. Make the installation script executable:
```bash
chmod +x setup.sh
```

3. Run the installation script:
```bash
./setup.sh
```

4. Follow the on-screen instructions to set your desired IP change interval.

## Usage

Once installed, the service will automatically start and run in the background. Your IP address will be changed at the interval you specified during installation.

### Checking Status

To check if the service is running:
```bash
systemctl status change-tor-ip.service
```

### Stopping the Service

To stop the IP changer:
```bash
sudo systemctl stop change-tor-ip.service
```

### Starting the Service

To start the IP changer:
```bash
sudo systemctl start change-tor-ip.service
```

### Changing the Interval

To change the IP rotation interval:
1. Stop the service
2. Edit the `change-tor-ip.service` file
3. Restart the service

## Uninstallation

To remove the IP Changer:
```bash
sudo systemctl stop change-tor-ip.service
sudo systemctl disable change-tor-ip.service
sudo systemctl stop tor
sudo systemctl disable tor
sudo rm /etc/systemd/system/change-tor-ip.service
sudo rm /home/$USER/change_tor_ip.sh
```

## Security Note

This tool uses the Tor network to change your IP address. While Tor provides anonymity, please be aware that:
- Some websites may block Tor exit nodes
- Your connection speed may be affected
- Always use HTTPS connections for sensitive data

## License

This project is licensed under the MIT License.

### For More Video subcribe <a href="http://youtube.com/HoloXinMarketing">TechChip YouTube Channel</a>
