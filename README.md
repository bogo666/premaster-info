# wave-sound-check

Using the Apple Digital Masters tools `afconvert` & `afinfo` on MacOS,
produce Apple Music "sound check" info, useful for Audio Mastering Engineers.

Info about Apple Digital Masters is available here:
<https://www.apple.com/apple-music/apple-digital-masters/>

Copyright (c) 2024 Chris Foote.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.

## Example Output

```text
$ ./wav-sound-check some_premaster.wav 
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
```
