# 五筆字型

配方： ℞ **wubi98**

[Rime](http://rime.im) 五筆字型輸入方案

五筆字型 98 及新世纪版 （源自 https://github.com/lswqzhang/RIME-wubi）

## 安裝

拼音反查、五筆拼音混合輸入依賴於

  - [袖珍简化字拼音](https://github.com/rime/rime-pinyin-simp) ℞ **`pinyin-simp`**

[東風破](https://github.com/rime/plum) 安裝口令(这里以fcitx-rime为例)： 

`git clone --depth 1 https://github.com/rime/plum.git`

`cd plum/`

`rime_frontend=fcitx-rime bash rime-install pinyin-simp`

`rime_frontend=fcitx-rime bash rime-install hlizard/rime-wubi98`

`cd /usr/share/rime-data`

`sudo vim default.yaml`

增加：
  - schema: wubi98_pinyin
  - schema: wubi98_trad

然后重新启动fcitx，切换中州韵， ctrl+\`选择输入方案即可。

模糊音设置请看文件 pinyin_simp.custom.yaml

授權條款：見 [LICENSE](LICENSE)
