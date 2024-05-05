# Base64

## Description

編碼與解碼是資訊領域日常都在使用的技術，如Ascii、Base64、Base32各有其適用處，請問你對Base64編碼與解碼的技術了解嗎?

你知道如何解碼下列資料嗎: QnJlYWtBTExDVEZ7NTN1c1pRM2hXVzI1ZGNoWjdkWGV9

## Solution

```sh
┌──(kali㉿kali)-[~]
└─$ echo QnJlYWtBTExDVEZ7NTN1c1pRM2hXVzI1ZGNoWjdkWGV9 | base64 -d
BreakALLCTF{53usZQ3hWW25dchZ7dXe}
```

> Flag: `BreakALLCTF{53usZQ3hWW25dchZ7dXe}`
