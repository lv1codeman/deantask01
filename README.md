
## First to do ##
先在空白專案中安裝npm install node-sass
參考他的package-lock.json來改sb-admin-2的package-lock.json
(為了讓sb-admin-2安裝時會裝最新版的node-sass)

改好就可以執行npm install了，sb-admin-2會根據他的package-lock.json逐一安裝需要的plugin
安裝後執行npm start
會自動開啟localhost:3000


## Browsersync ##
此時在localhost:3001也會跑Browsersync

這時候只要修改index.html按下存檔，Browsersync就會幫你更新localhost:3000的頁面(右上角會有提示)

就不用一直在網頁上重新整理了

## node-sass ##
修改scss/中的.scss檔案，也會自動幫你compile到css/底下的.css內





