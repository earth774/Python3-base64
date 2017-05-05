# Python3-base64-to-Picture
Ex. File base_64.py is example To develop. 

## Import

```python
import base64
```

## Encode base64

important encode

```python
UU = base64.b64encode(f.read())
```

```python
with open(r"E:\New folder (2)\Store.jpg", "rb") as f:
        #data12 = f.read()
	UU = base64.b64encode(f.read())
        #UUU = base64.b64decode(UU)

	print(UU) 
```



## Decode base64

get encode to decode

```python
imgdata = base64.b64decode(UU)
```

```python
imgdata = base64.b64decode(UU) 
filename = "aa"+".jpg"  
with open(filename, 'wb') as f:
    f.write(imgdata)
```

## Overview

```python
import base64
with open(r"E:\New folder (2)\Store.jpg", "rb") as f:
        #data12 = f.read()
	UU = base64.b64encode(f.read())
        #UUU = base64.b64decode(UU)

	print(UU) # sent base 64 text for process become to pic

imgdata = base64.b64decode(UU) # Get UU for base 64 text to pic 
ppp = strftime("%d-%m-%Yh%Hm%Ms%S", localtime())
filename = ppp+".jpg"  # I assume you have a way of picking unique filenames
with open(filename, 'wb') as f:
    f.write(imgdata)
```