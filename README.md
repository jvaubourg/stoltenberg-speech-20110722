# Prime Minister's Stoltenberg press conference - Norway, 22 July 22.00

## Historical Speech

The same evening after the [2011 Norway attacks](https://en.wikipedia.org/wiki/2011_Norway_attacks), the Prime Minister's Stoltenberg read an historical speech.

He said:

> We must show [...] that the answer to violence is even more democracy.

We should help him to spread the word.

Please, as much as possible, do not link this page or other one, but copy the videos and the subtitles on personal servers and various video platforms. The original video is currently too hard to find. We need to replicate it, for more availability, even when sources disappeared.

If you speak a language not available in the subtitle files, feel free to propose your contribution!

## Subtitles
### English

* [subtitles/stoltenberg_2011-07-22.en.srt](subtitles/stoltenberg_2011-07-22.en.srt)

This translation corresponds to the [official speech translation](https://www.regjeringen.no/en/aktuelt/transcript-from-prime-minister-stoltenbe/id651770/), from the Norwegian government.

### French

* [subtitles/stoltenberg_2011-07-22.fr.srt](subtitles/stoltenberg_2011-07-22.fr.srt)

This translation is an homemade work, based on the [English version](https://www.regjeringen.no/en/aktuelt/transcript-from-prime-minister-stoltenbe/id651770/) and the proposition found on [this blog](http://krn-defouloir.blogspot.fr/2011/07/jens-stoltenberg-sadresse-aux.html).

## Videos
### Origins

The original video was taken from [VGTV](http://www.vgtv.no/#!/video/42403/se-stoltenberg-snakke-om-bombeangrepet), thanks to `youtube-dl`:

```
% youtube-dl http://www.vgtv.no/#!/video/42403/se-stoltenberg-snakke-om-bombeangrepet
```

The syncing of the subtitles was done, with the help of [this other video](https://www.youtube.com/watch?v=VwdZs0GqWHA).

### Available formats

* [WEBM](videos/stoltenberg_2011-07-22.webm)
* [OGV](videos/stoltenberg_2011-07-22.ogv)
* [MP4](videos/stoltenberg_2011-07-22.mp4)

The downloaded FLV video file was converted to these 3 standard HTML5 formats thanks to `ffmpeg`:

```
% ffmpeg -i stoltenberg_2011-07-22.flv -b:v 1500k -vcodec libvpx -acodec libvorbis -ab 160000 -f webm -g 30 stoltenberg_2011-07-22.webm
% ffmpeg -i stoltenberg_2011-07-22.flv -b:v 1500k -vcodec libtheora -acodec libvorbis -ab 160000 -g 30 stoltenberg_2011-07-22.ogv
% ffmpeg -i stoltenberg_2011-07-22.flv -b:v 1500k -vcodec libx264 -strict -2 -preset medium -g 30 stoltenberg_2011-07-22.mp4
```
