It works this way.
NW.JS click trough transparent option doesn't work on Linux, <br>
it only makes app click trough forever.<br>
So using this module, i created virtual cursor inside the app, <br>
that listens to libinput (has to be modified if you have trackpad + mouse)<br>
When virtual cursor is over non transparent region, the nw.js window is no longer click trough,<br>
otherwise it's click trough. Nw.JS has to run in X11 which usally is default.<br>
Main issue is tracking cursor position on wayland, is reason why this was created
