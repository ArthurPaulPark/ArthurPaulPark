<div align="center">

# 👋 Hi, I'm Arthur Park

### 🤖 AI Software Developer &nbsp;|&nbsp; 🎓 Computer Science Student

**Building software where user data never leaves the device.**

<br>

[![GitHub](https://img.shields.io/badge/GitHub-ArthurPaulPark-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ArthurPaulPark)
[![Live Demo](https://img.shields.io/badge/▶_Try_GRU_Fitness-Live_Demo-2ea44f?style=for-the-badge)](https://arthurpaulpark.github.io/Fitness_Web/)
[![Focus](https://img.shields.io/badge/Focus-On--Device_AI-7c3aed?style=for-the-badge)](#-featured-projects)

</div>

---

## 🚀 Featured Projects

### 🏋️ GRU Fitness &nbsp;·&nbsp; [![Live](https://img.shields.io/badge/▶_live-demo-2ea44f?style=flat-square)](https://arthurpaulpark.github.io/Fitness_Web/) [![Repo](https://img.shields.io/badge/source-code-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/ArthurPaulPark/Fitness_Web) ![MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

> **Real-time AI workout coach that runs entirely in your browser.**
> Counts reps and grades your form for squats, push-ups, and pull-ups —
> with **zero backend, zero account, zero API keys**. Webcam frames and pose
> data never leave the device.

```text
Webcam → MediaPipe Pose → 33 landmarks × (x, y, z, visibility)
       → 30-frame window (132 features) → 2-layer GRU (64 hidden units)
       → ONNX Runtime Web → posture signal
       → joint-angle state machine → reps · form score · feedback
```

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX_Runtime-005CED?style=flat-square&logo=onnx&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=flat-square&logo=google&logoColor=white)
![WebAssembly](https://img.shields.io/badge/WebAssembly-654FF0?style=flat-square&logo=webassembly&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

<br>

### 🔐 QR Guard &nbsp;·&nbsp; [![Repo](https://img.shields.io/badge/source-code-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/ArthurPaulPark/Secure_QR_Scanner) ![MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

> **Offline QR scanner that analyzes a link without ever requesting it.**
> Skipping network I/O *is* the security property — a malicious QR can't use
> your scan to probe your local network or harvest your IP.

- 🚫 **Never calls the URL** — no HTTP, no DNS, no redirect following
- 🎯 **Never says "safe"** — reports observable signals, leaves the verdict to you
- 🔍 Flags dangerous schemes, private IPs, punycode lookalikes, brand impersonation
- 🛡️ Hardened input: magic-byte checks, size and pixel ceilings, `O_NOFOLLOW`
- ✅ Security tests that patch `getaddrinfo` to prove analysis does zero DNS

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Tkinter](https://img.shields.io/badge/Tkinter-FFD43B?style=flat-square&logo=python&logoColor=black)
![macOS](https://img.shields.io/badge/macOS-000000?style=flat-square&logo=apple&logoColor=white)

<br>

### 🪐 Falling System &nbsp;·&nbsp; [![Repo](https://img.shields.io/badge/source-code-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/ArthurPaulPark/FallingSystem)

> **3D free-fall physics simulator built in Unity during high school.**
> Compare gravitational acceleration across 🌍 Earth, 🌕 the Moon, and 🔴 Mars
> in an interactive 3D space. Where the interest in simulation started.

![Unity](https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white)

---

## 🛠 Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=csharp&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**AI / Machine Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=for-the-badge&logo=google&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Frameworks & Runtimes**

![Unity](https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![WebAssembly](https://img.shields.io/badge/WebAssembly-654FF0?style=for-the-badge&logo=webassembly&logoColor=white)

**Tools**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![macOS](https://img.shields.io/badge/macOS-000000?style=for-the-badge&logo=apple&logoColor=white)

---

## 📚 Currently Exploring

- 🧠 LLM agent architectures & the **Model Context Protocol (MCP)**
- 📦 Deploying models to constrained runtimes — **WebAssembly, edge, offline-first**
- 🔎 **Retrieval systems that keep the index local**
- 🏗️ AI software architecture & multi-agent systems

---

<div align="center">

## 📊 GitHub Activity

<a href="https://github.com/ArthurPaulPark">
  <img src="https://streak-stats.demolab.com?user=ArthurPaulPark&theme=github-dark&hide_border=true" height="180" alt="Contribution streak" />
</a>

<br><br>

<sub>💬 Open an issue on any repository to get in touch.</sub>

</div>
