# Compact-Caesar-Cipher

## Python3 (py)
- [implementation](https://github.com/loneicewolf/ciphers-python/blob/main/Caesar_Cipher.py)
```py
def r_string(s,k): return(''.join([ chr(97+(ord(c)-97+k)%26) for c in s ]))
def r_letter(l,k): return(chr(97+(ord(l)-97+k)%26))
```
![image](https://github.com/loneicewolf/Compact-Caesar-Cipher/assets/68499986/5002bf53-1a3f-4f93-ad13-9cb78992fe3b)



## JavaScript (js)
- [implementation](http://stackoverflow.com/a/617685/987044)
```js
function rot(s,i) {return s.replace(/[a-zA-Z]/g, function (c) {  return String.fromCharCode((c <= 'Z' ? 90 : 122) >= (c = c.charCodeAt(0) + i) ? c : c - 26); });}
```
![image](https://github.com/loneicewolf/Compact-Caesar-Cipher/assets/68499986/b6a61be9-efd5-477b-aab7-0742c4f41d4e)

