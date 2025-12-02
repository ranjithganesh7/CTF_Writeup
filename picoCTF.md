## PICO CTF

| Challenge | Category | Description | Core Concept & Tools Used | Solution Summary |
| :--- | :--- | :--- | :--- | :--- |
| **Riddle Registry** | Forensics/Misc | Flag hidden in a PDF file's metadata. | **Metadata Analysis** & **Base64 Decoding** | Used adobe pdf viewer to view properties found the metadata, found a Base64 string, and decoded it using **https://www.base64decode.org/**. |
| **Log Hunt** | Forensics/Log | Flag parts scattered and repeated across a large server log file. | **Log Reconstruction** & **Data Processing** | Uploaded the large log file to **Gemini**, prompting it to identify, filter, and correctly order the unique flag fragments for reconstruction. |
| **Hidden in Plain Sight** | Steganography | Flag hidden inside a JPG image using steganography. | **Steganography** & **Password Discovery** | Used **https://www.dcode.fr/strings-extractor** to find the hidden password (`pAzzword`) in the metadata, then extracted the flag from the image using **https://futureboy.us/stegano/decinput.html**. |
| **Flag in Flame** | Forensics/Encoding | Large encoded block of text in a log file hiding a PNG image with a hex code. | **Base64/Hex Decoding** & **File Signature Analysis** | Identified the block as Base64, decoded it to a PNG using **[Base64 to PNG Converter](https://base64.guru/converter/decode/image/png)**, and then hex decoded the visible code using **[Hex Decode](https://www.convertstring.com/EncodeDecode/HexDecode)** to get the flag. |

***
