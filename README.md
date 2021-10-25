# jiekesi
This project is only for testing, no one can use it indiscriminately. 

Onedrive 目錄索引 


功能： 
不佔用服務器空間，不走服務器流量， 


直接列出OneDrive 目錄，文件直鏈下載。 


使用及免責協議 
使用及免責協議 


安裝運行 
源碼安裝運行： 
需求： 
1、PHP空間，PHP 5.6+ 需打開curl支持 

2、OneDrive 賬號(個人、企業版或教育版/工作或學校帳戶) 

3、OneIndex 程序 


配置： 
  
計劃任務 
[可選] 後台定時刷新緩存，可增加前台訪問的速度。 推荐配置，非必需。后台定时刷新缓存，可增加前台访问的速度。


# 每小时刷新一次token
0 * * * * /具体路径/php /程序具体路径/one.php token:refresh

# 每十分钟后台刷新一遍缓存
*/10 * * * * /具体路径/php /程序具体路径/one.php cache:refresh



Docker 安裝運行 
請參考 TimeBye/oneindex

特殊文件實現功能 
README.md、 HEAD.md 、 .password特殊文件使用 


可以參考 https://github.com/donwa/oneindex/tree/files


在文件夾底部添加說明:   



在OneDrive 的文件夾中添加 README.md文件，使用Markdown 語法。 



在文件夾頭部添加說明:   



在OneDrive 的文件夾中添加 HEAD.md 文件，使用Markdown 語法。 



加密文件夾:   



在OneDrive 的文件夾中添加 .password文件，填入密碼，密碼不能為空。 



直接輸出網頁: 



在OneDrive 的文件夾中添加 index.html 文件，程序會直接輸出網頁而不列目錄。 

配合文件展示設置-直接輸出效果更佳。 


