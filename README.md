# Claude-Code-for-FREE Claude Code with Ollama (Anthropic API Compatibility)

**Release date:** January 16, 2026  
**Requires:** Ollama v0.14.0+

This README explains how to run **Claude Code** using **Ollama** with full **Anthropic Messages API compatibility**, allowing you to use Claude Code with **open‑source local models** or **Ollama Cloud models**.

Claude Code is Anthropic’s agentic coding tool that runs directly in your terminal. With Ollama acting as an Anthropic‑compatible backend, you can replace Claude models with local or cloud models seamlessly.

---

## Features

- Anthropic Messages API compatibility
- Works with Claude Code CLI
- Local and cloud model support
- Tool / function calling
- Streaming responses
- Multi‑turn conversations
- System prompts
- Extended thinking
- Vision (image input)

---

## Prerequisites

- Ollama **v0.14.0 or later**
- Claude Code CLI
- A model with **≥ 64k context length** (recommended)

---

## Install Claude Code

### macOS / Linux / WSL

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

### Windows (PowerShell)

```powershell
irm https://claude.ai/install.ps1 | iex
```

### Windows (CMD)

```cmd
curl -fsSL https://claude.ai/install.cmd -o install.cmd && install.cmd && del install.cmd
```

---

## Connect Claude Code to Ollama

Configure the following environment variables so Claude Code talks to Ollama instead of Anthropic’s cloud.

```bash
export ANTHROPIC_AUTH_TOKEN=ollama
export ANTHROPIC_BASE_URL=http://localhost:11434
```

> The API key is required by the SDK but ignored by Ollama.

---

## Run Claude Code

### Using a local model

```bash
claude --model gpt-oss:20b
```

### Using an Ollama Cloud model

```bash
claude --model glm-4.7:cloud
```

> Ollama Cloud models always run at their **maximum context length**.

---

## Recommended Models

### Local Models

- `gpt-oss:20b`
- `qwen3-coder`

### Cloud Models

- `glm-4.7:cloud`
- `minimax-m2.1:cloud`

---

## Context Length

Claude Code performs best with **64k+ token context** models.

To adjust local model context length, refer to the Ollama context length documentation.

---

## Using the Anthropic SDK with Ollama

Existing applications using the **Anthropic SDK** can connect to Ollama by simply changing the `base_url`.

### Python Example

```python
import anthropic

client = anthropic.Anthropic(
    base_url='http://localhost:11434',
    api_key='ollama',  # required but ignored
)

message = client.messages.create(
    model='qwen3-coder',
    messages=[
        {'role': 'user', 'content': 'Write a function to check if a number is prime'}
    ]
)

print(message.content[0].text)
```

---

### JavaScript Example

```javascript
import Anthropic from '@anthropic-ai/sdk'

const anthropic = new Anthropic({
  baseURL: 'http://localhost:11434',
  apiKey: 'ollama',
})

const message = await anthropic.messages.create({
  model: 'qwen3-coder',
  messages: [{ role: 'user', content: 'Write a function to check if a number is prime' }],
})

console.log(message.content[0].text)
```

---

## Tool / Function Calling

Models can invoke tools exactly like Claude models.

### Python Tool Example

```python
import anthropic

client = anthropic.Anthropic(
    base_url='http://localhost:11434',
    api_key='ollama',
)

message = client.messages.create(
    model='qwen3-coder',
    tools=[
        {
            'name': 'get_weather',
            'description': 'Get the current weather in a location',
            'input_schema': {
                'type': 'object',
                'properties': {
                    'location': {
                        'type': 'string',
                        'description': 'The city and state, e.g. San Francisco, CA'
                    }
                },
                'required': ['location']
            }
        }
    ],
    messages=[{'role': 'user', 'content': "What's the weather in San Francisco?"}]
)

for block in message.content:
    if block.type == 'tool_use':
        print(f'Tool: {block.name}')
        print(f'Input: {block.input}')
```

---

## Supported Anthropic Features

- Messages API
- Multi‑turn conversations
- Streaming
- System prompts
- Tool / function calling
- Extended thinking
- Vision (image input)

For the complete compatibility list, see the Anthropic compatibility documentation.

---

## Learn More

- Claude Code official guide
- Ollama documentation
- Anthropic Messages API compatibility docs

---

## Summary

With Ollama acting as an Anthropic‑compatible backend, **Claude Code becomes a powerful local‑first coding agent** that works with open‑source and cloud models—without changing your existing Anthropic‑based workflows.

Happy hacking 🚀

