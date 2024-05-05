# Big Zip

## Description

Unzip this archive and find the flag.
- [Download zip file](https://artifacts.picoctf.net/c/504/big-zip-files.zip)

## Solution

```sh
┌──(kali㉿kali)-[~/Documents/pico]
└─$ unzip big-zip-files.zip 
Archive:  big-zip-files.zip
   creating: big-zip-files/
 extracting: big-zip-files/jpvaawkrpno.txt  
  inflating: big-zip-files/oxbcyjsy.txt  
  inflating: big-zip-files/hllhxlvvdgiii.txt  
  inflating: big-zip-files/bdvnqbuutefealgveyiqd.txt  

...
以下省略
...
```


因為使用 find 沒有發現相關檔案，所以使用 grep 遞迴查詢

```sh
┌──(kali㉿kali)-[~/Documents/pico/big-zip-files]
└─$ find ./ -name "flag.txt"
                                                                             
┌──(kali㉿kali)-[~/Documents/pico/big-zip-files]
└─$ grep -r "picoCTF" ./    
./folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt:information on the record will last a billion years. Genes and brains and books encode picoCTF{gr3p_15_m4g1c_ef8790dc}
```

> Flag: `picoCTF{gr3p_15_m4g1c_ef8790dc}`
