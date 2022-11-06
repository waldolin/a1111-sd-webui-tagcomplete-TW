# Booru tag autocompletion for A1111 简中

原项目：
## [a1111-sd-webui-tagcomplete](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete)


## 简中整合包

整合了来自[阿巧的人工通用及人名tag翻译](https://ngabbs.com/read.php?tid=33869519)，以及[原tagcomplete简中版](https://github.com/sgmklp/tag-for-autocompletion-with-translation)的翻译，来自[标签超市](https://github.com/wfjsw/danbooru-diffusion-prompt-builder)的翻译，来自[手抄本法术书的翻译](https://docs.google.com/spreadsheets/d/14Gg1kIGWdZGXyCC8AgYVT0lqI6IivLzZOdIT3QMWwVI/)，以及[窝自己](https://github.com/byzod/a1111-sd-webui-tagcomplete-CN)的300来个翻译

其中来自`中文化danbooru-tag 人名.xlsx`的tag完全没有翻译，只是摘取了有中文和日文的部分塞进去（理直气壮

因为 ~完全妹有翻译~ 只做了微不足道的翻译，和一些复制粘贴的工作，欢迎dalao fork完善


## 文件说明

文件|说明
---|---
Tags-zh-full-pack.csv  | 新版格式翻译，适用于[tagcomplete 1.11](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete/releases/tag/1.11.0)及之后的版本
config.json  | 新版格式配置文件, 默认值与官方配置不同
Tags-zh-full-pack-legacy.csv  | 旧版格式翻译，适用于[tagcomplete 1.10](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete/releases/tag/1.10.1)及之前的版本
config-legacy.json| 旧版格式配置文件, 默认值与官方配置不同


## 安装

1. 安装[tagcomplete](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete#installation)
2. 将`Tags-zh-full-pack.csv`（或旧版`-legacy`）放到`<tag-autocomplete安装目录>\tags\`中
3. 可选方案：
    1. 将`config.json`（或旧版`config-legacy.json`重命名为`config.json`后）放到`<tag-autocomplete安装目录>\tags\`中覆盖对应文件
    2. 打开`<tag-autocomplete安装目录>\tags\config.json`，修改`"translationFile": "",`为`"translationFile": "Tags-zh-full-pack.csv"` （旧版：修改`"extraFile": "",`为`"extraFile": "Tags-zh-full-pack-legacy.csv",`
4. 根据[官方配置说明](https://github.com/DominikDoom/a1111-sd-webui-tagcomplete#config)按照自己的喜好修改配置
