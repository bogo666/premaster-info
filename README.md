# premaster-info

Using the Apple Digital Masters tools `afconvert` & `afinfo` on MacOS,
produce Apple Music "sound check" info and convert the output
into a summary useful for Audio Mastering Engineers, including:
crest factor, loudness range, and L & R peak locations in seconds.

Info about Apple Digital Masters is available here:
<https://www.apple.com/apple-music/apple-digital-masters/>

It also depends on the 'sox' audio conversion utility, which I would
recommend you install with homebrew:

```shell
brew install sox
```

Copyright (c) 2024 Chris Foote.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.

## Example Output

```text
$ ./premaster-info some_premaster.wav 
Sound Check Info for somme_premaster.wav
========================================

Approx Length:        00h:02m:50.88s
Bit Depth:            24
Sample Rate:          48 kbps
iLUFS:                -14.3081
Max Short-term LUFS:  -10.7634
Loudness Range:       8.4
True Peak:            -0.161641
Crest Factor:         -14.146459
Max Momentary LUFS:   -8.95639
                   Left               Right
Noise Floor:       -129.15            -129.03
Peak Location:     00h:01m:36.00s     00h:01m:22.09s
Max Power Loc:     00h:00m:43.20s     00h:00m:43.20s

Peak Amplitude
==============
LEFT    True Peak:   -5.24877
        Max ST LUFS: -16.6525
RIGHT   True Peak:   -0.206122
        Max ST LUFS: -13.13
Peak Power
==========
LEFT    True Peak:   -0.175676
        Max ST LUFS: -15.1847
RIGHT   True Peak:   -0.175676
        Max ST LUFS: -15.1847
```
