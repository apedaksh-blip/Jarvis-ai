# AYUSH // JARVIS v2

## Files
- `index.html` — cinematic JARVIS HUD + text/voice UI
- `netlify/functions/chat.mjs` — secure server-side OpenAI API proxy
- `netlify.toml` — Netlify Functions directory

## Netlify setup
In Netlify:
1. Site configuration → Environment variables.
2. Add `OPENAI_API_KEY` with your OpenAI API key.
3. Optional: add `OPENAI_MODEL` = `gpt-5.6-luna`.
4. Redeploy.

Do NOT put the API key inside `index.html` or GitHub.

Voice input uses the browser's SpeechRecognition API where supported. Voice output uses the browser's speechSynthesis API.
