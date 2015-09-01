# python_challenge
Random hacks at http://www.pythonchallenge.com/

### Level 0
```sh
Compute 2**38 and hit at http://www.pythonchallenge.com/pc/def/274877906944.html
```
### Level 1
Two ways are there:

1. Run this command in your terminal 

```sh
echo "g fmnc wms bgblr rpylqjyrc gr zw fylb. rfyrq ufyr amknsrcpq ypc dmp. bmgle gr gl zw fylb gq glcddgagclr ylb rfyr'q ufw rfgq rcvr gq qm jmle. sqgle qrpgle.kyicrpylq() gq pcamkkclbcb. lmu ynnjw ml rfc spj." | tr [a-xy-z] [c-za-b]
echo "map" | tr [a-xy-z] [c-za-b]
```
2. Python script
```py
import string
tbl = string.maketrans(
    "abcdefghijklmnopqrstuvwxyz", "cdefghijklmnopqrstuvwxyzab"
)

st = "g fmnc wms bgblr rpylqjyrc gr zw fylb. rfyrq ufyr amknsrcpq ypc dmp. bmgle gr gl zw fylb gq glcddgagclr ylb rfyr'q ufw rfgq rcvr gq qm jmle. sqgle qrpgle.kyicrpylq() gq pcamkkclbcb. lmu ynnjw ml rfc spj."

print st.translate(tbl) # i hope you didnt translate it by hand. thats what computers are for. doing it in by hand is inefficient and that's why this text is so long. using string.maketrans() is recommended. now apply on the url.
url = "map"
url = url.translate(tbl)
```

