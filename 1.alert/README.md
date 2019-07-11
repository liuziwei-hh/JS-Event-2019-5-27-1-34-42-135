## 要求 
    
- 补充以下HTML，实现点击某一个数字可以alert出该数字。

```html
  <!DOCTYPE html>
  <html lang="en">
  <head>
      <meta charset="UTF-8">
      <title>事件监听</title>
  </head>
  <body>
  
  <ul id="no">
      <li>1</li>
      <li>2</li>
      <li>3</li>
      <li>4</li>
      <li>5</li>
      <li>6</li>
      <li>7</li>
  </ul>
  
  <script>
    window.onload = function(){
    var obj_lis = document.getElementById("no").getElementsByTagName("li");
    for(i=0;i<obj_lis.length;i++){
        obj_lis[i].onclick = function(){
            alert(this.innerHTML);
        }
    }
}
  </script>
  </body>
  </html>
```
