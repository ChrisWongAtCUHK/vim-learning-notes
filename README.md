# Vim學習筆記

## [vim 按鍵與功能](http://note.artchiu.org/2009/04/30/vim-%e6%8c%89%e9%8d%b5%e8%88%87%e5%8a%9f%e8%83%bd/)

### 區塊選擇
* v    字元選擇，會將游標經過的地方反白選擇。
* V     行選擇，會將游標經過的反白選擇。
* [Ctrl ] + v     區塊選擇，可以用長方形的方式選擇資料。
	- [按I->輸入文字(或符號)->按Esc：多行插入](https://stackoverflow.com/questions/9549729/vim-insert-the-same-characters-across-multiple-lines)
		+ I 在前面插入
		+ A 在後面加上
* y     將反白的地方複製起來。
* d     將反白的地方刪除掉。

### 多檔案編輯
* 內使用 :r filename 可將檔案 filename 的內容在游標處插入。
* 可於 vim 後接多個檔案來同時開啟多個檔案，例如：vim filename1 filename2 filename3。

### 多檔案編輯的按鍵
* :n     編輯下一個檔案。
* :N     編輯上一個檔案。
* :files     列出目vim前開啟的所有檔案。

### 多視窗功能
* :sp     開啟同一檔案於新視窗。
* :sp filename     開啟檔案 filename 於新視窗。
* [Ctrl ] + wj     游標移動到下方的視窗。按法為：先按下 [Ctrl ] 不放，再下 w 後放開所有的按鍵，然後再按下j。
* [Ctrl ] + wk     游標移動到上方的視窗。按法為同上。
* [Ctrl ] + wq     結束下方視窗，與 [Ctrl ] + wj 移動到下方視窗後，再按下 :q 離開相同。

### 其他按鍵與功能
* :set nu     設定行號。
* :set nonu     取消定行號。
* :set wrap     自動換行。
* :set nowrap     不自動換行。
* :set hlsearch     將搜尋的字串反白。
* :set autoindent     自動縮排。
* :set noautoindent     不自動縮排。
* :set backup     自動儲存備份。備份檔名為 filename~。
* :set rule     顯示右下角的狀態說明。
* :set showmode     顯示 -insert- 等字眼在左下角的狀態列。
* :set all     顯示目前所有的環境參數設定值。
* :syntax (off | on)     是否依據程式相關語法顯示不同顏色。

