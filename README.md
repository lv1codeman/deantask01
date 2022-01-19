# First to do #

初始npm  
```npm init```  
  
安裝plugins  
```npm install```  
  
安裝後執行  
```npm start```   
  
**gulp**會執行專案中的gulpfile.js  
  
已知會被啟用的功能：  
* Browsersync
* node-sass
* gulp

## Browsersync ##

會自動開啟localhost:3000  
此時在localhost:3001也會跑Browsersync  

這時候只要修改*index.html*按下存檔，Browsersync就會幫你更新*localhost:3000*的頁面(右上角會有提示)  

就不用一直在網頁上重新整理了  

## node-sass ##

修改scss/中的.scss檔案，也會自動幫你compile到css/底下的.css內  
	
## glup ##

根據*gulpfile.js*的語法  
會刪除vendor資料夾  
並新建一次vender資料夾，從node_modules中複製bootstrapJS, bootstrapSCSS, chartJS, dataTables, fontAwesome, jquery, jqueryEasing的檔案到vendor底下  

---

## 我做了什麼修改? ##

在空白專案中安裝**node-sass**  
```npm init```
```npm install node-sass```  

參考他的*package-lock.json*來改sb-admin-2的*package-lock.json*  
(為了讓sb-admin-2安裝時會裝最新版的**node-sass**)  
  
改好就可以執行```npm install```了，sb-admin-2會根據他的*package-lock.json*逐一安裝需要的plugin  
安裝後執行```npm start```  