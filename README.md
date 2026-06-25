# Artifact Cleanroom: Autonomous AI Code Quarantine Guardrail

An advanced security framework built for the **Kaggle AI Agents Intensive Capstone (Freestyle Track)**. This system intercepts untrusted AI-generated artifacts, routes them through a 2-stage verification graph, and enforces safety constraints before local environment execution.

## 🛠️ Project Architecture
- `agent.yaml`: Defines the multi-agent execution states and quarantine routing topology.
- `cleanroom_scanner.py`: Core programmatic execution engine handling line-by-line structural hazard checks.
- `SKILL.md`: Portability skill definition mapping native capabilities to the Antigravity ecosystem.

## 🚀 Quick Start & Verification
To test the environment locally, execute the engine against the provided scenario payloads:

```powershell
# Scenario 1: Verify a safe developer script passing through clear
python cleanroom_scanner.py safe_code.py

# Scenario 2: Verify an obfuscated malicious threat being intercepted & suspended
python cleanroom_scanner.py clever_obfuscation.py
