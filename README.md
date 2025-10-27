ifconfig -a
rpm -i +tên gói cài đặt
nano /etc/xinetd.d/telnet



systemctl start xrdp
netstat -antup | grep xrdp 
systemctl enable xrdp
- firewall-cmd --permanent --add-port=3389/tcp
- firewall-cmd --reload
 chcon --type=bin_t /usr/sbin/xrdp
chcon --type=bin_t /usr/sbin/xrdp-sesman
netstat -antup | grep xrdp
systemctl restart xrdp
 netstat -antup | grep xrdp
