1. Install livekit plugins:  

```
  pip install \
    "livekit-agents[deepgram,openai,cartesia,silero,turn-detector]~=1.0" \
    "livekit-plugins-noise-cancellation~=0.2" \
    "python-dotenv"

  pip install git+https://github.com/dttvn0010/livekit-vits.git  
```

2. Download model files:  
```
  python agent.py download-files  
```

3. Download TTS models from https://drive.google.com/file/d/1YYtDaqmd6oipHZ45GtGuXwHWBEMHl6pK/view?usp=drive_link and extract to folder "tts-models"  

4. Start agent:  
```
   python agent dev
```


   
