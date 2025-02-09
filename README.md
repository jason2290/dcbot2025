# dcbot2025
一個用於DC自動化操作的項目，方便您管理各項DC大小事務  
請與作者取得聯繫之後並取得權限後，前往[dcbot-2025-](https://github.com/jason2290/dcbot-2025-)
## 📖 目錄
### 聊天機器人`dcchatbot`  
   當前版本:v1.2 (2025/2/9更新)
  - 新增RANDOM_CHAT，可選擇是否隨機選取訊息發送  
  - 新增DELETE_AFTER_SEND，可選擇是否於訊息發送後刪除資料庫
      
`v1.1 (2025/2/8更新)`- 修正時間無法讀取問題- 新增傳送訊息錯誤時報錯
### 蒐集聊天機器人`dccollectbot`
   當前版本:v1.1 (2025/2/9更新)
  - 新增黑名單功能，包含黑名單指定的字詞不會建檔至資料庫
  - 新增自訂最小字詞長度功能，低於指定字數的句子不會建檔至資料庫
  - 新增延時建檔功能，訊息發送後10秒內被刪除(包含被MOD機器人刪除)不會建檔至資料庫
### Role機器人`dcrolebot`
   當前版本:v1
   
---
## ✨ 聊天機器人 `dcchatbot`
`dcchatbot`是一個基於`Python`的訊息推送工具，支援多帳號同步隨機推送

### 🔧 安裝
請確保您已安裝[Python](https://www.python.org/downloads/) 不一定要求版本完全相符  
本程式撰寫時使用的版本為Python 3.12.5  
若使用上有問題可以用`python --version`確認版本  

### 🔧 配置
請下載整份資料夾  
需要配置的文件有`account.csv`、`chatlist.csv`、`envexample.txt`共三份  

### 🔧 使用
文件配置好之後直接執行`python chat.py`即可  

---

## ✨ 蒐集聊天機器人 `dccollectbot`
`dccollectbot`是一個基於`Node`的訊息擷取工具，支援單帳號擷取指定頻道內所有訊息並保存

### 🔧 安裝
請確保您已安裝[Node.js](https://nodejs.org/) 和 [npm](https://www.npmjs.com/)  
不要求版本完全相符  

### 🔧 配置
請下載整份資料夾
需要配置的文件有`config.json`、`envexample.txt`共兩份

### 🔧 使用
文件配置好之後直接先執行`npm install`安裝所有需要模組  

---

## ✨ Role機器人 `dcrolebot`  
`dcrolebot`是一個基於`python`的role領取工具，支援多帳號檢查指定頻道Role並與指定Role派發機器人交互領取缺失的Role

### 🔧 安裝
請確保您已安裝[Python](https://www.python.org/downloads/) 不一定要求版本完全相符  
本程式撰寫時使用的版本為Python 3.12.5  
若使用上有問題可以用`python --version`確認版本  

### 🔧 配置
請下載整份資料夾
需要配置的文件有`account.csv`共一份

### 🔧 使用
文件配置好之後須分三步執行腳本

