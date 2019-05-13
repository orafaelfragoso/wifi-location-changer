# Mac OSX Wi-Fi Location Changer
> Automatic wi-fi changer

## Installation

### Automated Installation

Execute:
```bash
./install.sh
```

### Manual Installation

Copy these files:
```bash
cp locationchanger /usr/local/bin
cp LocationChanger.plist ~/Library/LaunchAgents/
```
Should you place the locationchanger script to another location, make sure you edit the path in LocationChanger.plist too.

Make locationchanger script executable:
```bash
chmod +x /usr/local/bin/locationchanger
```
Load LocationChanger.plist as a launchd daemon:
```bash
launchctl load ~/Library/LaunchAgents/LocationChanger.plist
```
