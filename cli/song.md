# 前言
相信大家看過很多電影裡面的帥氣駭客們，總是在黑底白字的介面前面輸入指令操控著電腦。 身為一個工程師，我們當然也要立志當帥氣的工程師，既然如此就得好好學學怎麼使用這烏漆抹黑的介面。

# 推薦學習資源
[鳥哥的 Linux 私房菜](https://linux.vbird.org/linux_basic/centos7/)

# 問題

### 名詞解釋

- GUI vs CLI : 
GUI: Graphical user interface; 圖形操作界面, 透過圖形或按鈕來執行功能
CLI: command line interface; 透過指令執行功能

- terminal :
在電腦是指透過硬體進行資料輸入

- shell
    - bash
    - zsh 
    
    兩者都是linux執行shell; 在Spelling Correctiong上zsh較有效率

### 請解釋下方 CLI 的指令作用
    
- `cat` : 顯示檔案內容, 如 $cat filename1

- `cd` : 改變目前所在工作資料夾位址, 如 $cd /home/username/Downloads

- `chgrp` : 更改檔案或資料夾group權限, 如 $sudo chgrp geeksforgeeks abc.txt

- `chown` : 更改檔案或資料夾所有者權限, 如 $chown geeksforgeeks file1; 只有root才能使用chown指令

- `chmod` : 更改檔案或資料夾rwx(read, write, execute)權限, 可選擇不同對象, 如
    u: User, meaning the owner of the file.
    g: Group, meaning members of the group the file belongs to.
    o: Others, meaning people not governed by the u and g permissions.
    a: All, meaning all of the above.
; 指令 $chmod u=rw,og=r new_file.txt 

- `cp` : 複製資料至指定資料夾; $cp Src_file Dest_file

- `curl` : 一個透過HTTP Protocol存取網路資源的指令; 可應用在RESTful操作 / 替代postmant的endpoint測試

- `less` : 顯示檔案內容, 一次一頁; $ less filename
 
- `ls` : 顯示資料夾底下的檔案或資料夾名稱; $ls

- `man` : 顯示個指令的使用說明; $ man command-name

- `mkdir` : 創建資料夾; $ mkdir filename
    
- `mv` : 更改名稱或移動檔案至指定資料夾; $ mv filename1 filename2 / $ mv filename filedir

- `grep` : 搜尋檔案中的關鍵字; $ grep 'word' filename; 可加上參數 -i case-insensitive / -R 搜尋所有目前資料夾及棋子資料夾所有檔案 / -c 顯示關鍵字出現次數 

- `|` : 用來分開指令的符號, 如 mkdir file | cp filename1 filename2

- `pwd` : 顯示目前工作資料夾

- `rm` : 刪除檔案

- `touch` : 新增或編輯檔案, 如  $ touch filename

- `vim` : 以vim編輯器遍及檔案, 如 vim filename

### 請說明以下 Linux file system structure 

- `/` : 根目錄, 所有資料夾的源頭

- `/bin` : user 二進位執行檔所在位置

- `/etc` : configure file所在位址

- `/home` : 所有user的個人檔案, 如 /home/john, /home/nikita

- `/lib` : 系統檔案

- `/var` : 可能CRUD檔案所在位置, 如 system log files (/var/log); packages and database files (/var/lib);  

- `/sbin` : system 二進位執行檔所在位置

- `/srv` : server 資料所在位置

- `/tmp` : 暫存資料夾位置, 當系統reboot時所有檔案會刪除

- `/usr` : user的各種資料, 如 binaries, libraries, documentation, and source-code
