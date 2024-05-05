# NET4_Wireshark封包分析

## Description

The shark won't bite you. Don't worry, it's wired!

答案格式:IW{xxxxxxxxxxxxxxx}

## Solution

解壓縮 flag.zip，發現要輸入密碼

```sh
┌──(kali㉿kali)-[~]
└─$ unzip flag.zip
Archive:  flag.zip
[flag.zip] flag.txt password: 
```

查看傳送檔案的封包，發現 Authorization  標頭很可疑

![image](image/hdqu1c.png)

```sh
┌──(kali㉿kali)-[~]
└─$ echo "ZmxhZzphenVsY3JlbWE=" | base64 -d
flag:azulcrema                                                                             
```

發現 azulcrema 是 flag.zip 的密碼

```sh
┌──(kali㉿kali)-[~]
└─$ unzip flag.zip
Archive:  flag.zip
[flag.zip] flag.txt password: 
 extracting: flag.txt
                                                         
┌──(kali㉿kali)-[~]
└─$ cat flag.txt
IW{HTTP_BASIC_AUTH_IS_EASY}
```

> Flag: `IW{HTTP_BASIC_AUTH_IS_EASY}`
