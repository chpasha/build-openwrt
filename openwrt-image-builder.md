## Cudi WR3000s ##
### master 24.10.5

`
base-files ca-bundle dnsmasq dropbear firewall4 fitblk fstools kmod-crypto-hw-safexcel kmod-gpio-button-hotplug kmod-leds-gpio kmod-nft-offload kmod-phy-aquantia libc libgcc libustream-mbedtls logd
mtd netifd nftables odhcp6c odhcpd-ipv6only opkg ppp ppp-mod-pppoe procd-ujail uboot-envtools uci uclient-fetch urandom-seed urngd 
-wpad-basic-mbedtls kmod-mt7915e kmod-mt7981-firmware mt7981-wo-firmware luci luci-app-attendedsysupgrade
mc iperf3 libiperf3 bind-dig curl jq
wireguard-tools kmod-wireguard luci-proto-wireguard
luci-proto-openfortivpn openfortivpn
ddns-scripts ca-certificates luci-app-ddns qrencode
wpad-mbedtls dawn luci-app-dawn fping kmod-batman-adv luci-proto-batman-adv batctl-full
`

## Cudi WR3000e ##
### Dump AP 24.10.5 ###

`
base-files ca-bundle dnsmasq dropbear firewall4 fitblk fstools kmod-crypto-hw-safexcel kmod-gpio-button-hotplug kmod-leds-gpio kmod-nft-offload kmod-phy-aquantia libc libgcc libustream-mbedtls logd
mtd netifd -nftables -odhcp6c -odhcpd-ipv6only opkg -ppp -ppp-mod-pppoe procd-ujail uboot-envtools uci uclient-fetch urandom-seed urngd 
-wpad-basic-mbedtls wpad-mbedtls kmod-mt7915e kmod-mt7981-firmware mt7981-wo-firmware luci luci-app-attendedsysupgrade
mc iperf3 libiperf3 curl dawn luci-app-dawn kmod-batman-adv luci-proto-batman-adv
`
 
## Cudi TR1200 ##
### master 24.10.5 mit LTE Support

`
base-files ca-bundle dnsmasq dropbear firewall4 fstools kmod-gpio-button-hotplug kmod-leds-gpio kmod-mt7603 kmod-nft-offload libc 
libgcc libustream-mbedtls logd mtd netifd nftables odhcp6c odhcpd-ipv6only opkg ppp ppp-mod-pppoe swconfig uci uclient-fetch 
urandom-seed urngd -wpad-basic-mbedtls kmod-usb2 kmod-usb-ohci kmod-usb-ledtrig-usbport kmod-mt7615e kmod-mt7663-firmware-ap luci luci-app-attendedsysupgrade
wpad-mbedtls dawn luci-app-dawn bind-dig kmod-batman-adv luci-proto-batman-adv
wireguard-tools kmod-wireguard luci-proto-wireguard
usb-modeswitch kmod-usb-net kmod-usb-net-cdc-ether
`

## Archer C7 v2 ##

### dump-ap 24.10.5 ### 

`
base-files ca-bundle dnsmasq dropbear firewall4 fstools kmod-ath9k kmod-gpio-button-hotplug kmod-nft-offload libc libgcc
libustream-mbedtls logd mtd netifd nftables odhcp6c odhcpd-ipv6only opkg -ppp -ppp-mod-pppoe procd-ujail swconfig
uboot-envtools uci uclient-fetch urandom-seed urngd -wpad-basic-mbedtls kmod-usb2 kmod-usb-ledtrig-usbport
kmod-ath10k ath10k-firmware-qca988x luci mc wpad-mbedtls dawn luci-app-dawn fping kmod-batman-adv luci-proto-batman-adv`


###  master 24.10.5: ###
`
base-files ca-bundle dnsmasq dropbear firewall4 fstools kmod-ath9k kmod-gpio-button-hotplug kmod-nft-offload libc 
libgcc libustream-mbedtls logd mtd netifd nftables odhcp6c odhcpd-ipv6only opkg ppp ppp-mod-pppoe procd-ujail swconfig 
uboot-envtools uci uclient-fetch urandom-seed urngd wpad-mbedtls kmod-usb2 kmod-usb-ledtrig-usbport 
kmod-ath10k ath10k-firmware-qca988x luci luci-app-attendedsysupgrade mc wireguard-tools kmod-wireguard luci-proto-wireguard ddns-scripts
ca-certificates luci-app-ddns qrencode dawn luci-app-dawn bind-dig curl jq fping batctl-full kmod-batman-adv luci-proto-batman-adv
usb-modeswitch kmod-usb-net kmod-usb-net-cdc-ether luci-proto-openfortivpn openfortivpn
`

