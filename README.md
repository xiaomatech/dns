# dns/dhcp/ntp配置

- 使用
```
  yum install -y dnsmasq ntp
  
  wget https://codeload.github.com/xiaomatech/dns/zip/master -O dns-master.zip
  
  unzip dns-master.zip
  
  #修改对应的dhcp.conf dns.conf
  
  #dns dhcp
  mv dns-master/dnsmasq.conf /etc/dnsmasq.conf
  mv dns-master/dhcp.conf /etc/dnsmasq.d/dhcp.conf
  mv dns-master/dhcp.conf /etc/dnsmasq.d/dns.conf
  mv dns-master/resolv.conf /etc/resolv.conf
  
  service dnsmasq restart
  
  #ntp
  mv dns-master/ntp.conf /etc/ntp.conf
  
  service ntpd restart
  
```


