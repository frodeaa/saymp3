# saymp3 -- tts mp3

A text to mp3 tool

    usage: saymp3 [-s voice] [-r rate] [-q quality] [-o output] [file...]

    create mp3 audio files from text input

    options:
      -s, -s alex        specify the voice to be used.
      -r, -r 175         speech rate to be used, in words per minute.
      -q, -q "-q 0 -v -V 9 -mm -B 32"
                         quality settings, see lame options (lame --longhelp)
      -o, -o out.mp3     output filename
      -v                 show version
      -h                 show help


## Example

    cat book.txt | saymp3 -s alex -r 175 -o book.mp3

## Dependencies

 - lame
 - mp3Val

You can install the dependencies with homebrew:

    $ brew install lame mp3val


## Install

    install -m 0755 saymp3 /usr/local/bin
