# Github 上現成的一個angular2+nginx+django的project

1. django:onbuild改成python:3.5-onbuild
1. 先執行看看是否會出錯，django使用1.9.X, angular2的package.json改為最新版->整個炸，完全不會動->angular2的部份直接由nginx處理。
1. 2016.12.08 更新了docker-compose.yml 及nginx的default.conf，angular2搬到nginx 目錄內。在angular2內執行`npm install` 就可以執行了。docker內的angular2不能即時更新，但只需執行`docker-compose restart`即可。
1. 更新版本，由於django與angular2都更新很多版了。
1. 把資料庫更新為postgres
1. 加上redis
1. 正式成為開發版本