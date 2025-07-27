1. Install livekit plugins:  

```
  pip install \
    "livekit-agents[deepgram,openai,cartesia,silero,turn-detector]~=1.0" \
    "livekit-plugins-noise-cancellation~=0.2" \
    "python-dotenv"
```

2. Create file ".env.local" with the following content:
```
  export OPENAI_API_KEY=<your_openai_key>
  export LIVEKIT_URL=wss://<your_livekit_project_id>.livekit.cloud
  export LIVEKIT_API_KEY=<your_livekit_api_key>
  export LIVEKIT_API_SECRET=<your_livekit_api_secret>
```
See: https://docs.livekit.io/agents/start/voice-ai/ for more details.

3. Download model files:
   ```
   python agent.py download-files
   ```

4. Start agent:  
```
   python agent dev
```

5. Open livekit playground from browser: https://agents-playground.livekit.io and start using the agent.


   
