pandoc /home/dale/Documents/Epiphany-7-draft-1.md -o ebook.epub -t epub3 --toc --toc-depth=3 --split-level=2 --epub-cover-image=cover.jpg --css=pandoc.css --epub-metadata=metadata.xml

cf/ https://medium.com/@blittler/markdown-formatting-for-ebooks-including-kindle-kobo-and-nook-ee15a5992bc

pandoc /home/dale/Documents/Epiphany-7-draft-1.md -o ebook.epub -t epub3 --toc --toc-depth=3 --split-level=2 --epub-cover-image=cover.jpg --css=pandoc.css --epub-metadata=metadata.xml --defaults

working version:

[source file] -o [render file] -t epub3 --toc --toc-depth=3 --split-level=2 --epub-cover-image=/home/dale/.pandoc/cover.jpg --css=/home/dale/.pandoc/calibre-reader-2.css
