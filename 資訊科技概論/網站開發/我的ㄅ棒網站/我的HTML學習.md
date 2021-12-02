

## HTML檔案結構

- 範例程式
- [HTML 文件的 doctype](https://www.wibibi.com/info.php?tid=403)
- HTML 文件的根元素`<html>` 元素 


- [HTML 文件的標頭`<head>` 元素](https://www.wibibi.com/info.php?tid=414)
  - `<head>` 標籤開始，至` </head>` 標籤結束
  - 寫在網頁 HTML 程式碼的最開頭部分
  - 開頭 `<head>` 與結尾 `</head>` 標籤之間，可以放置網頁的其他重要元素，如 title、meta、link、script、style、base 等
  - 用來標示網頁的許多基本資訊
  - 瀏覽器（browser）會根據 `<head></head>` 標籤內的資訊，呈現出設計師所設計的網頁樣貌
  - 一個網頁僅能有一組 head 標籤，也只需要一組 head 標籤 
  - [HTML title 網頁標題](https://www.wibibi.com/info.php?tid=118)
  - [HTML meta 標籤](https://www.wibibi.com/info.php?tid=415)

- HTML 文件的主體`<body>` 元素

  - [HTML H1 H2 H3 H4 H5 H6 標題](https://www.wibibi.com/info.php?tid=354)
- HTML5 新增的結構元素 

## 文件結構與基本排版

- 區塊格式
  - [pre 元素 (預先格式化區塊)](https://github.com/MyDearGreatTeacher/2021_2_courses/blob/main/%E8%B3%87%E8%A8%8A%E7%A7%91%E6%8A%80%E6%A6%82%E8%AB%96/%E7%B6%B2%E7%AB%99%E9%96%8B%E7%99%BC/%E6%88%91%E7%9A%84%E3%84%85%E6%A3%92%E7%B6%B2%E7%AB%99/html_pre.md)
  - [blockquote 元素 (引述區塊)](https://developer.mozilla.org/zh-TW/docs/Web/HTML/Element/blockquote)  [說明2](https://www.w3schools.com/tags/tag_blockquote.asp)
  - [address 元素 (聯絡資訊)](https://www.w3schools.com/tags/tag_address.asp)
  - [hr 元素 (水平線)](https://www.w3schools.com/tags/tag_hr.asp)
 
- 插入或刪除資料==> ins、del 元素

```html
  <html> 
    <head> 
        <title>pre tag</title> 
		<meta charset="UTF-8">
    </head> 
    <body> 
        <pre> 
            GeeksforGeeks 
            A Computer   Science Portal   For Geeks 
        </pre> 
		            GeeksforGeeks 
            A Computer   Science Portal   For Geeks 
		
		<blockquote cite="http://developer.mozilla.org">
        <p>這是取自於 Mozilla Developer Center 的引言。</p>
			
	<hr>
			
        </blockquote>
      
	<hr>
      	
	<address>
        Written by <a href="mailto:8wingflying@gmail.com">My dear Great teacher</a>.<br>
        Visit us at:<br>
         MYdeargreatteacher.com<br>
         Box 999, Hackerland<br>
         Taiwan
    </body> 
</html> 
```
## [清單列表lists](https://www.w3schools.com/html/html_lists.asp)
- 無順序清單列表(Unordered List)與編號==>` <ul>、<li>` 元素
- 有序清單列表(Ordered List)與編號==>` <ol>、<li>` 元素
- 定義清單(Description List) ==>` <dl>、<dt>、<dd>` 元素

- 如何把清單列表lists 置中 呈現? [How to center an unordered list?](https://stackoverflow.com/questions/19443013/how-to-center-an-unordered-list)


## 文字格式 [HTML Formatting Elements](https://www.w3schools.com/html/html_formatting.asp)
- Formatting elements were designed to display special types of text:
```
<b> - Bold text
<strong> - Important text
<i> - Italic text
<em> - Emphasized text
<mark> - Marked text
<small> - Smaller text
<del> - Deleted text
<ins> - Inserted text
<sub> - Subscript text
<sup> - Superscript text
```
- [HTML 網頁文字加入底線](https://www.wibibi.com/info.php?tid=143)
- [HTML font 文字](https://www.wibibi.com/info.php?tid=397)

## [超連結(hyperlink) `<a> </a>`](https://www.fooish.com/html/hyperlink-a-tag.html)

- <a href="https:你的github網址" target="_blank">我的github</a>
- 常用到的三個功能分別是 href、target 以及 title
- href 用來標示超連結要連到哪個網址
- target 用來標示連結的目標
  - target="_blank" - 意思是在新視窗開啟
  - target="_self" - 意思是在原本的視窗開啟
  - target="_parent" - 意思是在父層視窗開啟

- [相對URL 的路徑資訊 `<base>` ](https://www.fooish.com/html/base-tag.html)

## 圖片的展示 [HTML Images](https://www.w3schools.com/html/html_images.asp)
  
- 嵌入圖片==> `<img>` 元素 Images
- Image Map(圖片地圖)
- Background Images(背景圖片)
- The `Picture` Element
- 可附標題內容的圖片 `<figure>、<figcaption>` 元素
  
- `<img>` `<figure>` `Picture`有何區別?

## 表格(Table)

```
- 建立表格==> <table>、<tr>、<td>、<th> 元素
- 表格標題==> <caption> 元素
- 表格的表頭、主體與表尾－<thead>、<tbody>、<tfoot> 元素
- 直行式表格==> <colgroup>、<col> 元素
```


## 聲音(audio) 與 影片(Video)

```
- 嵌入影片==> <video> 元素
- 嵌入聲音==> <audio> 元素
- 嵌入物件==> <object> 元素
- 嵌入Script ==> <script>、<noscript> 元素
- 嵌入浮動框架 ==> <iframe> 元素
- 內嵌youtube影片
```
## 表單(FORM)
```
- 建立表單 ==> <form>、<input> 元素
- 按鈕 ==> <button> 元素
- 標籤 ==> <label> 元素
- 群組標籤 ==> <optgroup> 元素
- 將表單欄位框起來 ==> <fieldset>、<legend> 元素
```
## 其他HTML 戰技

- [網頁跑馬燈語法教學 HTML marquee 程式設計](https://www.wibibi.com/info.php?tid=68)
- 網頁自動導向



