pdftesseract
============

Pdftesseract is a perl script that uses imagemagick and tesseract to
extract plain text from a scanned pdf-file and writes it to STDOUT. It
has some support for some image preprocessing (selecting a page rage,
multicolumn documents) and runs in parallel.

INSTALLATION
============

Clone the archive and make sure you have perl, imagemagick and
tesseract installed. Make also sure that you have the tesseract
language data for your target languages. After that, you can call it with

	perl pdftesseract --language eng+deu example.pdf > example.txt

For further details of its usage execute

	perl pdftesseract --help
   
If you make pdftesseract executable (chmod 755 pdftesseract on UNIX)
and copy or symlink it somewhere in your $PATH, you should be able to
call pdftesseract simply by typing

	pdftesseract --language eng example.pdf
