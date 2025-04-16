# Set Image Timeframe
```
exiv2 -M"set Exif.Image.DateTime 2015:10:24 20:00:00" 1.jpg
```
```
DateTime (Original) – When the image was taken (DateTimeOriginal)
Exif.Photo.DateTimeOriginal
Exif.Image.DateTime (legacy, may differ from DateTimeOriginal)

DateTimeDigitized – When the image was digitized (often same as DateTimeOriginal)
Exif.Photo.DateTimeDigitized

ModifyDate – When the file was last modified
Exif.Image.DateTime (sometimes used for modification time)
Exif.Photo.SubSecTimeOriginal (fractional seconds for DateTimeOriginal)

xmp:CreateDate – When the resource was created
xmp:ModifyDate – When the resource was last modified
xmp:MetadataDate – When metadata was last changed
photoshop:DateCreated (Adobe Photoshop-specific)

Iptc.Application2.DateCreated (Format: YYYYMMDD)
Iptc.Application2.TimeCreated (Format: HHMMSS±HHMM)
Iptc.Application2.DigitalCreationDate
Iptc.Application2.DigitalCreationTime
```
# Definition
>DateTimeOriginal is when the photo was taken.  
>DateTime is when it was further modified.

![image](https://github.com/user-attachments/assets/21c09e66-4d0c-4a15-bf3e-d777c49f1b94)

# Display exif, iptc, xmp metadata
exiv2 -pa imagefile
