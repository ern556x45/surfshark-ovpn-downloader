### *Surfshark OpenVPN Automatic file updater*


Hello.

I have made an automatic script to void the issue of the same files being used all the time.

The script itself has comments under each command explaining why and how it works.

This is using the Shark-china one click download link. It should autodelete all files and replace them with new ones. It's a proxy site from Surfshark so it is owned and operated by them.

Renaming the unzip file is prone to producing errors so I would suggest keeping it like this and relying on the rm command to avoid bloating up the system.

To connect you will need to cd into the /etc/ovpn directory.

You can add automatic authentication to each of the downloaded OpenVPN files to connect quciker and with less hassle.

1. Simply head to /etc/openvpn/.
2. Create a new file called "auth.conf".
3. Add OpenVPN username and password in lines 1 and 2, they can be found on my.surfshark.comn or my.shark-china.com and heading to VPN > Manual connection > OpenVPN > Credentials.
4. Remove the "#" from line 23 or "sudo sed".
5. Next time your files are updated, the line to authenticate automatically will add itself.

Hope this helps! 
**S.B.**