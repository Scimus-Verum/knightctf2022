# Unzip Me

- **Category:** misc
- **Points:** 100

## Challenge:

> Can you unzip the file ?

## Solution:

1. Extract `unzipme` file from `unzipme.tar.gz` archive.
```
$ tar -xf unzipme.tar.gz
```
2. Read strings from `unzipme` file.
```
$ strings unzipme
lfgat.txCKFTs{_OOy_uWsPa3P_DHt_e1f3L
lfgat.txKP
```
3. The flag format is `KCFT{...}`, so we need to swap each letter in each pair in that string `CKFTs{_OOy_uWsPa3P_DHt_e1f3L}`.

**Flag:**`KCTF{sO_yOu_sWaPP3D_the_f1L3}`

