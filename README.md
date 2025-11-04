It work this way.
NW.JS click trough transparent option doesn't work on Linux, it only makes app click trough forever.
So using this module, i created virtual cursor inside the app, that listens to libinput (has to be modified if you have trackpad + mouse)
When virtual cursor is over non transparent region, the nw.js window is no longer click trough, otherwise it's click trough.
Nw.JS has to run in X11 which usally is default. Main issue is tracking cursor position on wayland
