1. Install livekit plugins:  

```
  pip install \
    "livekit-agents[deepgram,openai,cartesia,silero,turn-detector]~=1.0" \
    "livekit-plugins-noise-cancellation~=0.2" \
    "python-dotenv"

  pip install git+https://github.com/dttvn0010/livekit-vits.git  
```

2. Install voice server from https://github.com/dttvn0010/vits-voice-server  

3. Update voice server url in file `agent.py`:  
```
    session = AgentSession(
        ...
        tts=TTS(lang="en", base_url="<voice_server_url>"),
        ...
    )

```


4. Start agent:  
```
   python agent dev
```


   
