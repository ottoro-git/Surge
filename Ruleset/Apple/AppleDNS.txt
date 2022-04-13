Apple DNS 通过收集 Apple 在全中国几乎所有省级行政区的 CDN IP 列表，解决 App Store / Mac App Store / iTunes Store / Apple Music / iBooks / TestFlight 在中国部分地区速度缓慢的问题。

ChinaNet：电信宽带专用
ChinaUnicom：联通宽带专用
auto(原 CMCC)：电信、联通、移动 三网通用

电信、联通宽带用户可以自行按照教程生成最适合自身网络环境的 CDN IP 列表，移动宽带用户或嫌麻烦的用户使用 auto 列表即可。

Apple DNS参考：

[Host]
// Apple DNS

// China Net (中国电信)
# API-1-ChinaNetCenter [ChinaNet] (Avg RTT: 9.772ms)
se.itunes.apple.com = 222.211.64.122
su.itunes.apple.com = 222.211.64.122
upp.itunes.apple.com = 222.211.64.122
play.itunes.apple.com = 222.211.64.122
client-api.itunes.apple.com = 222.211.64.122
# API-2-ChinaCache [ChinaNet] (Avg RTT: 15.339ms)
itunes.apple.com = 125.65.247.14
init.itunes.apple.com = 125.65.247.14
# API-HK-Akamai-1 [HongKong0] (Avg RTT: 52.706ms)
search.itunes.apple.com = 184.87.97.50
# API-HK-Akamai-2-AMRadio [HongKong1] (Avg RTT: 58.221ms)
radio.itunes.apple.com = 184.87.100.246
radio-activity.itunes.apple.com = 184.87.100.246
radio-services.itunes.apple.com = 184.87.100.246
# Apple Music Streaming [ChinaNet-ChinaCache] (Avg RTT: 10.465ms)
aod.itunes.apple.com = 139.206.198.9
mvod.itunes.apple.com = 139.206.198.9
streamingaudio.itunes.apple.com = 139.206.198.9
# Beats 1 Radio (Not Available in Mainland China) [Malaysia] (Avg RTT: 90.211ms)
itsliveradio.apple.com = 202.76.239.11

// China Unicom （中国联通）
# API-1-ChinaNetCenter [ChinaUnicom] (Avg RTT: 71.482ms)
se.itunes.apple.com = 123.138.61.6
su.itunes.apple.com = 123.138.61.6
upp.itunes.apple.com = 123.138.61.6
play.itunes.apple.com = 123.138.61.6
client-api.itunes.apple.com = 123.138.61.6
# API-2-ChinaCache [ChinaUnicom] (Avg RTT: 62.808ms)
itunes.apple.com = 60.6.197.202
init.itunes.apple.com = 60.6.197.202
# API-HK-Akamai-1 [HongKong0] (Avg RTT: 109.218ms)
search.itunes.apple.com = 23.42.189.88
# API-HK-Akamai-2-AMRadio [HongKong1] (Avg RTT: 192.861ms)
radio.itunes.apple.com = 23.13.185.169
radio-activity.itunes.apple.com = 23.13.185.169
radio-services.itunes.apple.com = 23.13.185.169
# Apple Music Streaming [ChinaUnicom-ChinaNetCenter] (Avg RTT: 27.633ms)
aod.itunes.apple.com = 113.207.6.58
mvod.itunes.apple.com = 113.207.6.58
streamingaudio.itunes.apple.com = 113.207.6.58
# Beats 1 Radio (Not Available in Mainland China) [Malaysia] (Avg RTT: 90.211ms)
itsliveradio.apple.com = 202.76.239.11

// Auto （三网通用）
aod.itunes.apple.com = hkg.aapldns.xyz
aodp.itunes.apple.com = hkg.aapldns.xyz
appldnld.apple.com = hkg.aapldns.xyz
iosapps.itunes.apple.com = hkg.aapldns.xyz
itsliveradio.apple.com = 42.99.128.168
osxapps.itunes.apple.com = hkg.aapldns.xyz
streamingaudio.itunes.apple.com = hkg.aapldns.xyz
swcdn.apple.com = hkg.aapldns.xyz
// aapldns.xyz 由 AppleDNS Team 托管，以 CNAME 的方式解析 Apple 服务器 IP
