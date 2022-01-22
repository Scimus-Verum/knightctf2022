# Let's Walk Together

- **Category:** digital forensics
- **Points:** 50

## Challenge:

> Do you know anything about this image?

## Solution:

1. Extract the hidden files from the image using `binwalk`.
```
$ binwalk -e interesting_waves.png 

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             PNG image, 1024 x 768, 8-bit/color RGBA, non-interlaced
99            0x63            Zlib compressed data, best compression
69968         0x11150         Zip archive data, at least v1.0 to extract, name: Flag/
70031         0x1118F         Zip archive data, encrypted at least v1.0 to extract, compressed size: 37, uncompressed size: 25, name: Flag/flag.txt
70313         0x112A9         End of Zip archive, footer length: 22
```
2. In extracted files find the zip archive protected with password.
3. We can bruteforce the password using the `john` and `rockyou.txt` wordlist.
```
$ zip2john flag.zip hash.txt
$ john --wordlist=rockyou.txt hash.txt
```
4. Password is `letmein!`
5. Just unzip the protected zip archive with this password and get the flag.

**Flag:**`KCTF{BiNw4lk_is_h3lpfUl}`

