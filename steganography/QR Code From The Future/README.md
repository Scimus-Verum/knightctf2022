# QR Code From The Future
- **Category:** steganography
- **Points:** 100

## Challenge:

> The following file was found in a device from a crashed UFO. Can you solve that mystery?

## Solution:
![QR_Code_From_The_Future](https://user-images.githubusercontent.com/74129817/150627988-14a62871-8825-481d-a2b5-df41d92b1d2e.gif)

1. Split gif file into individual frames, I used this site: https://ezgif.com/split.
2. Download all frames and scan each one using `zbarimg`.
```
$ zbarimg *.gif
```
3. As a result, we get the following line:`}pvznalq_bg_pvgngf_zbes_qriybir_gbt_rqbp_ED{SGPX`
4. It's just a substitution cipher (ROT13): `}cimanyd_ot_citats_morf_devlove_tog_edoc_RQ{FTCK`
5. Reverse text: `KCTF{QR_code_got_evolved_from_static_to_dynamic}`

**Flag:**`KCTF{QR_code_got_evolved_from_static_to_dynamic}`






