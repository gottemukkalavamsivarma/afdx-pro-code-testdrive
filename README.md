# Agentforce DX - TDX26 Demo

This demo showcases the suite of Agentforce DX Pro-Code Developer Tools.

---

## Preview an Agent Using the CLI
```bash
sf agent preview --use-live-actions --authoring-bundle Local_Info_Agent
```
## Ask AFV to Diagnose Agent Behavior
```
Read the agentforce-development skill, then preview the local info agent to see if it's answering weather questions correctly.
```
## Run Agent Tests
```bash
sf agent test run --api-name Local_Info_Agent_Test --wait 5
```

---

# Other Useful Commands

## Update Agent Tests
```bash
sf agent test create --api-name Local_Info_Agent_Test --spec specs/Local_Info_Agent-testSpec.yaml --force-overwrite 
```

## Fetch Agent Test Results From a Previous Run
```bash
sf agent test results --job-id xxxxxx --json
```
---

# Demo Management Commands

## Reset the Demo
```bash
./setup
```
## Update the `agent` plugin
```bash
sf plugins install agent@latest
```
## Get the latest changes and tags
```bash
git pull --tags --force
```