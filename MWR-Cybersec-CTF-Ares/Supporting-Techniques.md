# 🧠 Supporting Techniques

## Overview
Supporting techniques used during exploitation phases.

---

## Steganography & Metadata Analysis
- Tools: Exiftool

The Ares' web application source code, contained a hidden comment that revealed a seperate server location: `/ares-possible-hq-locations`

<img width="600" height="355" alt="image" src="https://github.com/user-attachments/assets/4ed9630f-4b4b-4698-80df-78fa64443ba6" />

The referenced server hosted four jpg files with hidden infomation through the technique of steganography. The extracted hidden information within one of the JPG files
conatined the killswitch `MWR{Secret-Server-Is-Under-MtEverest}`

<img width="600" height="355" alt="image" src="https://github.com/user-attachments/assets/05aa7087-2180-4df7-82ae-952b321b0b3f" />



---

## Hash Cracking
- Tools: John the Ripper and supplied wordlist

Retrieved plaintext credentials used to unzip a protected archive file. 

<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/9a801b73-7e0c-4824-a553-c6cdde7815e9" />

File conatined the killswitch: MWR{Hacking-And-Cracking-Your-Way}.

<img width="400" height="90" alt="image" src="https://github.com/user-attachments/assets/bf6daa6f-c7a8-4a9c-ba7e-4ba26f82187c" />

---

## Encoding & Decoding
- Tools: CyberChef for Base64 and ROT13 decoding

 A small data fragment left behind by Ares was embedded with an encoded string `WkpFe05lcmYtdW5mLW4teHZ5eWZqdmdwdX0=` was identified as Base64 due to its format and padding character (`=`). After decoding it, the result was `ZJE{Nerf-unf-n-xvyyfjvgpu}`.
 This output was then identified as ROT13 encoded. After applying ROT13 decoding, the final flag was revealed as `MWR{Ares-has-a-killswitch}`.


---

## Summary
📌 These techniques supported primary exploitation tasks by revealing hidden data and credentials.
