+++
title = "Chunking"
date = "2019-05-14"
description = "Bite off what you can chew"
draft = false
+++

<img src="/images/coffee_shop.jpg" alt = "Seylou Bakery" style="width:642px;height:442px;">
## Need to Break Apart Large File?

Munching on this carrot cake from Seylou Bakery in D.C., I thought about the time I had to deal with a large .jar file for which I had to break apart.
Linux: <br>

$ split --help <br>
Usage: split [OPTION] [INPUT [PREFIX]] <br>
Output fixed-size pieces of INPUT to PREFIXaa, PREFIXab, ...; default<br>
size is 1000 lines, and default PREFIX is `x'.  With no INPUT, or when INPUT<br>
is -, read standard input.<br>

Mandatory arguments to long options are mandatory for short options too.<br>
  -a, --suffix-length=N   use suffixes of length N (default 2)<br>
  -b, --bytes=SIZE        put SIZE bytes per output file<br>
  -C, --line-bytes=SIZE   put at most SIZE bytes of lines per output file<br>
  -d, --numeric-suffixes  use numeric suffixes instead of alphabetic<br>
  -l, --lines=NUMBER      put NUMBER lines per output file<br>
  <br>
  --verbose               print a diagnostic to standard error just<br>
                          before each output file is opened
      --help     display this help and exit<br>
      --version  output version information and exit<br>
      
      
    split -l 10000 filename

split a large file by lines' <br>
The output is the filename00, filename01, etc...



