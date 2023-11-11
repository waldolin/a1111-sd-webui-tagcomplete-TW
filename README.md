# Booru tag autocompletion for A1111 繁體中文化

原項目：
## [a1111-sd-webui-tagcomplete](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete)


## 繁體中文整合包

整合了來自[阿巧的人工通用及人名tag翻譯](https://ngabbs.com/read.php?tid=33869519)，以及[原tagcomplete簡中版](https://github.com/sgmklp/tag-for-autocompletion-with-translation)的翻譯，來自[標籤超市](https://github.com/wfjsw/danbooru-diffusion-prompt-builder)的翻譯，來自[手抄本法術書的翻譯](https://docs.google.com/spreadsheets/d/14Gg1kIGWdZGXyCC8AgYVT0lqI6IivLzZOdIT3QMWwVI/)，以及[byzod](https://github.com/byzod/a1111-sd-webui-tagcomplete-CN)的300來個翻譯，加上[waldolin](https://github.com/waldolin/a1111-sd-webui-tagcomplete-TW)轉成繁體中文

其中來自`中文化danbooru-tag 人名.xlsx`的tag完全沒有翻譯，只是摘取了有中文和日文的部分塞進去（by_byzod)

因為 ~完全妹有翻譯~ 只做了微不足道的翻譯，和一些複製粘貼的工作，歡迎大佬完善


## 文件說明

文件|說明
---|---
Tags-zh-full-pack.csv  | 簡體翻譯檔，適用於[tagcomplete 1.11](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete/releases/tag/1.11.0)及之後的版本
Tags-tw-full-pack.csv  | 繁體翻譯檔，適用於[tagcomplete 1.11](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete/releases/tag/1.11.0)及之後的版本
config.json  | 可選配置檔，預設值與官方配置不同


## 安裝

1. 安裝Stable Diffusiond的extension [tagcomplete](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete#installation)
2. 將`Tags-tw-full-pack.csv`放到`<tag-autocomplete安裝目錄>\tags\`中
3. "您可以在下面找到它Settings > Tag autocomplete > Translation filename > Translation file uses old 3-column translation format instead of the new 2-column one。打開它後，第二列將在解析過程中不被使用並被跳過。選Tags-tw-full-pack.csv"
*ps你也可以在翻譯部分新增一個附加文件，該文件將用於翻譯標籤和別名，並且還可以透過翻譯進行搜尋。該檔案必須是格式為 的 .CSV <English tag/alias>,<Translation>。一些較舊的文件使用三列格式，這需要啟動相容性設定。
4. 可選方案：
    1. 將`config.json`放到`<tag-autocomplete安裝目錄>\tags\`中覆蓋對應檔
    2. 打開`<tag-autocomplete安裝目錄>\tags\config.json`，修改`"translationFile": "",`為`"translationFile": "Tags-tw-full-pack.csv"`
5. 根據[官方配置說明](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete#config)按照自己的喜好修改配置

#
喜歡可以訂閱跟分享旺哥的YouTube頻道，謝謝！  
歡迎訂閱+小鈴鐺，關注我的頻道ww00yy  
【YOUTUBE 頻道】:零之自由創作空間的頻道(https://www.youtube.com/channel/UCKcW62Ys6zRFp3syvkDYOlQ)  
【旺哥的Twitch】https://www.twitch.tv/a0980368677   
【旺哥的paypal】https://streamlabs.com/a0980368677/tip   
贊助連結：paypal: https://www.paypal.me/waldo870  
【line貼圖】https://store.line.me/stickershop/author/4127681/zh-Hant  
歡迎支持與贊助，謝謝  
ようこそサポートとスポンサー  
Welcome support and sponsorship  
Bienvenido apoyo y patrocinio  
Benvenuto supporto e sponsorizzazione  
आपका स्वागत है समर्थन और प्रायोजन
