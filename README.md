# Claude-Code-for-FREE Claude Code with Ollama (Anthropic API Compatibility)

## Profile Information

<!-- ========================================= -->
<!-- ULTRA-FUTURISTIC HEADER (REPLACES OLD BLACK HEADER) -->
<!-- Paste this entire file into docs/index.md -->
<!-- ========================================= -->

<style>
/* Neon GRID background */
.neon-grid {
  background: #000;
  position: relative;
  overflow: hidden;
  padding: 70px 20px;
  border-bottom: 3px solid #0ff;
}

/* Grid lines */
.neon-grid::before {
  content: "";
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background-image:
        linear-gradient(rgba(0,238,255,0.06) 1px, transparent 1px),
        linear-gradient(90deg, rgba(0,238,255,0.06) 1px, transparent 1px);
  background-size: 50px 50px;
  animation: gridMove 12s linear infinite;
  pointer-events: none;
}

/* Grid movement */
@keyframes gridMove {
  0% { transform: translateY(0); }
  100% { transform: translateY(50px); }
}

/* Floating particles */
@keyframes floatParticle {
  0% { transform: translateY(0) translateX(0); opacity: 0.9; }
  50% { transform: translateY(-20px) translateX(10px); opacity: 0.6; }
  100% { transform: translateY(0) translateX(0); opacity: 0.9; }
}

.particle {
  position: absolute;
  width: 10px;
  height: 10px;
  background: radial-gradient(circle, #00eaff, rgba(0,234,255,0.2));
  border-radius: 50%;
  filter: blur(4px);
  animation: floatParticle 6s ease-in-out infinite;
  pointer-events: none;
}

/* Glassmorphism card */
.glass-box {
  position: relative;
  display: inline-block;
  padding: 28px 32px;
  border-radius: 18px;
  background: rgba(0, 255, 255, 0.03);
  border: 1px solid rgba(0, 255, 255, 0.12);
  backdrop-filter: blur(8px);
  box-shadow: 0 8px 30px rgba(0,0,0,0.6);
  z-index: 2;
  text-align: center;
  max-width: 920px;
  width: 100%;
}

/* Profile image */
.profile-img {
  width: 132px;
  height: 132px;
  border-radius: 50%;
  border: 3px solid rgba(0, 234, 255, 0.9);
  box-shadow: 0 0 26px rgba(0,234,255,0.18);
  object-fit: cover;
}

/* Name glow */
.name-glow {
  font-size: 48px;
  font-weight: 800;
  color: #e6ffff;
  margin: 16px 0 6px;
  text-shadow: 0 0 12px #00eaff, 0 0 30px #00b8ff;
}

/* Typing animation */
.typing {
  color: #9fe6ff;
  font-size: 20px;
  white-space: nowrap;
  overflow: hidden;
  border-right: 2px solid #9fe6ff;
  width: 0;
  display: inline-block;
  animation: typing 4.5s steps(30, end) infinite, blink 0.9s step-end infinite;
  margin-bottom: 14px;
}

@keyframes typing {
  0% { width: 0; }
  45% { width: 260px; }
  100% { width: 0; }
}
@keyframes blink {
  50% { border-color: transparent; }
}

/* Navbar */
.navbar {
  margin-top: 20px;
  display: flex;
  justify-content: center;
  gap: 16px;
  flex-wrap: wrap;
}

.navbar a {
  color: #aef0ff;
  text-decoration: none;
  font-weight: 600;
  padding: 8px 14px;
  border-radius: 8px;
  transition: all 0.25s ease;
  border-bottom: 2px solid transparent;
}

.navbar a:hover {
  color: #ffffff;
  background: rgba(255,255,255,0.02);
  border-bottom: 2px solid #00eaff;
  transform: translateY(-2px);
}

/* Social icons row */
.social-links {
  margin-top: 18px;
}

.social-links a {
  display: inline-block;
  margin: 0 10px;
  text-decoration: none;
  color: #9fe6ff;
  transition: color 0.2s;
}
.social-links a img { vertical-align: middle; width: 28px; height: 28px; filter: drop-shadow(0 0 6px rgba(0,234,255,0.12)); }

</style>

<div class="neon-grid">
  <!-- PARTLES (positions randomized; you can add/remove) -->
  <div class="particle" style="top:8%; left:18%; animation-delay:0s;"></div>
  <div class="particle" style="top:28%; left:72%; animation-delay:0.9s;"></div>
  <div class="particle" style="top:62%; left:45%; animation-delay:1.6s;"></div>
  <div class="particle" style="top:46%; left:12%; animation-delay:2.3s;"></div>
  <div class="particle" style="top:14%; left:86%; animation-delay:3.1s;"></div>

  <div style="display:flex; justify-content:center; padding:40px 16px;">
    <div class="glass-box">

      <!-- profile image (uses GitHub username .png endpoint) -->
      <img src="https://gifdb.com/images/high/coding-girl-animation-fe7t4gejurmtof8v.gif" width="400" alt="coding-boy-animation" />

      <!-- name -->
      <div class="name-glow">Samad</div>

      <!-- typing subtitle -->
      <div class="typing">AI Agents Developer</div>

      <!-- navbar -->
      <div class="navbar">
        <a href="#guide">Guide</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>      
      </div>
       

      <!-- social links -->
      <div class="social-links">
        <a href="https://github.com/samade747" target="_blank" title="GitHub">
          <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub">
        </a>
        <a href="https://www.linkedin.com/in/samaddeveloper-aiagents-developer/" target="_blank" title="LinkedIn">
          <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="LinkedIn">
        </a>
      </div>

    </div>
  </div>
</div>
![Profile Views](https://komarev.com/ghpvc/?username=samade747&style=flat-square)
---






![Profile Views](https://komarev.com/ghpvc/?username=samade747&style=flat-square)

![GitHub Followers](https://img.shields.io/github/followers/samade747?label=Followers&style=social)  

![GitHub Stars](https://img.shields.io/github/stars/samade747?label=Stars&style=social)




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

