# FileD
- **Category:** steganography
- **Points:** 25 

## Challenge:

> Can you see everything?

## Solution:

1. Determine the type of `filed.zip` file.
```
$ file filed.zip
filed.zip: Zip data (MIME type "application/x-krita"?)
```
2. We can see that zip archive is Krita file, so convert it to `kra` file.
```
$ mv filed.zip filed.kra
```
3. Open the file with Krita and find `ctf.png` image file, it has our flag.
![image](https://user-images.githubusercontent.com/74129817/150627156-ef2bc661-e45f-4603-a380-e198781bec26.png)

**Flag:**`KCTF{W00_n1ce_you_got_me}`





