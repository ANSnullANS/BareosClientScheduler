# BareosClientScheduler
Windows-Service that allows Client-Side scheduling of Bareos-Backups.

## Why?
Bareos is a great tool for structured backup, but the scheduler basically relies on the clients to be available at a given time.

To be able to handle Mobile-Devices and Roadwarriors whilst only taking backups when they are in-house, I've created this rather simple Windows-Service.

## How?
BareosClientScheduler will start together with Windows and run regular checks to see if a backup is needed (based on it's schedule) and doable (client connected to corporate LAN via destinct network-adapter).

### Service Configuration
All customizable settings are included in "config.json" in the Application-Folder.
