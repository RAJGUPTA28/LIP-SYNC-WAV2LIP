# LIP-SYNC-WAV2LIP
ABOUT
-----

Base Repository - [Wav2Lip](https://github.com/Rudrabha/Wav2Lip)
------
![IMG](https://github.com/RAJGUPTA28/LIP-SYNC-WAV2LIP/blob/main/lipsync-animation-cc-base-expression-data-4.jpeg)
![ING](https://github.com/RAJGUPTA28/LIP-SYNC-WAV2LIP/blob/main/obama_lip_syncing_uw_1499864933490.webp)
# Pretrained Model Download 

| Model  | Description |  Link to the model | 
| :-------------: | :---------------: | :---------------: |
| Wav2Lip  | Highly accurate lip-sync | [Link](https://iiitaphyd-my.sharepoint.com/:u:/g/personal/radrabha_m_research_iiit_ac_in/Eb3LEzbfuKlJiR600lQWRxgBIY27JZg80f7V9jtMfbNDaQ?e=TBFBVW)  |
| Wav2Lip + GAN  | Slightly inferior lip-sync, but better visual quality | [Link](https://iiitaphyd-my.sharepoint.com/:u:/g/personal/radrabha_m_research_iiit_ac_in/EdjI7bZlgApMqsVoEUUXpLsBxqXbn5z8VTmoxp55YNDcIA?e=n9ljGW) |




Lip-syncing videos using the pre-trained models (Inference)
-------
You can lip-sync any video to any audio:
```bash
python inference.py --checkpoint_path <ckpt> --face <video.mp4> --audio <an-audio-source> 
```
The result is saved (by default) in `results/result_voice.mp4`. You can specify it as an argument,  similar to several other available options. The audio source can be any file supported by `FFMPEG` containing audio data: `*.wav`, `*.mp3` or even a video file, from which the code will automatically extract the audio.


Input Files
---
 - Audio [Input_Audio](https://drive.google.com/file/d/1v1uthiVq20MfWpkV8LDOHJpudx49KYYx/view?usp=drive_link)
 - Video [Input_Video](https://www.youtube.com/watch?v=YMuuEv37s0o&sub)

   - Note
     ---
        - Make sure all the frames in the video must have a face in it , other wise the model will return No face detected Error

Output File
---
 - Final Video [result_video](https://drive.google.com/file/d/1rzS6IkmS6DVf36OOYnH6Qesk6zpJvglz/view?usp=drive_link)

IMPROVEMENTS
---
We can bring significant Improvement in the output by adjusting the arguments bringing the change in below variations

- Variations
  --- 
  - NO SMOOTH ARGUMENT 
  - PADDING ARGUMENT
  - RESIZE FACTOR

ISSUES
---
- The Pretrained model will only work if all the frames in the video must have a face in it
- ```bash
  --box method unknown
  ```
    - Raised the issue -  https://github.com/Rudrabha/Wav2Lip/issues/42#issuecomment-1807015405
 
**CONTRIBUTION**

