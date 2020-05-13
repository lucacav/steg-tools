# steg-tools

This is a list of tools and resources for learning and experimenting with steganography and information hiding.  

# Tools

* [Exiftool](https://exiftool.org) is a Perl library and a command line application for the manipulation of metadata of different files, including EXIF, GPS, XMP, and ID3.

* Strings is part of the [binutils](https://www.gnu.org/software/binutils/) and it is pre-installed in many unix OSes. On macOS is part of Xcode command line tools and can be installed with: `xcode-select --install`. 
Strings can be used to find printable strings (i.e., ASCII strings) in binary and other files. 

* [binwalk](https://github.com/ReFirmLabs/binwalk) is a simple (yet powerful) tool for binary files. Among the various use, it can be used to find embedded or appended files or blocks of executable code. On Linux can be installed with `apt-get install binwalk`, while on macOS is available through [Homebrew](https://brew.sh/index_it) with `brew install binwalk`. 

* [zsteg](https://github.com/zed-0xff/zsteg) can be used to detect data within PNG and BMP images, which can be embedded by using steganography. It can be installed via `gem install zsteg` and provides different extraction methods. With the flag `-a`, it can be used to search an image for hidden content by using all the known methods, or it can be tweaked to search for specific combinations of R, G, B, A channels.


* [Steghide](http://steghide.sourceforge.net) is a tool for hiding data in different media files (i.e., audio and image). Embedded data can be compressed, encrypted and protected with a checksum to verify the integrity of the message. 

* zbarimg is part of the [ZBar](http://zbar.sourceforge.net) suite of tools for scanning and reading barcodes and QRcodes for different sources (e.g., videos and images). It also offers a Python API, which allows to easily integrate the scanning functionalities in scripts to automate the analysis process. 


# Further Reading

* [steg-in-the-wild](https://github.com/lucacav/steg-in-the-wild) a list of real-world attacks leveraging some form of steganography or information hiding.

* [SteganoCC](http://steganocc.gforge.inria.fr) is a set of covert channels (i.e., hidden communication paths implemented by using information hiding) acting between two Android processes. This technique is at the basis of the *colluding applications threat*, which can be used to exfiltrate data between two isolated processes. 
