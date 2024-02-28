# Mod 26

## Description

Cryptography can be easy, do you know what ROT13 is? `cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_Ncualgvd}`


## Solution

將每一字元的 $ASCII$ 加 13 在模 26

### Python
```python
s = "cvpbPGS{arkg_gvzr_V'yy_gel_2_ebhaqf_bs_ebg13_Ncualgvd}"
res = ""
for c in s:
    if c >= 'a' and c <= 'z':
        res += chr((ord(c)+13-ord('a'))%26+ord('a'))
    elif c >= 'A' and c <= 'Z':
        res += chr((ord(c)+13-ord('A'))%26+ord('A'))
    else:
        res += c
print(res)
```

### Output
```txt
picoCTF{next_time_I'll_try_2_rounds_of_rot13_Aphnytiq}
```


> flag : `picoCTF{next_time_I'll_try_2_rounds_of_rot13_Aphnytiq}`
