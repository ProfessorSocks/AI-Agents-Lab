# Roadmap

## Phase 1 — Foundation

Goal: Get a working local monitoring agent.

- [x] Create Python project
- [x] Set up virtual environment
- [x] Monitor Open WebUI
- [x] Monitor Ollama
- [x] Monitor Home Assistant
- [x] Check CPU, RAM, and disk usage
- [x] Send Home Assistant notifications
- [x] Keep a basic log file

## Phase 2 — Self-Healing Systems Agent

Goal: Make the agent take safe automatic actions.

- [x] Restart Open WebUI Docker container when offline
- [x] Restart Ollama Windows process when offline
- [x] Verify service recovery after restart
- [ ] Add cooldowns to prevent restart loops
- [ ] Track how many restarts happen per day
- [ ] Add severity levels: INFO, WARNING, CRITICAL
- [ ] Add Docker container status inspection
- [ ] Add Windows process checks
- [ ] Add GPU status monitoring
- [ ] Add disk-space cleanup recommendations

## Phase 3 — Agent Memory

Goal: Make the agent notice patterns over time.

- [ ] Create structured JSON log
- [ ] Track repeated failures
- [ ] Summarize daily system health
- [ ] Ask Ollama for root-cause analysis when problems repeat
- [ ] Generate weekly reliability reports
- [ ] Store known fixes and past actions

## Phase 4 — Home Assistant Operator

Goal: Connect the AI systems agent to the smart home.

- [ ] Send Alexa announcements for critical alerts
- [ ] Create Home Assistant dashboard sensors
- [ ] Add input booleans to enable/disable auto-repair
- [ ] Add Home Assistant buttons for manual agent actions
- [ ] Notify when the AI computer reboots
- [ ] Monitor smart home dependencies

## Phase 5 — Mechatronics Learning Coach

Goal: Build a personal AI coach for mechatronics and IT skill growth.

- [ ] Track daily learning tasks
- [ ] Recommend next project step
- [ ] Maintain project notes
- [ ] Generate Anki cards from study notes
- [ ] Help plan ESP32, Raspberry Pi, and robotics projects
- [ ] Connect progress to career goals

## Phase 6 — Bambu Printer Monitoring Agent

Goal: Add practical hardware monitoring.

- [ ] Monitor print status from Home Assistant
- [ ] Announce print completion
- [ ] Detect printer errors
- [ ] Detect filament runout
- [ ] Detect spaghetti or failed print alerts if available
- [ ] Log print history
- [ ] Recommend maintenance tasks

## Phase 7 — Opportunity Finder

Goal: Support money-making and IT career growth.

- [ ] Search for computer repair opportunities
- [ ] Search for entry-level IT jobs
- [ ] Rank opportunities by value
- [ ] Draft application notes
- [ ] Track follow-ups
- [ ] Recommend portfolio improvements based on job descriptions

## Long-Term Vision

The final system should become a local AI operations assistant for:

- Home lab reliability
- Smart home automation
- 3D printer monitoring
- Mechatronics learning
- IT career growth
- Practical money-making projects

The goal is not to build a toy chatbot. The goal is to build a useful local agent that can observe, reason, act, and improve over time.
