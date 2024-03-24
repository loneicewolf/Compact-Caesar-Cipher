# Compact-Caesar-Cipher

Python3 (py)
```py

```



## JavaScript (js)
- [implementation](http://stackoverflow.com/a/617685/987044)
```js
function rot(s,i) {return s.replace(/[a-zA-Z]/g, function (c) {  return String.fromCharCode((c <= 'Z' ? 90 : 122) >= (c = c.charCodeAt(0) + i) ? c : c - 26); });}
```
ScreenShot
![image](https://github.com/loneicewolf/Compact-Caesar-Cipher/assets/68499986/b6a61be9-efd5-477b-aab7-0742c4f41d4e)


