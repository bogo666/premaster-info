# premaster-info

Using the Apple Digital Masters tools `afconvert` & `afinfo` on MacOS,
produce Apple Music "sound check" info and convert the output
into a summary useful for Audio Mastering Engineers, including:
crest factor, loudness range, and L & R peak locations in seconds.

Info about Apple Digital Masters is available here:
<https://www.apple.com/apple-music/apple-digital-masters/>

Copyright (c) 2024 Chris Foote.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.

## Example Output

```
$ ./premaster-info some_premaster.wav 
Sound Check Info for somme_premaster.wav
========================================

Bit Depth:            24
Sample Rate:          48 kbps
iLUFS:                -14.3081
Max Short-term LUFS:  -10.7634
Loudness Range:       8.4
True Peak:            -0.161641
Crest Factor:         -14.146459
                   Left           Right
Noise Floor:       -129.15        -129.03
Peak Location:     96.00 s        82.09 s
Max Power Loc:     43.20 s        43.20 s
```
