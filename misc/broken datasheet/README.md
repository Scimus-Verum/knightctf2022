# Broken Datasheet

- **Category:** misc
- **Points:** 100

## Challenge:

> One of my friend sent me an important datasheet to me. But the sheet seems broken. Can you please help me to recover or read the datasheet.

## Solution:

1. Extract the hidden files from `Broken Datasheet.xlsx` using `binwalk`.
```
$ binwalk -e Broken\ Datasheet.xlsx
```
2. In extracted files you can find another `Broken Datasheet.xlsx` file. Again extract all files from it.
3. After open the `sharedStrings.xml` file in `xl` folder and you can find the flag.
![image](https://user-images.githubusercontent.com/74129817/150630483-8097824d-e903-4089-af2c-d433ff300864.png)

**Flag:**`KCTF{XLSX_Fil3$_4R3_Actually_0n3_Kind_0f_Zip_Fil3}`

