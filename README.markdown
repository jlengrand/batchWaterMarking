# batchWaterMarking : a simple way to watermark all your pictures in one line

This repository contains the last version of my personal watermarking script. 

This script simply aims at adding an unobtrusive watermark to all images of an input folder and copy final images in an output folder.
The watermark is added with transparency effect in order to keep the image quality. 

The script should recognize all kinds of image formats, and correctly handle filenames with spaces and (most of) unusual characters.
In addition, the script is designed to automatically recognize whether your image is in portrait or lanscape mode. The watermark is put in a different corner to better visual results. 

The use of this script is pretty straightforward : 
```Bash
$ waterMark in_folder out_folder watermark_image
```

where :
- in_folder contains your input images
- out_folder will contain all new images
- watermark_image is the watermark you want to set on the image

The script also resize images in order to fit with [Piwigo](http://fr.piwigo.org/)'s default settings. (1024x768). This option should be set as optional soon.

## Installation

The only prerequisite to use this script is imagemagick : 
```Bash
$ apt-get install imagemagick
```

You do not need to install this script in any way. 
You can use it from anywhere as long as you use __absolute paths!__

A simple way to use waterMark from anywhere is to add it to your ~/bin folder; and give the script execution rights.
```Bash
$ chmod +x ~/bin/waterMark
```
This way, you will be able to run it directly in your terminal. 

## Next steps

Some more options should be added soon:
- Insert some contrast calculation in order to choose the best color from two different watermarks. This way, the watermark would always be visible
- Dynamically changechange the size of the watermark to avoid resizing input images
- Windows support ? ? ?
- Python version to avoid ugly bash ? 

Any idea is welcome

## Copyright

You are free to use and modify this script this script as you wish. 
Please just let my name on top of it and add yours after your modifications ;)

## Contact

I would enjoy having feedback if you use this script. 
Feel free to mail me for any comment or request. And let me know if you find bugs !

You can contact me at julien at lengrand dot fr, or on my [current website](http://www.lengrand.fr)

