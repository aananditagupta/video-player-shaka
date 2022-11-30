# FX Video Player Challenge

The solution is a working video player with:

- very basic custom controls, play/pause button and ff/rewind button
- ability to load/destroy player (simulating a normal playback session)
- multiple subtitles support
- multiple audio track support
- custom subtitle displayer


## Tasks from the Challenge
1. Add the functionality to jump 5s with the ff/rewind buttons. The buttons and the handlers for the click events are already set up for you.

- **resources:**
    - https://developer.mozilla.org/en-US/docs/Web/API/HTMLMediaElement/currentTime
<br>
2. The UI has elements to show the current time and the duration of the video, but they don't get updated and just show 00:00. Fix it!

- **tips:**
    - use `parseTime()` method from `utils.js` to parse the time to the correct `mm:ss` format
- **resources:**
    - https://developer.mozilla.org/en-US/docs/Web/API/HTMLMediaElement/duration
    - https://developer.mozilla.org/en-US/docs/Web/API/HTMLMediaElement/timeupdate_event
    - https://developer.mozilla.org/en-US/docs/Web/API/HTMLMediaElement/currentTime
<br>
3. Add multiple audio tracks support. Do a very similar thing to what we did with the subtitle tracks, but this time with the audio tracks.

- **tips:**
    - use the method `getAudioLanguages()` from Shaka Player in a very similar fashion to how we use Shaka's `getTextTracks`
    - You'll find some guidance in `shaka.js` on the steps you must follow to pull the audio tracks from Shaka Player and push them to the UI.
- **resources:**
    - https://shaka-player-demo.appspot.com/docs/api/shaka.Player.html
