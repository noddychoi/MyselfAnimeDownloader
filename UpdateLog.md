# 更新日誌

## ver1.0.2
- 1.將很多功能拆到 event 資料夾裡，減少 main.py 的行數。
	- 有些功能拆到別的 .py 檔時，可以正常的創建 QtWidget 的物件，有些則不行，不知道為什麼??
	- 有些功能則是拆過去版面配置會亂掉，所以不拆。
- 2.將 `wait_list`, `now_list`拔掉，改成單獨一個 `download_queue`因這個改動程式碼做了大幅的改動。
	- main.py。
		- 提升與降低優先權的程式碼。
		- 剛開啟時讀取上一次動漫載到哪裡的程式碼。
		- 創建下載任務 TableWidget 的程式碼。
	- Myself_thread.py。
		- Class DownloadVideo 。
- 3.新增UpadteLog.md。
- 4.README 更新。

## ver1.0.1
- 1.修正 下載 wait 到 now 後，又新增資料到　 wait 裡面問題，不知道為什麼之前都沒發現?? 還是是之後拆開功能才發生的BUG??  未來將重寫續下載功能，現在這種方式有點不穩又怪怪的，現在測試的時候有出現BUG，但沒有每次都發生所以找不到問題點在哪。
- 2.現在手動查詢版本狀況已經是最新版本時會跳出提示。
- 3.解決 Mac 因排版亂掉發生點不到功能的問題

## ver1.0
- 12/05 的 版本
![image](https://i.imgur.com/WYDIX0m.gif)<br>