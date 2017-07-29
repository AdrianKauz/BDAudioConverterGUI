BDAudioConverterGUI (Version 0.3.0.0)
=====================================

About:
-------------------------------------------------------------------------------------
BDAudioConverterGUI is inspired by BeLight,
which unfortunately is no longer being developed.

"BD" is the shortcut for BluRay and this format is the reason,
that i've written this GUI. Because a lot of series or movies on BluRay are having
the wrong pitch in the German-Audiostream like Fringe, Firefly, Prison Break etc..
So I needed a tool, which can do that for me and more and thought it's a good way
to write it self. So I can get some exercise in C#.

BDAudioConverterGUI uses eac3to, SoX, Aften, Dcaenc, Lame and NeroAACEnc to transcode
audiofiles from their format to another.
For this, it generates a Batch-file witch will be executed.
So eac3to can pipe the audiostream to sox and sox can pipe the audiostrem to
another sox-instance or to an output-instance like Aften, Lame etc.

BDAudioConverterGUI has an option to change the tempo and the pitch.
Downmixing from 5.1 to 2.0 is supported to.
It allows to convert the samplingrate, the bitdepth and encoding type before adding
effects and can change it back or to another setting, that fit an encoders input.


BDAudioConverterGUI comes without Nero AAC Encoder.
Only Nero is allowed to distribute the encoder.
You need to download it manualy from the official Nero website.
http://www.nero.com/deu/technologies-aac-codec.html
Just copy "neroAacEnc.exe" to the "neroaacenc" folder.


Supported Input-Files:
-------------------------------------------------------------------------------------
AC3, TrueHD, DTS, DTS-HD, WAV, FLAC

For DTS-HD: Eac3to needs Arcsoft DTS decoder files.
-> http://forum.doom9.org/showthread.php?p=1305698#post1305698


Supported Output-Files:
-------------------------------------------------------------------------------------
AAC, AC3, DTS, FLAC, MP3, WAV
For encodings to DTS: Sometimes it works, sometimes not. It's still experimental.


License:
-------------------------------------------------------------------------------------
BDAudioConverterGUI is created under the lincense of GNU GENERAL PUBLIC LICENSE V3.0.


Changes:
-------------------------------------------------------------------------------------
Changes can be found in the file: "changelog.txt"


BDAudioConverterGUI uses:
-------------------------------------------------------------------------------------
Aften: A/5s audio encoder           Version: Git 2012.02.03
dcaenc - command-line DTS encoder   Version: 2012.01.14 (compiled by LoRd_MuldeR)
eac3to - audio conversation tool    Version: 3.24
LAME MP3 Encoder                    Version: 3.99
MediaInfo                           Version: 0.7.52.0
Nero AAC Encoder                    Version: 1.5.4.0
SoX - Sound eXchange                Version: 14.4.0

Copyright (C) 2012 - 2017 Adrian Kauz