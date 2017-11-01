# PrettyIndex

PrettyIndex is a responsive, coloured kind of Metro theme built to enhance the experience of browsing web directories. It uses the `mod_autoindex` Apache module, some CSS to override the default style and—some JS & JQuery—to alter the generated table structure of a directory listing.

![alt screenshot](https://github.com/martinlb/martinlb.github.io/blob/master/img/afterPrettyIndex.png)

## Installation

PrettyIndex requires an Apache(2.2.11+) enabled HTTP server.

Let's assume you have a folder named `share` in your server root directory (the path thus being `http://mywebsite.com/share`) that you'd like to use as your listing directory:

* [Download](https://github.com/martinlb/PrettyIndex/archive/master.zip) and unzip PrettyIndex
* Copy and paste the contents of the `/PrettyIndex` folder to your `/share` folder.
* Edit `.htaccess` in `/share` and replace `/share/...` with the relative path from the server root.
* You can also add file descriptions at the end of the `/share/.htaccess` file.
* [Treat yo'self](http://25.media.tumblr.com/tumblr_lw7q28y0Mz1qanm80o1_500.gif), you're done.

## PrettyIndex theme

If you'd like to alter the default PrettyIndex theme, look in the `/PrettyIndexTheme` folder and you'll find the following files:

* `header.html`
* `footer.html`
* `style.css`

Edit these as you would any other HTML or CSS file.

## Icons

The PrettyIndex theme has icons in place for the following extensions:

    .7z .aac .aif .aifc .aiff .ape .asf .asx .au .avi .bmp .bz2 .cab .css .csv .doc  .docx
    .f4a .f4b .f4p .f4v .flac .flv .gif .gz .htm .html .ico .iff .it .jar .java .jpe .jpeg .jpg
    .js .m4a .m4v .mid .mkv .mod .mov .mp3 .mp4 .mpa .mpg .odp .oga .ogg .ogv .pdf .php .png
    .pot .potm .potx .pps .ppsm .ppsx .ppt .pptm .pptx .psd .ra .rm .s3m .srt .swf .tar .tif
    .tiff .tsv .txt .vob .wav .wma .wmv .xcf .xlam .xlr .xls .xlsm .xlsx .xltm .xltx .xm .zip
    
## Troubleshooting

Make sure the options set in `.htaccess` files of PrettyIndex can actually be changed. This means that you need to allow to ovveride the used options in your apache configuration of the directory PrettyIndex used with: `AllowOverride Indexes`

Find more information in the in the [apache documentation](https://httpd.apache.org/docs/2.2/de/mod/core.html).

## Credits

PrettyIndex owes its existence to the amazing [apaxy](http://adamwhitcroft.com/apaxy/) by [Adam Whitcroft](https://twitter.com/adamwhitcroft).

[Font Awesome](http://fontawesome.io/) are used as icons in PrettyIndex.

[Bootstrap](http://getbootstrap.com/) is used to make PrettyIndex responsive.

[JQuery](https://jquery.com/) is used to get total control of Apache autoindex listing.
