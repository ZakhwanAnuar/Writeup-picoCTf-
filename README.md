## 📑 Table of Contents

- [Forensics](#forensics)
  - [Event Viewing](#event-viewing)
  - [Bitlocker 1](#bitlocker-1)
  - [Bitlocker 2](#bitlocker-2)
  - [Blast From The Past](#blast-from-the-past)
  - [Corrupted File](#corrupted-file)
  - [Dear Diary](#dear-diary)
  - [Disco 1](#disco-1)
  - [Disco 2](#disco-2)
  - [Disco 3](#disco-3)
  - [Flag In Flame](#flag-in-flame)
  - [Hidden In Plain Sight](#hidden-in-plain-sight)
  - [Hide Me](#hide-me)
  - [Lookey Here](#lookey-here)
  - [Operation Orchid](#operation-orchid)
  - [Red](#red)
  - [Redaction Gone Wrong](#redaction-gone-wrong)
  - [Riddle Registry](#riddle-registry)
  - [Scan Surprise](#scan-surprise)
  - [Secret Of The Polyglot](#secret-of-the-polyglot)
## Forensics
### Event Viewing

### Bitlocker 1

### Bitlocker 2

### Blast From The Past

### Corrupted File

### Dear Diary

First, I extracted the `.gz` file and opened it in **Autopsy** for analysis.

![Autopsy Analysis](Forensics/Dear-Diary/Autopsy.png)

While browsing the extracted files, I noticed a suspicious file named **`innocuous-file.txt`**.  

![Hxd Analysis](Forensics/Dear-Diary/Search.png)
I inspected this file using **HxD** and searched for its occurrences across the disk image.

![Hxd Analysis](Forensics/Dear-Diary/Final.png)

Each occurrence contained a **partial fragment of the flag**.  
By extracting all the fragments and combining them together, I was able to recover the full flag.

#### 🚩 Flag: picoCTF{1_533_n4m35_80d24b30}



### Disco 1

This challenge is so easy you. you just need to strings and grep the flag.

![string](Forensics/Disko1/Strings.png)

### Disco 2
First, the disk image was searched for flag strings:
![string](Forensics/Disko2/strings.png)

This returned multiple flags, so the hint was followed stating the correct flag is in the Linux partition.

The partition table was analyzed using:
![.](Forensics/Disko2/checking.png)

This showed the Linux partition starting at sector 2048 with 51200 sectors.

The Linux partition was extracted:
![.](Forensics/Disko2/extract.png)

Finally, the extracted image was searched for the flag:
![.](Forensics/Disko2/final.png)

#### 🚩 Flag: picoCTF{4_P4Rt_1t_i5_90a3f3d1}

### Disco 3

### Flag In Flame

### Hidden In Plain Sight

### Hide Me

### Lookey Here

### Operation Orchid

### Red

### Redaction Gone Wrong

### Riddle Registry

### Scan Surprise
### Event Viewing

**Category:** Forensics  
**Difficulty:** Easy  

#### 📜 Description
...

#### 🔍 Analysis
...

#### 🛠 Solution
...

#### 🚩 Flag


### Secret Of The Polyglot

