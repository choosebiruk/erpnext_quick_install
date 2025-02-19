# Unattended Install Script for ERPNext
Unattended script for ERPNext installation (Supports Versions 13, 14 and 15).

This is a no-interactive script for installing ERPNext Versions 13, 14 and 15. You can set up either development or production with very minimal interaction.

# How To:
To use this script, follow these steps:

# Before Installation

Make sure you install git and the latest package versions by updating system packages if you are running this script on a fresh Ubuntu machine.

```
sudo apt install git
sudo apt update && sudo apt -y upgrade
```
and then reboot your machine 

# Installation:

1. Clone the Repo:
```
git clone https://github.com/choosebiruk/erpnext_quick_install.git
```
2. navigate to the folder:
```
cd erpnext_quick_install
```
3. Make the script executable
```
sudo chmod +x erpnext_install.sh
```
4. Run the script:
```
source erpnext_install.sh
```

# Install Apps:

1. Frappe Payments:
```
bench get-app payments
bench --site [Site] install-app payments
```
2. Frappe HR:
```
bench get-app hrms
bench --site [Site] install-app hrms
```
3. Frappe Non-Profit:
```
bench get-app non_profit
bench --site [Site] install-app non_profit
```

# Compatibility

Ubuntu 22.04 LTS,
Ubuntu 20.04 LTS

Debian 10 (Buster),
Debian 11 (Bulls Eye)

# NOTE:

Version 15 Compatibility is set to Ubuntu 22.04 LTS and above only. Other Distros or lower Ubuntu versions not supported for version 15 installation.
Visit https://github.com/gavindsouza/awesome-frappe to learn about other apps you can install.

Wherever your see [Site] replace it with your actual site.

