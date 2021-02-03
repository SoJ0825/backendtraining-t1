# 前言
版本控制系統大概是最基礎的工具，不管你是在前端、後端還是 APP。熟悉 Git 是基本技能。假設你現在是一個人開發 Web 專案，你至少需要熟悉以下流程。

# 推薦學習資源
中文書：[為你自己學Git](https://gitbook.tw/)

# 問題
- Q1: 請說明
    1. 什麼是版本控制系統？ 程式開發時會有不同的開發功能以及需求, 定義每個開發的階段並紀錄該狀態, 使能夠回復或刪除該狀態, 對程式狀態進行控制, 就是版本控制
    2. Git 版本控制中有哪幾種檔案狀態？ stage / repository / remote

![](https://i.imgur.com/hZoDAPf.png)
- Q2: 上圖 A-J 是 Git 中檔案狀態切換得流程，請查出 A-J 執行的指令。(重點是確保自己真的學到在什麼情況下使用該指令。)
    - A: 將一般目錄變成 git working folder: git init
	- B: 將 working folder 的異動狀態登錄到 stage: git add
	- C: 將 stage 的狀態放到 local repository: git commit
    - D: 將 local repository 的狀態放到 remote repository: git push
    - E: 將 remote repository 的狀態取回到 local repository: git pull
    - F: 將 local repository 的狀態退回到 stage 階段（是 C 的逆向）: git reset
    - G: 將 stage 的狀態退回到 working folder 階段（是 B 的逆向）: git restore
    - H: 將 local repository 的狀態一口氣退回到 working folder 階段（是 B+C 的逆向）: git reset --hard
    - I: 從 remote repository 取回建立成新的 working folder: git clone
    - J: 將 git working folder 變回一般目錄: rm -rf .git
    
- Q3. 做這個題目，你事前評估做了什麼、利用了哪些資源、排程為何、事後怎麼驗收、得到什麼經驗？
評估：先看題目,應該是有操作過,因此決定不open book,看到底答案是否正確
