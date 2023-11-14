# GET aHEAD

## 題目敘述
Find the flag being held on this server to get ahead of the competition
http://mercury.picoctf.net:21939/

## 解題
到 CMD 輸入指令取得 `HEAD`
```cmd
curl -I http://mercury.picoctf.net:21939/
```

```
┌──(xyz㉿DrXYZ)-[~]
└─$ curl -I http://mercury.picoctf.net:21939/
HTTP/1.1 200 OK
flag: picoCTF{r3j3ct_th3_du4l1ty_6ef27873}
Content-type: text/html; charset=UTF-8
```


## flag
```
picoCTF{r3j3ct_th3_du4l1ty_6ef27873}
```
