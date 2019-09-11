# Chrome slow motion bug

This repository contains a proof-of-concept showing that Chrome 76 plays back video in
SLOW MOTION instead of dropping frames, when rendering the video on an WebGL canvas.

In addition, the video element reports the WRONG timestamps, so what you see on screen
cannot be correctly correlated with the time of the video!

This leads to the case where Chrome can not be used for creating professional video tools utilizing
WebGL + video playback because the video is in slow motion and the timestamps are not accurate.

Operating system: macOS.
