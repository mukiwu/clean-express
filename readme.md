# Express Clean APP

使用 Express Generator 產生的 Express Clean 專案資料夾，供每次開發使用。

## 用到的設定

* 樣板引擎：ejs

* CSS 預處理器：compass / scss (含大括號以及分號)

## 安裝方法

```
npm install
```

```
nodemon app.js
```

預設 port 為 3000，請在網頁輸入 http://localhost:3000 以瀏覽網站。

## nodemon 簡易介紹

使用 nodemon 套件，自動協助重啟伺服器。

測試完後如需上正式站，請記得打開 `app.js`，將以下程式碼做調整：

```
// 移除原本的註釋
module.exports = app;

// 以下全部都可以移除
var debug = require('debug')('my-application');
app.set('port', process.env.PORT || 3000);
var server = app.listen(app.get('port'), function() {
debug('Express server listening on port ' + server.address().port);
});
```

