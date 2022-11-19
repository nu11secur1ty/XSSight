## Date
```
alert(Date()); 
```
## List
```
alert()
confirm() 
prompt()
```
## window object
```
window.alert()
window.confirm()
window.prompt()
```
## Prompt and Print
```js
<script>
function myFunction() {
  let person = prompt("Please enter your name", "Chuskopek Pechkov");
  if (person != null) {
    document.getElementById("demo").innerHTML =
    "Hello " + person + "! How are you today?";
  }
}
</script>
```
