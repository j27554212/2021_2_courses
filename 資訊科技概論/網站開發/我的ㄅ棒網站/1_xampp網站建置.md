# xampp網站建置

## xampp
- XAMPP是最流行的PHP開發環境
- XAMPP是完全免費且易於安裝的Apache發行版本，其中包含MariaDB、PHP和Perl。XAMPP開放源碼套件的設置讓安裝和使用出奇容易。
  - 網站伺服器(web server) ==> Apache
  - 資料庫伺服器(database server) ==> MariaDB
  - 伺服器程式開發engine  ==> PHP

- [下載](https://www.apachefriends.org/zh_tw/download.html)

## xampp目錄結構

- 網站程式放在  C:\xampp\htdocs
- 你自己開發的網站 C:\xampp\htdocs\dragon
  - 第一個網頁 C:\xampp\htdocs\dragon\index.html

```
c:\xampp>dir *.exe
 磁碟區 C 中的磁碟沒有標籤。
 磁碟區序號:  4A50-AC15

 c:\xampp 的目錄

2013/03/30  下午 08:29            60,928 service.exe
2021/10/07  下午 02:27        12,521,156 uninstall.exe
2021/04/06  下午 07:38         3,368,448 xampp-control.exe  ==> 
2013/03/30  下午 08:29           118,784 xampp_start.exe
2013/03/30  下午 08:29           118,784 xampp_stop.exe
               5 個檔案      16,188,100 位元組
               0 個目錄  392,993,292,288 位元組可用
```

## 課本補充範例
```
<!DOCTYPE html>
<html>


<head>
    <title>Audio and Video</title>
</head>


<body>

<h1>Audio</h1>

<audio controls autoplay>
    <source src="media/music.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>

<h1>Video</h1>

<video width="320" height="240" controls>
    <source src="media/breakfast.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

</body>
</html>
```

![web1.png](web1.png)

## 我的第一支程式
```html
<!DOCTYPE html>
<html>
<head>
    <title>MY First web programming</title>
</head>
<body>

<h1>Hello My friens</h1>


<h3>中文不會通嗎?</h3>


</body>
</html>
```
![web2.png](web2.png)

## 第二支程式
```html
<!DOCTYPE html>
<html>

<head>
    <title>MY First web programming</title>
	<meta charset="utf-8">
</head>

<body>

<h1>Hello My friens</h1>


<h3>中文不會通嗎?</h3>


</body>
</html>
```

![web3.png](web3.png)
