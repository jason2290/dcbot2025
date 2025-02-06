# dcbot2025
一個用於DC自動化操作的項目，方便您管理各項DC大小事務  
請與作者取得聯繫之後並取得權限後，前往[dcbot-2025-](https://github.com/jason2290/dcbot-2025-)
## 📖 目錄
- 聊天機器人`dcchatbot`
- 蒐集聊天機器人`dccollectbot`
- Role機器人`dcrolebot`

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
1. `account.csv`中請配置Dc token，一行一個帳號  
2. `chatlist.csv`中請配置要發送的訊息，一行一個訊息  
腳本為防止重複傳送訊息  
會在發送訊息之後自動刪除文檔中的訊息  
若希望重複傳送一樣的訊息  
複製貼上多行相同的訊息即可  
3. `envexample.txt`中配置各種參數，詳細部分會在檔案中註明  
**注意在配置後須將檔案更名為`.env`**

### 🔧 使用
文件配置好之後直接執行`python chat.py`即可  
第一次執行前請先執行`pip install aiohttp python-dotenv`安裝必要模組

---

## ✨ 蒐集聊天機器人 `dccollectbot`
`dccollectbot`是一個基於`Node`的訊息擷取工具，支援單帳號擷取指定頻道內所有訊息並保存

### 🔧 安裝
請確保您已安裝[Node.js](https://nodejs.org/) 和 [npm](https://www.npmjs.com/)  
不要求版本完全相符  

### 🔧 配置
請下載整份資料夾
需要配置的文件有`config.json`、`envexample.txt`共兩份
1. `config.json`中配置"allowedChannelsIds"即可，支持同時填入多個頻道
2. `envexample.txt`中配置DISCORD_TOKEN該項即可  
**注意在配置後須將檔案更名為`.env`**

### 🔧 使用
文件配置好之後直接先執行`npm install`安裝所有需要模組  
再執行`node .`開始執行程式擷取資料

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
1. `account.csv`中僅需配置第一欄位`token`即可  
其餘資料在腳本執行時會自動補上  
Role機器人參數配置較為複雜故不支援使用.env自行修改參數

### 🔧 使用
文件配置好之後須分三步執行腳本
1. `python 1-getuser.py`獲取帳號資訊  
   本步驟若無新增帳號只需執行一次  
   執行之後會自動取得後續步驟需要資料
3. `python 2-roleclick.py`會檢查帳號是否有role，無role的會自動領取
4. `python 3-getrole.py`獲取帳號的role資訊
   執行之後會顯示各個帳號的資訊，用以檢查role是否領取成功

