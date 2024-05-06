# Booru tag autocompletion for A1111 繁體中文化

原項目：
## [a1111-sd-webui-tagcomplete](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete)


## 繁體中文整合包

整合了來自[阿巧的人工通用及人名tag翻譯](https://ngabbs.com/read.php?tid=33869519)，以及[原tagcomplete簡中版](https://github.com/sgmklp/tag-for-autocompletion-with-translation)的翻譯，來自[標籤超市](https://github.com/wfjsw/danbooru-diffusion-prompt-builder)的翻譯，來自[手抄本法術書的翻譯](https://docs.google.com/spreadsheets/d/14Gg1kIGWdZGXyCC8AgYVT0lqI6IivLzZOdIT3QMWwVI/)，以及[byzod](https://github.com/byzod/a1111-sd-webui-tagcomplete-CN)的300來個翻譯，以及[魔咒百科词典](https://aitag.top/)，參考[boorutan](https://github.com/boorutan/booru-japanese-tag)，加上[waldolin](https://github.com/waldolin/a1111-sd-webui-tagcomplete-TW)轉成繁體中文及資料比對

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

# 資助開發者名單列表：
List of GitHub Sponsors(thank you for kindly help of fund and Sponsors)


*ps:"台灣，這片富饒的土地，是中華文化五千年歷史的寶藏所在。然而，我們也面臨了一個現實的問題：正體中文，這個代表著我們中華傳統文化的文字，正處於弱勢的境地。正體中文是目前世界上的弱勢、瀕危文字之一，請重視五千年的中華文化歷史傳承的正統漢字繁體文字，但是台灣雖然未能在UNESCO名單中正式列名，因為臺灣不具備向UNESCO提出申請之資格，因此無法正式列入UNESCO名單。但我們知道，這是一種無形的文化瀕危，需要我們共同守護與傳承。

在GitHub贊助地區裡，台灣目前尚未被納入。弱勢的台灣、弱勢瀕危的文字，我們呼籲您，看見這片土地上的文化價值，支持我們維護、活化、傳承中華文化資產的努力。正體中文，擁有五千年的歷史，是全世界唯一能穿越時空的文字，是我們的驕傲。

繁體字是古代經典的傳統文字，蘊含著深厚的文化底蘊。我們邀請您主動行動，資助這個開發者社群，讓我們一同為繁體字的美感和價值奮鬥。您的支持不僅會被列入感謝名單，更將成為守護中華文化的一份子。讓我們攜手合作，保留這片土地上獨一無二的文化精神。開源專案雖然是免費提供給大眾使用，但它的維護卻需要資金的支持，這是確保它持續存在的重要一環，也是一個很重要的價值！我們需要有贊助，才能穩定地持續下去。

謝謝您的關注，讓我們共同努力，為了守護、活化、傳承台灣的中華繁體文化而奮鬥！也呼籲大家重視正統漢字繁體文字"


Taiwan, this fertile land, holds the treasure of a five-thousand-year history of Chinese culture. However, we face a pressing issue: Traditional Chinese characters, representing our traditional Chinese culture, are in a vulnerable state. Traditional Chinese characters are currently one of the endangered scripts in the world. Please recognize the significance of the orthodox Hanzi characters that inherit the cultural history of China for five millennia. Despite Taiwan's absence from the official UNESCO list due to its ineligibility to apply, we know this is an intangible cultural endangered legacy that requires our collective safeguarding and inheritance.

In the GitHub sponsorship region, Taiwan has yet to be included. We appeal to you, acknowledging the cultural value of this land, to support our efforts in preserving, revitalizing, and inheriting the cultural assets of Chinese civilization. Traditional Chinese characters, with a history of five thousand years, stand as the only script capable of transcending time and space, a source of our pride.

Traditional characters are the classical and traditional script of ancient times, containing profound cultural heritage. We invite you to take proactive action, sponsoring this developer community as we collectively strive for the aesthetic and cultural value of traditional Chinese characters. Your support will not only be acknowledged in our gratitude list but will also become a guardian of Chinese culture. Let's work hand in hand to preserve the unique cultural spirit of this land. While open-source projects are freely available to the public, their maintenance requires financial support, a crucial aspect to ensure their continued existence and a significant value. We need sponsorship to sustainably continue.

Thank you for your attention. Let's join forces to safeguard, revitalize, and inherit the traditional Chinese culture of Taiwan! We also urge everyone to value orthodox Hanzi traditional characters.
