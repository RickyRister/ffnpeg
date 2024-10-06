# ffnpeg

Bash script containing common ffmpeg usages so I don't have to keep looking them up.

## Installation

Just copy or link `ffnpeg` to your `$PATH`.

## Usage

Run with `-h` to get usage info.

```
Usage: ffnpeg [options] <command> [options] file ...

Available Commands:
segment		Splits media into segments of a given length
split		Splits the media at the timestamp
trim		Trims media to the given timestamps
convert		Converts one or more files into a different format
concat		Concats one or more videos
extract		Extracts the audio or video from the video
musicvid	Combines an audio file with a static image
replace		Replaces the audio of a video

Universal Options:
-d		deletes input file afterwards (use with caution!)
-c		turn off -c copy (needed when converting between codecs)
-y		overwrite output files without asking
-p		runs ffmpeg on each file in parallel
-q		turn on quiet mode
-l PATH		sets location of output file
-n NAME		sets the output filename and extension
-s SUFFIX	adds a suffix to the output filenames
-e FORMAT	sets the output's extension. Will overwrite -n's extension
```

ffnpeg contains several commands.
You can run `-h` with those commands to get the usage info for them.

## Known Bugs

I'm pretty sure the `split` and `trim` commands don't work properly, 
and at this point I don't have any intent of fixing them.
(I wrote this script and didn't touch it for a year and now I have no idea how any of it works.)
Just don't use those commands I guess.
