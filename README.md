# Prime Minister's Stoltenberg press conference - Norway, 22 July 22.00

## Historical Speech

The same evening after the [2011 Norway attacks](https://en.wikipedia.org/wiki/2011_Norway_attacks), the Prime Minister's Stoltenberg read an historical speech.

He said:

> We must show [...] that the answer to violence is even more democracy.

We should help him to spread the word.

Please, as much as possible, do not directly link this page, but copy the video and subtitle files on personal servers or/and various video platforms. The original video is currently too hard to find: we need to replicate it, for ensuring its availability in the future.

If you speak a language not currently available in the subtitle files, feel free to propose your contribution.

## Subtitles

You can use Subtitle Editor (package `subtitleeditor` on Debian/Ubuntu) for composing a new translation, and this [online converter](https://atelier.u-sub.net/srt2vtt/) for converting SRT files to VTT ones.

### English

* [subtitles/stoltenberg_2011-07-22.en.srt](subtitles/stoltenberg_2011-07-22.en.srt)

This translation corresponds to the [official English version](https://www.regjeringen.no/en/aktuelt/transcript-from-prime-minister-stoltenbe/id651770/) of the speech, provided by the Norwegian government.

The syncing with the video was done with the help of [this other video](https://www.youtube.com/watch?v=VwdZs0GqWHA).

### French

* [subtitles/stoltenberg_2011-07-22.fr.srt](subtitles/stoltenberg_2011-07-22.fr.srt)

This translation is based on the [English version](subtitles/stoltenberg_2011-07-22.en.srt), and the proposition found on [this blog](http://krn-defouloir.blogspot.fr/2011/07/jens-stoltenberg-sadresse-aux.html).

## Videos
### Origins

The original video was taken from [VGTV](http://www.vgtv.no/#!/video/42403/se-stoltenberg-snakke-om-bombeangrepet) in FLV format, thanks to `youtube-dl`:

```
% youtube-dl http://www.vgtv.no/#!/video/42403/se-stoltenberg-snakke-om-bombeangrepet
```

### Available formats

* [WEBM](videos/stoltenberg_2011-07-22.webm)
* [OGV](videos/stoltenberg_2011-07-22.ogv)
* [MP4](videos/stoltenberg_2011-07-22.mp4)

The original FLV file was converted to these 3 standard HTML5 formats, thanks to `ffmpeg`:

```
% ffmpeg -i stoltenberg_2011-07-22.flv -b:v 1500k -vcodec libvpx -acodec libvorbis -ab 160000 -f webm -g 30 stoltenberg_2011-07-22.webm
% ffmpeg -i stoltenberg_2011-07-22.flv -b:v 1500k -vcodec libtheora -acodec libvorbis -ab 160000 -g 30 stoltenberg_2011-07-22.ogv
% ffmpeg -i stoltenberg_2011-07-22.flv -b:v 1500k -vcodec libx264 -strict -2 -preset medium -g 30 stoltenberg_2011-07-22.mp4
```

### Displaying on a website

Please, download the 3 files available in [videos/](videos/) and the VTT files available in [subtitles/](subtitles/), and insert this HTML5 snippet in your webpage:

```
<video width="512" height="288" preload="metadata" tabindex="0" controls>
  <source type="video/webm" src="stoltenberg_2011-07-22.webm">
  <source type="video/mp4" src="stoltenberg_2011-07-22.mp4">
  <source type="video/ogv" src="stoltenberg_2011-07-22.ogv">
  <track label="Français" kind="subtitles" srclang="fr" src="stoltenberg_2011-07-22.fr.vtt" default>
  <track label="English" kind="subtitles" srclang="en" src="stoltenberg_2011-07-22.en.vtt">
  <button id="subtitles" type="button" data-state="subtitles">CC</button>
  Please, use a recent browser to view this video.
</video>
```
