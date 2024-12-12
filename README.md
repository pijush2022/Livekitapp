'First open Livekit sandbox from this link :-  "https://cloud.livekit.io/projects/p_/sandbox"'
'Then from the profile create a new project'
'Go to the setting on the sandbox and create a Key - API Key,Secret Key and Url'
'And then follow the code '



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


'The api keys are as follows:-'

'LIVEKIT_URL="wss://radar-assisstant-qxnpthve.livekit.cloud"'
'LIVEKIT_API_KEY="API6sPifj8SQgEt"'
'LIVEKIT_API_SECRET="ZjV2o6xhmrDwDsbuPmUFlfVKIQawhfzsKlwfOjU3DKeB"'
'DEEPGRAM_API_KEY="93e797d9a10fc8ffb261c5205eb7cc595e306ba2"'
'CARTESIA_API_KEY="sk_car_sP-XwIY5BgeWhLSNQhoIA"'
'CEREBRAS_API_KEY="csk-wwe56rxmwn5chh6kp5h2hmv4dej2wth48rt9ex344cpywm3h"'
'ELEVEN_API_KEY = "sk_c2e10f3205f8ca25371c58d1e1cb66b49d2326e2dd90ae7d"'

## Run a client

1. Go to the [playground](https://agents-playground.livekit.io/#cam=0&mic=1&video=0&audio=1&chat=0&theme_color=amber) (code [here](https://github.com/livekit/agents-playground))
2. Choose the same LiveKit Cloud project you used in the agent's `.env` and click `Connect`
