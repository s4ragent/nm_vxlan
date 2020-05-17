# nm_vxlan

sudo nmcli connection add type vxlan id 10 con-name vxlan0 ifname vxlan0 dev eth0 remote 127.0.0.1 ip4 192.168.0.11/24

git clone https://github.com/s4ragent/nm_vxlan

cd nm_vxlan
sudo cp 09_vxlan /etc/NetworkManager/dispatcher.d/09_vxlan

sudo chmod +x /etc/NetworkManager/dispatcher.d/09_vxlan


sudo nmcli con up vxlan0



