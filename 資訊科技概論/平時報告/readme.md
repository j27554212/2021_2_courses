# Agenda
- 標題:網站開發技術
- Agenda:
  - Web programming
  - 網站建置
  - HTML 開發技術
  - CSS開發技術
  - JAVAscript開發技術
  - 我的ㄅ棒網站: 網站架構


## Web programming
- 2-4頁簡報說明
- 客戶端網頁程式開發(Client-side web programming)
- 伺服端網頁程式開發(Server-side web programming)

## 網站建置
- xampp :一頁說明
- 安裝過程: 三頁說明
- 網站目錄:一頁說明

## HTML 開發技術
- [HTML: HyperText Markup Language](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [Paragraphs](https://www.w3schools.com/html/html_paragraphs.asp)
  - [div](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_div)
- [HTML Images](https://www.w3schools.com/html/html_images.asp)
  - [gif animation](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_hackman)
  - [Image Map](https://www.w3schools.com/html/html_images_imagemap.asp)
  - [Background Image on a HTML element](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_background3) 
- [Marquee](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/marquee)
- [Audio](https://www.w3schools.com/html/html5_audio.asp)
- [Video](https://www.w3schools.com/html/html5_video.asp)
- [HTML YouTube Videos](https://www.w3schools.com/html/html_youtube.asp)
- [frame](https://www.w3schools.com/html/html_iframe.asp)
- [Table](https://www.w3schools.com/html/html_tables.asp)
- [Form](https://www.w3schools.com/html/html_forms.asp)
- [HTML canvas](https://www.w3schools.com/html/html5_canvas.asp)
  - [A looping panorama](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_animations) 
- [HTML Layout](https://www.w3schools.com/html/html_layout.asp)
- [HTML Responsive Web Design](https://www.w3schools.com/html/html_responsive.asp)


## CSS開發技術
- [Inline CSS](https://www.w3schools.com/html/html_css.asp)
- [Internal CSS](https://www.w3schools.com/html/html_css.asp)
- [External CSS](https://www.w3schools.com/html/html_css.asp)
  - 相同目錄下的XXX.css
  - 遠方網站的YYY.css  

## JAVAscript開發技術

## 我的ㄅ棒網站: 網站架構
- 首頁:index.html
  - 入崑山 拜龍師 學藝記
- 五支純html程式
- 3支CSS程式
- 2支javascript程式

## HTML進階主題: HTML Canvas 
- [Canvas 教學文件](https://developer.mozilla.org/zh-TW/docs/Web/API/Canvas_API/Tutorial)

### [簡單範例]()
```html
<!DOCTYPE html>
<html>
<body>

<canvas id="myCanvas" width="200" height="100" style="border:1px solid #d3d3d3;">
Your browser does not support the HTML canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.font = "30px Arial";
ctx.strokeText("Hello World",10,50);
</script>

</body>
</html>
```

- [太陽系動畫](https://developer.mozilla.org/zh-TW/docs/Web/API/Canvas_API/Tutorial/Basic_animations)
- [循環景色](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_animations)
