# CineGato | Krunker Cutscene Engine

Simple cutscenes tool for krunkscript | Easy to set up cutscenes

[Here's a video of it working](https://streamable.com/pq8tez)

This version includes the following functions:
## Control
Action| Description
-------- | -----
cts_newCutscene()		  | Creates a blank loaded cutscene
cts_playEvents(skippable) | Starts the cutscene
cts_endEvents() 		  | Ends the cutscene. Is called automatically after all events

## Events
Action| Description
-------- | -----
cts_camera_glideTo(relative, posX, posY, posZ, rotX, rotY, rotZ, duration)		  | Glides the camera to the specified location and rotation. Can be relative to player.
cts_camera_shake(intensity, duration) | Shakes the camera for the given values
cts_sound_play(assetID, volume, rate) | Plays a custom sound at the given volume and rate
cts_time_wait(duration) | Waits the desired time given in milliseconds
cts_show_arms() | Shows player model's arms. Called automatically after cutscene ends
cts_hide_arms() | Hides player model's arms
cts_player_bringToCamera() | Brings the player to the camera's location
cts_fade_in(duration) | Fades the camera back in over the duration given
cts_fade_out(duration () | Fades the camera out over the duration given

## Dialogue
Action| Description
-------- | -----
cts_dialogue_createBox() | Creates the Dialogue Box (MUST BE RUN BEFORE STARTING A NEW BOX OR ADDING TEXT)
cts_dialogue_add(dialogue, speaker, speed, autoClose) | Adds one page of text to the box. To hide speaker, leave it as a blank string
cts_dialogue_waitForFinish() | Stalls the cutscene until there is no more text box on screen

## Contributing
Feel free to create your own functions and submit them and I will add them.

For the most part, these should be written solely on the Client Side script.

If you have questions, join my [Discord](https://dsc.gg/gatohub) and ask me there
