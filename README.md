# VGTNTool

專案頁面：[VGTNTool](https://zh.wikipedia.org/wiki/User:SuperGrey/gadgets/VGTNTool)

為 [Module:Vgtn/data](https://zh.wikipedia.org/wiki/Module:Vgtn/data) 提供了更直觀的編輯視圖——現在可以直接在 [WikiProject:電子遊戲/譯名表](https://zh.wikipedia.org/wiki/WikiProject:電子遊戲/譯名表) 上編輯了。 

## 使用方式
### 發行版本
将如下程式碼复制至 [User:你的用戶名/common.js](https://zh.wikipedia.org/wiki/Special:MyPage/common.js) 頁面：

```js
importScript('User:SuperGrey/gadgets/VGTNTool/main.js');  // Backlink: [[User:SuperGrey/gadgets/VGTNTool]]
```

### 從原始碼建構

1. **安裝 Node.js**
   - 請先安裝 [Node.js](https://nodejs.org/)。

2. **安裝依賴套件**
   - 在 VGTNTool 目錄下執行：
     ```sh
     npm install
     ```

3. **建構 Bundled 版本**
   - 執行下列指令以產生 `dist/bundled.js`：
     ```sh
     npm run build
     ```
   - 若需持續監看檔案變動並自動重建，請執行：
     ```sh
     npm run watch
     ```

4. **安裝至維基**
   - 將 `dist/bundled.js` 上傳至你的維基用戶頁面，例如 [User:你的用戶名/VGTNTool.js](https://zh.wikipedia.org/wiki/Special:MyPage/VGTNTool.js)。
   - 在 [User:你的用戶名/common.js](https://zh.wikipedia.org/wiki/Special:MyPage/common.js) 頁面加入：
     ```js
     importScript('User:你的用戶名/VGTNTool.js');  // 修改為你的用戶名
     ```
