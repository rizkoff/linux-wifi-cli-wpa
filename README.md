# linux-wifi-cli-wpa
HOWTO: linux (worked @paspbian) wifi cli wpa commands

https://askubuntu.com/questions/138472/how-do-i-connect-to-a-wpa-wifi-network-using-the-command-line

wpa_passphrase myrouter > wpa.conf

cat wpa.conf >> /etc/wpa_supplicant/wpa_supplicant.conf

wpa_supplicant -Dwext -iwlan0 -c/etc/wpa_supplicant/wpa_supplicant.conf

dhclient wlan0
