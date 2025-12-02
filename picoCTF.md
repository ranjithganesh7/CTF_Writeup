## PICO CTF

| Challenge | Category | Description | Core Concept & Tools Used | Solution Summary |
| :--- | :--- | :--- | :--- | :--- |
| **Riddle Registry** | Forensics/Misc | Flag hidden in a PDF file's metadata. | **Metadata Analysis** & **Base64 Decoding** | Used `exiftool` (or online viewer) to extract metadata, found a Base64 string, and decoded it using **https://www.base64decode.org/**. |
| **Log Hunt** | Forensics/Log | Flag parts scattered and repeated across a large server log file. | **Log Reconstruction** & **Data Processing** | Uploaded the large log file to **Gemini**, prompting it to identify, filter, and correctly order the unique flag fragments for reconstruction. |
| **Hidden in Plain Sight** | Steganography | Flag hidden inside a JPG image using steganography. | **Steganography** & **Password Discovery** | Used **https://www.dcode.fr/strings-extractor** to find the hidden password (`pAzzword`) in the metadata, then extracted the flag from the image using **https://futureboy.us/stegano/decinput.html**. |

***
