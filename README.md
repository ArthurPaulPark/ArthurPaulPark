## Arthur Park

Computer science student building applications where **user data stays on the user's machine**.

That constraint drives the architecture rather than decorating it: a fitness
tracker that never ships a webcam frame to a server, and a QR scanner that
analyzes a link without ever requesting it. Both ship as working software you
can run today.

---

### Selected projects

#### [GRU Fitness](https://github.com/ArthurPaulPark/Fitness_Web) · [live demo →](https://arthurpaulpark.github.io/Fitness_Web/)

Browser-based exercise assistant that counts reps and gives real-time form
feedback for squats, push-ups, and pull-ups. Webcam frames, pose data, and
session statistics never leave the device — there is no backend, no account,
and no API key.

```text
Webcam → MediaPipe Pose Landmarker → 33 landmarks × (x, y, z, visibility)
       → 30-frame sequence (132 features/frame) → 2-layer GRU (64 hidden units)
       → ONNX Runtime Web → posture signal
       → joint-angle state machine → reps, form score, feedback
```

Three exercise-specific GRU classifiers trained in PyTorch and exported to
ONNX, running client-side through ONNX Runtime Web. Rep counting is a
rule-based state machine layered on the model output, so a rep only counts
after the sequence receives a good-posture signal during its measuring phase.

`PyTorch` · `ONNX Runtime Web` · `MediaPipe` · `WebAssembly` · `JavaScript`

#### [QR Guard](https://github.com/ArthurPaulPark/Secure_QR_Scanner)

Offline QR scanner for macOS that surfaces risk signals in a decoded URL
**without fetching it**. Skipping network I/O during analysis is the security
property: a malicious QR cannot use the scan itself to reach the local
network, trigger a state-changing request, or collect the user's IP.

The tool deliberately never labels a link *safe* — it reports what it can
observe locally (dangerous URI schemes, private and reserved IPs, punycode
lookalikes, brand impersonation, redirect parameters) and leaves the verdict
to the user. Image input is bounded and validated: magic-byte checks, size
and pixel ceilings, regular files only, opened with `O_NOFOLLOW`.

Dependencies are pinned exactly for reproducible audits, and the security
tests assert the boundary holds — one patches `socket.getaddrinfo` to raise,
proving analysis completes with no DNS resolution at all.

`Python` · `OpenCV` · `Tkinter` · `Threat modeling` · `unittest`

#### [Falling System](https://github.com/ArthurPaulPark/FallingSystem)

A 3D free-fall physics simulator built in Unity during high school, letting
students compare gravitational acceleration across Earth, the Moon, and Mars.
Distributed as a prebuilt Windows binary. Earlier work, kept public as a record
of where the interest in simulation and interactive tooling started.

`Unity` · `C#`

---

### Working with

| | |
| --- | --- |
| **Languages** | Python · C# · Java · JavaScript |
| **ML** | PyTorch · ONNX · MediaPipe |
| **Practices** | On-device inference · Threat modeling · Reproducible builds |

---

### Currently exploring

- LLM agent architectures and the Model Context Protocol (MCP)
- Deploying models to constrained runtimes — WebAssembly, edge, and offline-first targets
- Retrieval systems that keep the index local

---

<sub>GRU Fitness and QR Guard are MIT-licensed and runnable from source.
Open an issue on any repository to get in touch.</sub>
