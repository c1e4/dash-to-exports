# dash-to-exports
Export files for Gnome extensions like Dash-to-Dock and Dash-to-Panel

It appears that 'dconf' is a wonderful tool, able to make backups and restore configs with a simple command!
Also made full backup of system settings, however I will not publish it here for obvious reasons, hehe.

Backup with: 
dconf dump /org/gnome/shell/extensions/dash-to-dock/ > dash-to-dock-settings.ini

Restore with:
dconf load /org/gnome/shell/extensions/dash-to-dock/ < dash-to-dock-settings.ini

To backup full system settings (including all the extensions, etc):
dconf dump / > dconf-system-settings-dump.ini
To restore: 
dconf load  / < dconf-system-settings-dump.ini
