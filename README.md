1. Install livekit plugins:  

```
  pip install \
    "livekit-agents[deepgram,openai,cartesia,silero,turn-detector]~=1.0" \
    "livekit-plugins-noise-cancellation~=0.2" \
    "python-dotenv"
```

2. Download file "agent.py":  
   ```
   wget https://raw.githubusercontent.com/dttvn0010/livekit-vits-demo/refs/heads/main/agent.py
   ```

3. Create file ".env.local" with the following content:
```
  OPENAI_API_KEY=<your_openai_key>
  LIVEKIT_URL=wss://<your_livekit_project_id>.livekit.cloud
  LIVEKIT_API_KEY=<your_livekit_api_key>
  LIVEKIT_API_SECRET=<your_livekit_api_secret>
```
For Windows, you may need to set OPENAI_API_KEY in System Environemnt, or from the terminal directly:
```
  set OPENAI_API_KEY=<your_openai_key>
```
See: https://docs.livekit.io/agents/start/voice-ai/ for more details.

4. Download model files:  
   ```
   python agent.py download-files
   ```

5. Start agent:  
```
   python agent.py dev
```

6. Open livekit playground from browser: https://agents-playground.livekit.io and start using the agent.


   
