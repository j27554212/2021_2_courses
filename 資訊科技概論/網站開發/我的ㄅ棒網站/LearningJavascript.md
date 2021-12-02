# [JavaScript Examples](https://www.w3schools.com/js/js_examples.asp)

- [1.Where to Insert JavaScript](https://www.w3schools.com/js/tryit.asp?filename=tryjs_whereto_head)
  - [JavaScript in Head](https://www.w3schools.com/js/tryit.asp?filename=tryjs_whereto_head)
  - [放在另一個 js檔案]
  - [放在遠端伺服器另一個 js檔案]

- [Javascript Framework]()
  - [An introduction to d3.js in 10 basic examples.](https://www.d3-graph-gallery.com/intro_d3js.html)
  - <!-- Load d3.js -->
  - <script src="https://d3js.org/d3.v4.js"></script> 


- [如何在 JavaScript 中獲取輸入值](https://www.delftstack.com/zh-tw/howto/javascript/javascript-get-input-value/)
  -  
- [output]
  - [輸出到browser console](https://www.w3schools.com/js/tryit.asp?filename=tryjs_output_console) 
  - [輸出到HTML]()
    - document.write(5 + 6);
  - [輸出到windows alert視窗]()
    - window.alert(5 + 6);
## [DOM (Document Object Model)](https://www.w3schools.com/js/js_htmldom.asp)

## [Browser Object Model (BOM)](https://www.w3schools.com/js/js_window.asp)

## js1.html

```
<html> 
    <head> 
        <title>pre tag</title> 
		<meta charset="UTF-8">
		<script src="https://d3js.org/d3.v4.js"></script>
		<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Paragraph changed.";
}
</script>
    </head> 
    <body> 
        <pre> 
            GeeksforGeeks 
            A Computer   Science Portal   For Geeks 
        </pre> 
		            GeeksforGeeks 
            A Computer   Science Portal   For Geeks 
		<hr>
		<blockquote cite="http://developer.mozilla.org">
        <p>這是取自於 Mozilla Developer Center 的引言。</p>
        </blockquote>
		<hr>
		<h2>Demo JavaScript in Head</h2>

<p id="demo">A Paragraph.</p>

<button type="button" onclick="myFunction()">Try it</button>
		<!-- Add a svg area, empty -->
<svg id="dataviz_area" height=200 width=450></svg>

<script>
var svg = d3.select("#dataviz_area")
svg.append("circle")
  .attr("cx", 2).attr("cy", 2).attr("r", 40).style("fill", "blue");
svg.append("circle")
  .attr("cx", 140).attr("cy", 70).attr("r", 40).style("fill", "red");
svg.append("circle")
  .attr("cx", 300).attr("cy", 100).attr("r", 40).style("fill", "green");
</script>
			<hr>
			<address>
        Written by <a href="mailto:8wingflying@gmail.com">My dear Great teacher</a>.<br>
        Visit us at:<br>
         MYdeargreatteacher.com<br>
         Box 999, Hackerland<br>
         Taiwan
</address>
    </body> 
</html> 
```




## 

```
<!DOCTYPE html> 
<html> 
  
<body> 
  
  <h4> 
      Change the text of the text field  
      ,and then click the button. 
  </h4> 
  
  <label for="domTextElement">Name: </label>
  <input type="text" id="domTextElement" > 
  
  <button type="button"  onclick="getValueInput()"> 
      click me!! 
  </button> 
  
  <p id="valueInput"></p> 

  <script> 

    const getValueInput = () =>{
      let inputValue = document.getElementById("domTextElement").value; 
      document.getElementById("valueInput").innerHTML = inputValue; 
    }
    
  </script> 
</body> 
  
</html> 
```





##

```

```





##

```

```


