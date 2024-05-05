# WarmUp 1

## Description

請問 0x9D (16進制) 的 10進制值是多少?

請送出符合要求的 flag 格式。 例如: 答案如果為11，請送出 hsctf{11}

## Solution

```python
print(int("0x9D", 16))
```

```sh
┌──(kali㉿kali)-[~]
└─$ python 16to10.py 
157
```

> Flag: `hsctf{157}`
