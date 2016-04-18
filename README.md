# FreeBSD 操作手冊 (繁體中文)

FreeBSD 文件計劃開始採用 GNU gettext 的方式來執行翻譯，GNU gettext 做為翻譯工具已相當成熟且已有許多可支援線上協同翻譯的平台，這解決了原採用 Docbook 格式無法同步最新的原文翻譯文件以及多人共同翻譯的問題。
但要採用 GNU gettext 的模式必須先將既有採用 Docbook 的文件內容轉移至 PO 檔，否則無法並存，本專案目標解決以下幾個問題：

- [ ] 將既有 Docbook 格式轉換為 GNU gettext 的 PO 格式以讓未來可以有更多人可參與翻譯工作
- [ ] 同步及匯整舊有翻譯至最新的原文翻譯版本以跟上目前的文件版本
- [ ] 統整文件內目錄標題以及相關名詞

# 如何翻譯?
* [book.html](book.html) 為採用 GNU gettext 翻譯所產生的新版文件
* [book.ori.html](book.ori.html) 為舊版本用 Docbook 翻譯所產生的舊版文件
* [zh_TW.po](zh_TW.po) 為 GNU gettext 的翻譯檔
* [book.xml](book.xml) 為使用 GNU gettext 翻譯檔所產生的 Docbook 文件

第一階段目標是將既有的舊版翻譯移植至 GNU gettext 的 PO 格式，舊版翻譯請參考 [book.ori.html](book.ori.html)。
由於 PO 檔所參照是最新版本的原文，因此，若舊有譯文與新版原有出入之部份需要予以修正，需盡可能保留先前翻譯人員的成果。

欲協助翻譯的人員可使用 git 下載最新修訂版本 [zh_TW.po](zh_TW.po) 檔案並採用以下 PO 檔編輯器進行翻譯，翻譯完的最終版本會統一提交至 FreeBSD Documentation Project。

要查看轉文成文件的翻譯成果可將所有檔案以 zip 格式下載至電腦並使用瀏覽器開啟 book.html。

# 官方文件
https://www.freebsd.org/doc/en_US.ISO8859-1/books/fdp-primer/po-translations.html

# PO 檔編輯器

##### Windows, Mac OS X
https://poedit.net/
##### Ubuntu
```
apt-get install poedit
```
##### FreeBSD
```
pkg install poedit
```

# 翻譯名詞對照表
| 原文  | 譯文 |
| ------------- | ------------- |
| Committer | 提交者 |
| Audit | 稽查 | 
| Disk | 磁碟 |
| Drive | 磁碟機 |
| Device | 裝置 |
| CD-ROM, DVD Drive | CD-ROM, DVD 光碟機 |
| Mount | 掛載 |
| Unmount | 卸載 |
| Home directory | 家目錄 |
| Signal | 信號 |
| Common Address Redundancy Protocol | 共用位址備援協定 |
| Line Printer | 行列式印表機 |
| Serial | 序列 |
| Spool, Spooling | 暫存 (需附註原文) |
| Script | (不翻譯) |
| Log | 日誌 (需附註原文) |
| System call | 系統呼叫 (需附註原文) |
| Slice  | TBD |
| third-party software | 第三方軟體 |
| Partition  | TBD |
| Partitioning | TBD |
| Swap Space | 交換空間 |
| Ports Collection | TBD, Ports 套件集 |
| Binary Package | TBD, Binary 套件 |
| Base System | TBD |
| Package | TBD, 套件 |
| Journaling | TBD | 
| Shell | (不翻譯) |
| Daemon | (不翻譯) |
| Console | (不翻譯) |
| Binary | (不翻譯) |
| Plugin | 附加元件 |
| Productivity Tools | 辦工工具 |

# PO 線上協同翻譯平台
* https://hosted.weblate.org/
* https://translatewiki.net/
* https://www.transifex.com/
