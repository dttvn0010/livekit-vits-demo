1. Install livekit plugins:  

```
  pip install \
    "livekit-agents[deepgram,openai,cartesia,silero,turn-detector]~=1.0" \
    "livekit-plugins-noise-cancellation~=0.2" \
    "python-dotenv"

```

2. Download model files: python agent.py download-files 


3. Start agent:  
```
   python agent dev
```


   
