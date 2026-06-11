# AI Systems Agent

An always-on local AI systems agent for monitoring, reasoning about, and self-healing a home AI lab.

This project runs on a dedicated Windows AI computer with Docker, Ollama, Open WebUI, and Home Assistant. The agent monitors critical services, detects failures, uses a local LLM for analysis, sends Home Assistant notifications, and can automatically restart failed services.

## Current Capabilities

- Monitors Ollama
- Monitors Open WebUI
- Monitors Home Assistant
- Checks CPU, RAM, and disk usage
- Sends Home Assistant persistent notifications
- Uses local Ollama models for problem analysis
- Restarts Open WebUI Docker container if it goes offline
- Restarts Ollama Windows process if it goes offline
- Logs agent activity to `agent.log`
- Runs continuously as an always-on loop

## Why This Project Exists

The goal is to build a practical local AI agent that saves time, supports home lab reliability, and demonstrates real-world IT automation skills.

This is not just a chatbot. It is an agent that can:

1. Observe the system
2. Detect problems
3. Reason about what matters
4. Take action
5. Verify results
6. Log what happened

## System Architecture

```text
Windows AI Computer
├── Docker
│   ├── Home Assistant
│   └── Open WebUI
├── Ollama
│   └── Local LLMs
├── Python Agent
│   ├── System monitoring
│   ├── Docker control
│   ├── Ollama reasoning
│   └── Home Assistant notifications
└── Home Assistant
    └── Notifications / Alexa / future automations
```

## Agent Loop

```text
Observe → Analyze → Decide → Act → Verify → Remember → Repeat
```

## Project Structure

```text
ai-systems-agent/
├── systems_agent.py
├── monitor.py
├── .env.example
├── requirements.txt
├── ROADMAP.md
├── README.md
└── .gitignore
```

## Setup

### 1. Clone the repo

```powershell
git clone https://github.com/YOUR_USERNAME/ai-systems-agent.git
cd ai-systems-agent
```

### 2. Create a virtual environment

```powershell
python -m venv venv
```

### 3. Activate the environment

```powershell
.\venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```powershell
pip install -r requirements.txt
```

### 5. Create `.env`

Copy:

```powershell
copy .env.example .env
```

Edit `.env` with your real Home Assistant token.

## Environment Variables

```env
HOME_ASSISTANT_URL=http://192.168.x.x:8123
HOME_ASSISTANT_TOKEN=your_long_lived_access_token
OLLAMA_URL=http://localhost:11434
OPEN_WEBUI_URL=http://localhost:3000
```

## Run the Agent

```powershell
python systems_agent.py
```

## Current Status

This project is in early development.

Completed:

- Basic monitoring
- Always-on loop
- Home Assistant notifications
- Open WebUI self-healing
- Ollama self-healing
- Basic logging

Next:

- Restart cooldown memory
- Failure history
- Docker container health inspection
- Alexa announcements
- Bambu printer monitoring
- Mechatronics learning coach

## Portfolio Value

This project demonstrates:

- Python automation
- Windows scripting
- Docker operations
- Local AI integration
- Home Assistant API usage
- Systems monitoring
- Self-healing infrastructure
- Practical AI agent architecture

## Disclaimer

This agent can restart local services. Use carefully and review any action logic before enabling automatic repair behavior.
