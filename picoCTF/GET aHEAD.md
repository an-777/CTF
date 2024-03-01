# GET aHEAD

## Description

Find the flag being held on this server to get ahead of the competition http://mercury.picoctf.net:53554/

## Solution

使用 `curl` 請求 `Request Method` `HEAD`
```cmd
┌──(kali㉿An777)-[~]
└─$ curl -I http://mercury.picoctf.net:53554/
HTTP/1.1 200 OK
flag: picoCTF{r3j3ct_th3_du4l1ty_2e5ba39f}
Content-type: text/html; charset=UTF-8
```
> flag : `picoCTF{r3j3ct_th3_du4l1ty_2e5ba39f}`
