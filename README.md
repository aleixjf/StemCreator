# StemCreator

StemCreator is a Stem file generator. Convert any supported audio file into a Stem.

The resulting Stem file will contain the original audio file splitted into four musical elements – bass, drums, others (piano, synths, other meoldic elements, etc.) and vocals. This will allow anyone to have more control over the music they play, bringing anyone's creativity and possibilities one step further.

StemCreator is inspired by `stemgen`, written by @alexdelafosse, and uses `jo` to create a JSON readable file which contains the tags of the original audio file. It then uses `spleeter` to separate the original file into 4 stems and `ni-stem` to create the Stem file from the 4 separated stems and the JSON file.

Really looking forward for someone who knows about swift or creating mac apps to pick up this project and create an interface for it. I did try by myself but was very unsuccessful.

## Why?

> "It's no secret that I'm fully behind the approach to encourage individuality in creativity and for artists to play differently. Stems is a new format that mirrors my constant quest for spontaneity to drive the art of performance forwards. I hope that releasing my album From My Mind To Yours in this format, mastered by LANDR, inspires others to support the approach and bring even more flexibility to the art of DJing amongst its most progressive supporters." – Richie Hawtin

As @alexdelafosse indicates, stems are fun to play with, but nobody's releasing them. Furthermore, DJ softwares like VirtualDJ 2021 or DJay Pro have just released updates for their softwares which also use AI to separate audio files to provide more tools to get more creative. NI still doesn't have this, and maybe never will (hopefully I'm wrong, of course), but this will help anyone to create their own stems and use them in Traktor's mature approach for this (they have been working with Stems and implementing them in Software/Hardware since they released them in 2014), Stem Decks.

## Requirements

- spleeter https://github.com/deezer/spleeter
- ffmpeg https://www.ffmpeg.org (required for spleeter too)
- ni-stem (provided in this repo or available at https://www.stems-music.com/stems-is-for-developers)
- jo https://github.com/jpmens/jo

## Installation (Recommended)

1. Install `spleeter` (refer to the GitHub link for installation instructions, the following might be incomplete or incorrect)
    1. Download and install miniconda: https://docs.conda.io/en/latest/miniconda.html
    2. Install miniconda
    3. Open the terminal/command line and write/paste the following: conda install -c conda-forge spleeter

2. Install `jo` (refer to the GitHub link for installation instructions, the following might be incomplete or incorrect)
    1. Download the .zip folder
    2. Open the terminal/command line and write/paste the following: brew install jo

3. Download the StemCreator.zip file of this project, and decompress it to the folder you want.
As a result, you'll have a folder called StemCreator inside the GitHub folder, and everything should work fine.

## Usage (in macOS, haven't tested it on Windows)

1. Open terminal/command line
2. Navigate inside the StemCreator folder with the terminal. For instance, if you placed it in the Desktop, run the following command: cd /Users/YOURUSERNAME/Desktop/StemCreator
3. Run the following command to create your stems: ./StemCreator -i "FOLDER OR FILE PATH"
4. Once the process is finished, you'll find the Stem or Stems in the same directory where the audio file was/inside the specified directory, inside a new folder called "STEMS"-

## Disclaimer

If you plan to use StemCreator on copyrighted material, make sure you get proper authorization from right owners beforehand.

## License

MIT License. I do not own any of the rights regarding spleeter, jo, ni-stems or whatever. This is just a script which uses different preexisting scripts. If anyone believes I'm infringing their copyright/license, please let me know. I only want to help the community :)
