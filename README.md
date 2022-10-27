# WIFI-SNIFF-PUBLIC

To sniff a wifi network and if it is a public network everything will be open so it is possible to retrieve information.

First do:

airmon-ng to choose the interface, example airmon-ng start (interface)

so you have your monitor interface which gives wlan0mon

do an airodump-ng wlan0mon to have the wifi network nearby, to have the bssid and the chanel.

the bssid found and the chanel do this command without forgetting to capture the packets, example:

airodump-ng wlan0mon --bssid xx:xx:xx:xx:xx:xx -c (chanel) -w /root/dump.cap
