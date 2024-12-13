#Instruction Details:-

`First open Livekit sandbox from this link :-  "https://cloud.livekit.io/projects/p_/sandbox"`
`Then from the profile create a new project`
`Go to the setting on the sandbox and create a Key - API Key,Secret Key and Url`
`And then follow the code `



# Insanely fast AI voice assistant in 50 LOC

Demo: [https://cerebras.vercel.app](https://cerebras.vercel.app)

This repo contains everything you need to run your own AI voice assistant that responds to you in less than 500ms.

It uses:
- 🌐 [LiveKit](https://github.com/livekit) transport
- 👂 [Deepgram](https://deepgram.com/) STT
- 🧠 [Cerebras](https://inference.cerebras.ai/) LLM
- 🗣️ [Cartesia](https://cartesia.ai/) TTS

## Run the assistant

1. `python -m venv .venv`
2. `sources .venv/Scripts/activate`
3. `pip install -r requirements.txt`
4. `cp .env.example .env`
5. add values for keys in `.env`
6. `python main.py dev`


## Run a client

1. Go to the [playground](https://agents-playground.livekit.io/#cam=0&mic=1&video=0&audio=1&chat=0&theme_color=amber) (code [here](https://github.com/livekit/agents-playground))
2. Choose the same LiveKit Cloud project you used in the agent's `.env` and click `Connect`
