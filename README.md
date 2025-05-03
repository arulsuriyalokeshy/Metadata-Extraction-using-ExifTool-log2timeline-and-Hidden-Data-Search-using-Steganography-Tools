# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps
- **Installation :**
```bash
   sudo apt update
   sudo apt install exiftool -y
   sudo apt install plaso -y
   sudo apt install steghide -y
   sudo apt install binwalk -y
 ```
- **Extract metadata from a file:**
```bash
  exiftool image path
  exiftool /home/kali/Desktop/test.jpg
```
- **Embed data**
  ```
  steghide embed -cf (image path) -ef (text file path)
  steghide embed -cf /home/kali/Desktop/test.jpg -ef /home/bharathi/Downloads/suriya.txt
  ```
- **Extract hidden data:**
  ```
  steghide extract -sf (imamge path)
  steghide extract -sf test.jpg
  ```
- **Using binwalk – for file analysis**  
  ```bash
   binwalk test.jpg
  ```
  
## OUTPUT:

### Extraction of Metadata using exiftool
![image](https://github.com/user-attachments/assets/8c4d990e-2e55-4ca7-8ca6-b03e802d7d3c)



### Data Embedding in Image
![image](https://github.com/user-attachments/assets/1ed085c5-e833-4c9e-ba36-56bace03ccb5)



### Extraction of hidden data
![image](https://github.com/user-attachments/assets/7fc93050-07ec-4d35-aba1-cccd5dde3a1e)


### Using binwalk – for file analysis
![image](https://github.com/user-attachments/assets/0de643e0-40a9-4586-82af-ed8d704cb8f1)


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

