<div align="center">

## \[ 3 lines of codes \]


</div>

### Description

Play a wave file with only 3 lines of codes!

It works with .wav files 100%, with other extension I don't know. Try and then report.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Power Of Anubis](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/power-of-anubis.md)
**Level**          |Beginner
**User Rating**    |4.2 (50 globes from 12 users)
**Compatibility**  |VB 6\.0
**Category**       |[Sound/MP3](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/sound-mp3__1-45.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/power-of-anubis-3-lines-of-codes__1-58843/archive/master.zip)





### Source Code

```
Private Declare Function sndPlaySound Lib "winmm.dll" Alias "sndPlaySoundA" _
(ByVal lpszSoundName As String, ByVal uFlags As Long) As Long
Const SND_SYNC = &H0
Const SND_ASYNC = &H1
Const SND_NODEFAULT = &H2
Const SND_LOOP = &H8
Const SND_NOSTOP = &H10
'----------PLAY WAVE SOUND--------
Private Sub PlayWaveSound_Click()
 soundfile$ = "c:/TheCustomSoundIWant.wav"
 wFlags% = SND_ASYNC Or SND_NODEFAULT
 HaHa = sndPlaySound(soundfile$, wFlags%)
End Sub
'-------STOP WAVE SOUND-------
Private Sub StopTheSound_Click()
StopTheSoundNOW = sndPlaySound(soundfile$, wFlags%)
End Sub
'Replace "c:/TheCustomSoundIWant.wav" with your sound
```

