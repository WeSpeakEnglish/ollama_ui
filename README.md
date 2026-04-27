# Ollama UI

A clean, lightweight, single-file web chat interface for Ollama with full conversation memory and context window control.

## Features

- Full conversation memory
- Context Window slider (real num_ctx control)
- Temperature adjustment
- Streaming responses
- System prompt support
- Automatic model loading
- Helpful ? tooltips
- Clear chat + memory reset

## How to Use

1. **Run Ollama:**
   ```
   ollama serve
   ```

2. **(Optional) SSH tunnel for remote server:**

 Run it locally if ollama running on remote server (for example in PowerShell) and keep the terminal opened
   
   ```
   ssh -L 11434:127.0.0.1:11434 user@your-server
   ```

4. Open `ollama-ui.html` in your browser
5. Click **Connect**, select a model and start chatting.

## Settings

| Setting | Description |
|---|---|
| `temp` | Controls creativity — `0.0` = safe/deterministic, `0.7` = default |
| `window` | Context window size in tokens |
| `context` | Quick preset selector |
| `stream` | Real-time response streaming (recommended ON) |
| `system prompt` | Hidden instruction passed to the model |

## Tips

- Pull models first: `ollama pull llama3:latest`
- Increase **window** for longer conversations
- Lower **temp** for coding or factual answers
- Use **Clear** to reset chat and memory

## Requirements

- [Ollama](https://ollama.com) installed and running
- A modern web browser
