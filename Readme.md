# TkVideoplayer

This is a simple library to **play video** files in tkinter. This library also provides the ability to play, pause, 
skip and seek to specific timestamps of the video. (Audio included)

### Installation
This is a modified version of tkVideoPlayer by PauleDemon. Download the folder tkVideoPlayer of this fork.

Functionalities:
- load(path) : to load a video file
- stop() : stops the video
- play() : plays the video
- video_info() : return video info like framerate(fps), durartion, frame size, total frames, codec and name of the video
- current_frame_number() : returns the frame number of current location
- current_img() : return the PIL image of current frame
- seek(sec, pause) : seek to any timestamp, use pause=True to pause after seeking
- seek_frame(frame, pause) : seeks accurately to any frame number, use pause=True to pause after seeking
- mute()/unmute() : enable audio in clip (currently in beta stage)
#### Simple Usage:
```python
import tkinter as tk
from tkVideoPlayer import TkinterVideo

root = tk.Tk()

videoplayer = TkinterVideo(master=root, scaled=True)
videoplayer.load(r"samplevideo.mp4")
videoplayer.pack(expand=True, fill="both")

videoplayer.play() # play the video

root.mainloop()
```
## If you are facing issues while playing some videos, turn off the audio.

### read the documentation [here](https://github.com/Akascape/tkVideoPlayer/blob/master/Documentation.md)

### Sample video players made using tkVideoPlayer:
<img src="https://user-images.githubusercontent.com/89206401/229363046-36ebcffd-36d2-4c7f-98ce-4aa6b402e9e0.png" width=550> 

https://user-images.githubusercontent.com/89206401/228515652-abe137d0-6823-4c56-ba5c-8eb8292e0182.mp4
