# saymp3

A text to mp3 tool

    usage: saymp3 [-s voice] [-r rate] [-q quality] [-o output] [file...]

    create mp3 audio files from text input

    options:
      -s, -s=alex        specify the voice to be used.
      -r, -r=175         speech rate to be used, in words per minute.
      -q, -q=4           quality settings for VBR, 0=highest, 9=smaller file
      -o, o=out.mp3      output filename
      -v                 show version
      -h                 show help


## Example

    cat book.txt | saymp3 -s=alex r=175 -q=4 -o book.mp3

## Install

    install -m 0755 saymp3 /usr/local/bin
