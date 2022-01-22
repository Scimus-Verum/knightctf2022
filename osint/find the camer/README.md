# Find The Camera

- **Category:** osint
- **Points:** 100

## Challenge:

> Can you find the manufacturer and the model number of the camera that took the picture of this bus?

## Solution:
![image](https://user-images.githubusercontent.com/74129817/150630284-dc4ae2d7-caf0-484e-ae25-b4c7e1bac1ad.png)
1. On the image we can see the author of it: `JenCh012`
2. If you google author name, you can find this link: https://fotobus.msk.ru/author/2739/
3. On the original image we can see logos of 'Diddeleng'. Wikipedia says that it is a commune with town status in southern Luxembourg.
4. So we need to find `JenCh012`'s bus images related to Luxembourg. To use a search option on this site we need to register an account.
5. We can search buses by numeric code, our bus has `206` value. 
6. As a result, we get this link: https://fotobus.msk.ru/photo/267442/?vid=204172
![image](https://user-images.githubusercontent.com/74129817/150630213-7c4ed4ae-88d3-47a4-af7c-63c71f7236f1.png)

**Flag:**`KCTF{SONY_DSC_S980}`

