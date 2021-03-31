# Wowza_Audiorepeater2
Original developed by Shamrock. This repository is just for securing the files and documentation

# Objective
Using the Audiorepeater as a module within Wowza it is possible to rip the audio from the video and send the audio to an Icecast2 / KH or Shoutcast server.

# Tutorial
You can find a setup on this page: https://vanmarion.nl/blog/blog/wowza-4-x-audiorepeater-2-module

# Reference
https://www.wowza.com/community/t/audiorepeater-module-for-live-audio-video-streams/603

```
This is a module which allows the audio of a Audio/Video stream to stripped out and a new stream to be created so providing a lower bandwidth option without the need to send a separate stream.

It can be used in a variety of situations where a lower bandwidth option is required but no re-encoding is possible/wanted
The audio stream can also be sent to a Shoutcast server if it is a valid MP3 or AAC+ stream.
It can be downloaded from here along with the instructions

//
New features are
You can repeat multiple streams in the same application. Each published stream looks for a configuration file in the StorageDir called -repeat.txt which should contain the details of where to repeat to. Please see the PDF for specific details

AAC+ is now fully supported for both RTMP and Shoutcast connections. This has been tested for LC, HE and HE v2.
When connecting to Shoutcast if the audio is MP3 the bitrate is automatically detected, AAC+ streams you have to configure the required bitrate display for Shoutcast.
Auto reconnect to unstable Shoutcast servers is now fully working, ie. if the remote side goes away Wowza will auto reconnect when it comes back.
Stalled source streams are detected and audio repeated streams are closed when no data from the source is detected.
Enjoy.

Shamrock

The new version fully supports AAC+ and also multiple streams in an application.

```