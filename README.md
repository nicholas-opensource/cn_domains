# cn_domains
List of Chinese domains

* Bilibili
* Netease Music
* Tencent Video
* iQiYi Video

* Updating...

For SSRP users:
```
cat > /etc/ssrplus/gfw_base.conf <<EOF
ipset=/baidu.com/gfwlist
server=/baidu.com/127.0.0.1#5335
EOF
uci set shadowsocksr.@global[0].gfwlist_url='https://raw.githubusercontent.com/nicholas-opensource/cn_domains/main/list.txt'
uci commit shadowsocksr
/etc/init.d/shadowsocksr restart
```
