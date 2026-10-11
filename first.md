
Name: Aditya Patil  
Event: COEP CyberCell FY Inductions Mini CTF  
  

## Overview

This repository contains step-by-step solutions, concepts, and methodology for the COEP CyberCell Mini CTF challenges. The writeup prioritizes practical command-line execution and digital forensics principles.



## Challenge Solutions

### Challenge 1- NOTHING TO SEE HERE
This was a very simple task, I just had to read the code 
*New learnings*- Encryption and Encoding are not the same

### Challenge 2- Mystery String
This was also a very easy task. I learned a new concept of Base64, it's basically a format of string which can be decoded very easily.<br>
*Tools Used*- Linux Terminal<br>
*New learnings*- Concept of Base64 and the command to decode it.
**echo -n "" | base64 -d**

### Challenge 3- Picture Perfect
*New learnings*- Digital image files often contain embedded metadata (EXIF) storing camera settings, author tags, and user comments.<br>
*Tool Used*- exiftool<br>
*Command*- exiftool photo.jpg<br>

### Challenge 04: Polite Robots
*New learnings*- Web crawlers follow the Robots Exclusion Standard (robots.txt) to identify disallowed paths. Hiding sensitive directories in robots.txt is an example of Security through Obscurity.<br>
*Tool Used*- <br>
*Methodology*- Checked /robots.txt to identify the restricted path (/s3cr3t-vault-7f3a/).
Navigated directly to <br>1.[https://cybercell.coeptech.ac.in/mini-ctf/s3cr3t-vault-7f3a/]<br>

### Challenge 05: Where Was This Taken?
*New Learnings*- When GPS metadata is stripped, visual indicators (architectural style, historical masonry, entrance arches, clock towers) are used to identify structures.
*Tool Used*-Google Image Search

### Challenge 06: Not What It Seems
*New Learnings*- Operating systems rely on file extensions, but actual file types are defined by magic byte headers. A **.jpg** extension can mask a hidden ZIP archive.<br>
*Command*-xxd mystery.jpg | head -n 2<br>unzip mystery.jpg<br>cat flag.txt
