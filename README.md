# Compact-Caesar-Cipher

Python3 (py)
```py

```



## JavaScript (js)
- [implementation](http://stackoverflow.com/a/617685/987044)
```js
<script type="text/javascript">
    function rot(s, i)    {  return s.replace(/[a-zA-Z]/g, function (c) {  return String.fromCharCode((c <= 'Z' ? 90 : 122) >= (c = c.charCodeAt(0) + i) ? c : c - 26); });   }
    function update() {  document.getElementById('output').value = rot(document.getElementById('input').value, +document.getElementById('rot').value);   }
</script>
```


