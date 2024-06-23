## $\textcolor{red}{\textsf{Compact Caesar Cipher}}$
=======================================================================================

## GUI Python3 (`Jupyter Notebook`)
```py
import ipywidgets
def r_string(s,k): return(''.join([ chr(97+(ord(c)-97+k)%26) for c in s ]))
def F():
    import ipywidgets as widgets
    from ipywidgets import HBox, VBox
    import numpy as np
    import matplotlib.pyplot as plt
    from IPython.display import display
    %matplotlib inline
    @widgets.interact
    def f(BOX=widgets.Text(value='abcdefghijklmnopqrstuvwxyz', disabled=False),k=range(0,26)):
        plain_text = BOX
        print(r_string(BOX,k))
F()
```
![image](https://github.com/loneicewolf/Compact-Caesar-Cipher/assets/68499986/a49fbf22-f3dc-4ba5-ac32-21b941ebddb1)
![image](https://github.com/loneicewolf/Compact-Caesar-Cipher/assets/68499986/5002bf53-1a3f-4f93-ad13-9cb78992fe3b)
- [implementation](https://github.com/loneicewolf/ciphers-python/blob/main/Caesar_Cipher.py)

```
#https://github.com/jupyter-widgets/ipywidgets/issues/1775
import ipywidgets as widgets

out = widgets.Output()
def on_value_change(change):
    with out:
        #print("here ",change['new'])
        k=change['new']
        print(r_string("abc",k))
slider = widgets.IntSlider(min=1, max=26, step=1, continuous_update=True)
play = widgets.Play(min=1, interval=50)

slider.observe(on_value_change, 'value')
widgets.jslink((play, 'value'), (slider, 'value'))
widgets.VBox([play, slider, out])
```

=======================================================================================
## JavaScript (js)
- [implementation](http://stackoverflow.com/a/617685/987044)
```js
function rot(s,i) {return s.replace(/[a-zA-Z]/g, function (c) {  return String.fromCharCode((c <= 'Z' ? 90 : 122) >= (c = c.charCodeAt(0) + i) ? c : c - 26); });}
```
![image](https://github.com/loneicewolf/Compact-Caesar-Cipher/assets/68499986/b6a61be9-efd5-477b-aab7-0742c4f41d4e)

=======================================================================================

