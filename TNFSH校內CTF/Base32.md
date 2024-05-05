# Base64

## Description

編碼與解碼是資訊領域日常都在使用的技術，Base32是由使用26個字母A-Z和數字0-9的編碼。

請問你對Base32編碼與解碼的技術了解嗎?

你知道如何解碼下列資料嗎:
IJZGKYLLIFGEYQ2UIZ5TS6BUHA2VMUZXO5UWS5CCLJMFKVLIJVSX2===

## Solution

```sh
┌──(kali㉿kali)-[~]
└─$ echo "IJZGKYLLIFGEYQ2UIZ5TS6BUHA2VMUZXO5UWS5CCLJMFKVLIJVSX2===" | base32 -d
BreakALLCTF{9x485VS7wiitBZXUUhMe}                                                                             
```

> Flag: `BreakALLCTF{9x485VS7wiitBZXUUhMe}`