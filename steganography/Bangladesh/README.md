# Bangladesh
- **Category:** steganography
- **Points:** 100

## Challenge:

> My friend John was interested to know my country . He told me that to give him some images and articles about my county . I gave him some images and articles. In one image I provided some hidden data but he can not find hidden data . I told him Always remember 3 number sum equal to a game-changer. but he can not find hidden data . For that reason, I gave him that game-changer key.

## Solution:
1. Download the `Bangladesh.jpg` image file and use `steghide` on it.
```
$ steghide --info Bangladesh.jpg
"Bangladesh.jpg":
  format: jpeg
  capacity: 8,4 KB
Try to get information about embedded data ? (y/n)
```
2. File has hidden data, but we don't know the password. So I decided to bruteforce the password using `stegseek` and `rockyou.txt` wordlist.
```
$ stegseek Bangladesh.jpg rockyou.txt
StegSeek 0.6 - https://github.com/RickdeJager/StegSeek

[i] Found passphrase: "2262"B)           
[i] Original filename: "not_real".
[i] Extracting to "Bangladesh.jpg.out".
```
3. Just open the `Bangladesh.jpg.out` file and you can see the flag.

**Flag:**`KCTF{Do_We_Remember_Cicada_3301}`
