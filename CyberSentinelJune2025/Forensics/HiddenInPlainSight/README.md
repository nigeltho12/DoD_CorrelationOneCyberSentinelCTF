🕵️ Hidden in Plain Sight
Category: Forensics
Points: 50
Status: ✅ Completed

Challenge Description
An innocuous image hid more than met the eye. The task was to uncover any hidden or steganographic clues embedded within the image file.

Approach

Used exiftool to analyze metadata.

Ran strings, binwalk, and viewed the image in CyberChef for hidden encodings.

Found a base64 string that decoded into the flag.

Roadblocks

Initial tools like zsteg and steghide gave no useful output.

Success came via CyberChef’s decoding utilities.

Flag
C1{REDACTED}
