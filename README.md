# Development of a Home Assistant Using Open-Source LLMs
### Master's Dissertation — University of Minho

**⭐ Final Grade: 17/20**

This repository contains the work developed for my Master's dissertation in Informatics Engineering (October 2025). The project, titled **Clarisse**, is a privacy-focused virtual home assistant designed to operate using entirely open-source technologies, avoiding reliance on proprietary cloud ecosystems like Alexa or Google Assistant.

### 📖 Project Overview
Clarisse was developed within the **Ready to Use Technology (R2UT)** project to enable natural voice interaction in smart homes, with a specific focus on **European Portuguese**.

The system utilizes a modular **Multi-Agent Architecture** where a central Orchestrator uses an LLM to route user requests to specialized agents (Device Control, Weather, Reminders, and Memory). This allows for complex reasoning, context retention, and precise tool execution.

### 🛠️ Key Technologies
The assistant follows a distributed architecture (Smart Speaker Client + GPU Inference Server):

*   **LLM Engine:** Llama-3.3-70B-Instruct (Quantized) served via **vLLM**.
*   **Speech-to-Text:** OpenAI **Whisper** (Fine-tuned for Portuguese).
*   **Text-to-Speech:** **Piper TTS** (with custom voice cloning).
*   **Wake Word & VAD:** openWakeWord & Silero VAD.
*   **Backend:** Python, FastAPI, and Eclipse Ditto for IoT device management.
*   **Hardware:** Raspberry Pi (Client) and NVIDIA H200 (Server).

### 📄 Author
**Pedro Miguel Castilho Martins**