###  master 25.10.0: ###
`
apk-mbedtls base-files ca-bundle dnsmasq dropbear firewall4 fstools kmod-ath9k kmod-gpio-button-hotplug kmod-nft-offload libc libgcc libustream-mbedtls 
logd mtd netifd nftables odhcp6c odhcpd-ipv6only ppp ppp-mod-pppoe procd-ujail swconfig uboot-envtools uci uclient-fetch urandom-seed urngd 
-wpad-basic-mbedtls kmod-usb2 kmod-usb-ledtrig-usbport kmod-ath10k-ct ath10k-firmware-qca988x-ct luci luci-app-attendedsysupgrade
mc wireguard-tools kmod-wireguard luci-proto-wireguard ddns-scripts
ca-certificates luci-app-ddns qrencode dawn luci-app-dawn bind-dig curl jq fping batctl-full kmod-batman-adv luci-proto-batman-adv
usb-modeswitch kmod-usb-net kmod-usb-net-cdc-ether luci-proto-openfortivpn openfortivpn
`

## Archer C60 v2 ##

### dump-ap with batman 24.10.3 ### ohne mc da kein Platz

#### (Achtung: mit non -ct Version von ath10k hängt sich Router mit Wifi-5 auf)
`
base-files ca-bundle -dnsmasq dropbear -firewall4 fstools kmod-ath9k kmod-gpio-button-hotplug kmod-nft-offload libc libgcc
libustream-mbedtls logd mtd netifd nftables -odhcp6c -odhcpd-ipv6only opkg -ppp -ppp-mod-pppoe procd-ujail swconfig
uboot-envtools uci uclient-fetch urandom-seed urngd -wpad-basic-mbedtls
kmod-ath10k-ct-smallbuffers ath10k-firmware-qca9888-ct luci wpad-mbedtls dawn luci-app-dawn kmod-batman-adv luci-proto-batman-adv
`
 
#### Script to run on first boot to enable 5Ghz

`
sed -i 's/\tdlink,dir-842-c3)/\tdlink,dir-842-c3\|\\\n\ttplink,archer-c60-v2)/' /etc/hotplug.d/firmware/11-ath10k-caldata
`
                         

## Archer C60 v2 with batman 25.12.0 ###
### Achtung, sehr wenig Platz, nur nötigste, ohne 2.4GHz (mit großen Image wird rootfs als temp ge-mounted, Einstellungen gehen verloren. Bug? mit df -h prüfen)
`
/dev/mtdblock6 448.0K 232.0K 216.0K 52% /overlay
overlayfs:/overlay 448.0K 232.0K 216.0K 52% /
`

`
apk-mbedtls base-files ca-bundle dropbear fstools libc libgcc libustream-mbedtls logd mtd netifd procd-ujail swconfig uboot-envtools uci 
uclient-fetch urandom-seed urngd wpad-mesh-mbedtls kmod-ath10k-ct-smallbuffers ath10k-firmware-qca9888-ct ipq-wifi-tplink_archer-c60-v2 
luci kmod-batman-adv luci-proto-batman-adv dawn luci-app-attendedsysupgrade
`

## Archer C58 ##

### dump-ap 23.05.06 ###

`
base-files busybox ca-bundle -dnsmasq dropbear -firewall4 fstools kmod-ath9k kmod-gpio-button-hotplug kmod-nft-offload libc libgcc 
libustream-mbedtls logd mtd netifd nftables -odhcp6c -odhcpd-ipv6only opkg -ppp -ppp-mod-pppoe procd procd-seccomp procd-ujail swconfig 
uboot-envtools uci uclient-fetch urandom-seed urngd wpad-mbedtls kmod-ath10k-ct-smallbuffers ath10k-firmware-qca9888-ct luci dawn luci-app-dawn
kmod-batman-adv luci-proto-batman-adv batctl-full
`

### dump-ap 24.10.4 ###

`
base-files busybox ca-bundle -dnsmasq dropbear -firewall4 fstools kmod-ath9k kmod-gpio-button-hotplug kmod-nft-offload libc libgcc 
libustream-mbedtls logd mtd netifd nftables -odhcp6c -odhcpd-ipv6only opkg -ppp -ppp-mod-pppoe procd procd-seccomp procd-ujail swconfig 
uboot-envtools uci uclient-fetch urandom-seed urngd wpad-mbedtls kmod-ath10k-ct-smallbuffers ath10k-firmware-qca9888-ct luci dawn luci-app-dawn 
kmod-batman-adv luci-proto-batman-adv batctl-full
`
