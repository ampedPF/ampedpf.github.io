## 5. Mute/Unmute App audio

There are a number of ways to achieve this but all in all, you'd need to have a seperate audio input which replicate the output from "[B] App.".

Using [Virtual Audio Cable](https://vb-audio.com/Cable/index.htm) additional cables for example, you could have the following setup:

- ```[B] App. Input``` is set as the output of Spotify from Windows app volume panel (Win + R, then type ```ms-settings:app-volume```).
- from Windows ```Sound``` panel (win+R, then type ```mmsys.cpl sounds```), activate the listen option of ```[B] App. Output``` and set it to ```[D] VoDs Output```

![listen](./images/listen.png)

- if you don't have any available Aux Audio slot in OBS ```Global Audio Devices```, you can add an ```Audio input capture source``` to your scene and select ```[D] VoDs Output```.
- in OBS ```Advanced Audio Properties```, set it active only on Track 6 and you're all set.
- (optional) you can set a hotkey to mute/unmute that source

![hotkey](./images/hotkey.png)
