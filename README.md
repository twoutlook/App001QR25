# App001QR25
## 需求說明
### 原作業模式
- 原作業以EXCEL檔案, 每個sheet 有50組
- 直接在EXCEL記錄scan的成品序號QR Code, 每25,使用internet 生成 QR Code獲得圖檔貼回EXCEL
- 重覆檢查僅限同一檔案的同一Sheet, 仍有部份檢查功能失效
- 每組以日期和其序號為標示, 大的QR Code 其內容為 25 個成品的序號, 每個成品序號為14碼
- 以A4列印,即在EXCEL按次序選10組,標籤紙已預裁,可單張撕下
- 成品以25個裝盒, 列印好的標籤, 以十盒為單位, 一一貼上

### 改進做法
- 改為局網網頁應用 WebApp
- scan的成品序號QR Code, 即可獲得大的QR Code
- 重覆檢查在DB層面進行, 可以涵蓋所有已完工和現在進行的成品序號
- 單組列印
- 單組貼到裝盒

## 程式開發

- bar code printer,ZEBRA ZT230, 以 USB 連在二廠辦公室PC,進門到底
- Kent 以 Bartender 打樣
- Mark 在上述基礎上,先以 .NET 6 MVC 打樣, http://192.168.150.250:8060/Home/QrSample
- 
