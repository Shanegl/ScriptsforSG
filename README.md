# ScriptsforSG
##This script is not for sharing.

hosts部分自行添加。
```
RUL-SET,https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Rule-Sets/ADs-Block.rulesets?token=AB7NJ4HQ3X55SXICDKH5SGK6RV7D4,reject
```
京东去广告、Banner
```
http-response ^https?://api\.m\.jd\.com/client\.action\?functionId=(start|myOrderInfo|orderTrackBusiness) requires-body=1,max-size=-1,script-path=https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Scripts/JDAdRemove.js?token=AB7NJ4C2KBFOWKTDQXKTLPC6RV7HK
```
什么值得买去广告
```
http-response ^https?:\/\/(h(aojia|omepage)|(articl|baik)e|s)-api\.smzdm\.com\/(home|sou) requires-body=1,max-size=-1,script-path=https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Scripts/SMZDM.js?token=AB7NJ4GAXZMF67ZIBOH35726RV7SM
```
B站App去广告整合（N脚本合一）
```
http-response ^https?:\/\/ap(i|p).(live.)?bilibili.com\/x(live)?\/(resource\/show\/tab|v2\/(reply\/main|view\/material|account\/(mine|teenagers\/status)|view|feed\/index|show\/popular\/index|rank)|app-room/v1/index/getInfoByRoom)\?access_key requires-body=1,max-size=-1,script-path=https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Scripts/Bilibili.js?token=AB7NJ4A5C3T7AS7BFINLSB26RV764
```
知乎去广告整合（N脚本合一）
```
http-response ^https?:\/\/(api|www)\.zhihu\.com\/(moments(\/recommend)?\?(action|feed_type)|topstory\/recommend|.*\/questions|market\/header|people|appview\/(v2|p)\/(answer\/)?\d{1,10}\?no\_image\=false(\&article\_fixed\_bottom\=1)?\&X\-SUGER\=) requires-body=1,max-size=-1,script-path=https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Scripts/Zhihu.js?token=AB7NJ4BK456JQ6PKUTOL6I26RV73A
```
丁香园用药助手解锁订阅（非医务工作者无需此App）
```
http-response ^https?:\/\/newdrugs\.dxy\.cn\/app\/user\/(p(ay\/checkIntroOfferPeriod|ro\/stat)|init)\? requires-body=1,script-path=https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Scripts/DingXiangDrugs.js?token=AB7NJ4H3CY3XEUYVIN6L4LK6RV7P4
```
Lightroom解锁订阅（越南大佬）
```
http-response ^https:\/\/photos\.adobe\.io\/v2\/accounts requires-body=1,script-path=https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Scripts/Lightroom.js?token=AB7NJ4C6YFK2BQLWAAORHJC6RV7KI
```
Photoshop解锁订阅（越南大佬）
```
http-response ^https://lcs-mobile-cops.adobe.io/mobile_profile/nul/v1 requires-body=1,script-path=https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Scripts/Photoshop.js?token=AB7NJ4CL7I5TTZXG4LTMUZK6RV7N6
```
淘宝历史价格，二合一修正（yichahucha）
```
http-response ^https?://(amdc|trade-acs)\.m\.taobao\.com/(amdc/mobileDispatch|gw/mtop\.taobao\.detail\.getdetail) requires-body=1,script-path=https://raw.githubusercontent.com/Shanegl/ScriptsforSG/master/Scripts/TaobaoPrice.js?token=AB7NJ4ARKBVRFCED7LCF4JC6RV7WI
```
