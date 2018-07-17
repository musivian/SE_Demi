# SoftEther

## Guide:

```cpp
chmod +x /etc/init.d/vpnserver
nano -w /etc/sysctl.conf

Change:
#net.ipv4.ip_forward=1
to
net.ipv4.ip_forward=1
CTRL + X then type Y then hit enter

echo 1 > /proc/sys/net/ipv4/ip_forward
sysctl --system

/etc/init.d/vpnserver restart
/usr/local/vpnserver/vpncmd
Type "1" and hit Enter three times

IPsecEnable
yes
no
yes
asiangamerz
AsianGamerz

ServerCertRegenerate <SERVER IP>
ServerCertGet ~/cert.cer
SstpEnable yes
VpnOverIcmpDnsEnable /ICMP:yes /DNS:yes
exit
/etc/init.d/vpnserver restart
```
