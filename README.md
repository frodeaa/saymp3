# saymp3

A text to mp3 tool

    usage: saymp3 [-v voice] [-r rate] [-V quality] [-o output] [file...]

    options:
      -v, -v=alex        specify the voice to be used.
      -r, -r=200         speech rate to be used, in words per minute.
      -V, -V=4           quality settings for VBR, 0=highest, 9=smaller file
      -o, o=out.mp3      output filename
      -h                 show help


## Example

    cat book.txt | saymp3 -v=alex r=200 -V=4 -o book.mp3

## Install

    install -m 0755 saymp3 /usr/local/bin