<!-- Banner -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&amp;height=230&amp;color=0:0d1117,45:12304a,100:1f6feb&amp;text=Aditya%20Pande&amp;fontColor=ffffff&amp;fontSize=58&amp;fontAlignY=38&amp;desc=AI%2FML%20Engineer%2C%20Geospatial%20AI%2C%20Edge%20and%20Efficient%20ML&amp;descAlignY=60&amp;descSize=18&amp;animation=fadeIn" alt="Aditya Pande — AI/ML Engineer" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&amp;weight=500&amp;size=20&amp;duration=3200&amp;pause=900&amp;color=58A6FF&amp;center=true&amp;vCenter=true&amp;width=820&amp;height=40&amp;lines=Production-grade+multimodal+geospatial+systems;Edge+and+efficient+LLMs%2C+speculative+decoding%2C+quantization;Privacy-first%2C+offline-capable+ML+for+real+deployments;Real-time+IoT+telemetry+and+edge+computer+vision" alt="Typing tagline" />
</p>

<p align="center">
  <a href="https://linkedin.com/in/aditya-pande"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&amp;logo=linkedin&amp;logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:adityapande403@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&amp;logo=gmail&amp;logoColor=white" alt="Email"/></a>
  <a href="https://huggingface.co/Adityapande403"><img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&amp;logo=huggingface&amp;logoColor=black" alt="Hugging Face"/></a>
  <a href="https://neogeoinfo.com"><img src="https://img.shields.io/badge/NeoGeoInfo-0d1117?style=for-the-badge&amp;logo=googlemaps&amp;logoColor=white" alt="NeoGeoInfo"/></a>
  <a href="https://github.com/adityapande403/adityapande403/blob/main/Aditya_Pande_Resume.pdf"><img src="https://img.shields.io/badge/R%C3%A9sum%C3%A9-PDF-2ea043?style=for-the-badge&amp;logo=readme&amp;logoColor=white" alt="Resume"/></a>
</p>

---

## 👋 About

I'm an **AI/ML Engineer (Entrepreneur-in-Residence) at [NeoGeoInfo Technologies](https://neogeoinfo.com)**. I design and ship end-to-end intelligent systems: multimodal geospatial fusion pipelines, real-time fleet telemetry, and small, fast models that run offline on a single consumer GPU or a CPU.

| | |
|---|---|
| 🔭 **Building now** | OptiFleet (IoT telemetry) · Multimodal Geospatial Fusion · edge LLM inference · privacy-first Indic NLP |
| 🌱 **Going deeper on** | Agentic AI · MLOps · Geospatial Intelligence · efficient inference |
| 💡 **Open to** | Geospatial AI · Autonomous Systems · Production ML |
| ⚙️ **Default stance** | Verify the model's output with deterministic checks, and publish the numbers, including the unflattering ones |

---

## 🧭 How I Build

```mermaid
flowchart LR
    A["Problem framing"] --> B["Synthetic + curated data<br/>hash-dedup, zero-leakage splits"]
    B --> C["LoRA / SFT / GRPO"]
    C --> D["Deterministic verification<br/>validators, compilers, equivalence checks"]
    D --> E["Quantize and export<br/>ONNX INT8, GGUF, Safetensors"]
    E --> F["Serve<br/>Python SDK, FastAPI, Node SDK, CLI"]
    F --> G["Offline / edge deployment"]
```

- **Verify, don't trust.** Models sit inside deterministic guardrails: Verhoeff and Luhn checksums, `jsonschema` validation, sandboxed `gcc -Wall -Wextra -Werror` builds, token-level equivalence tests.
- **Leakage-free evaluation.** Hash-based dedup and split-leakage audits before any number gets reported.
- **Small and local by default.** Quantized ONNX/GGUF artifacts, under 3 GB of VRAM, CPU fallbacks, no runtime network calls.
- **Shipped, not demoed.** SDKs, REST APIs, CLIs, test suites, and reproducible reports in every repo.

---

## 🚀 Featured Projects

### ⚡ Efficient &amp; Edge LLMs

<table>
<tr>
<td width="50%" valign="top">
<h4><a href="https://github.com/adityapande403/SpecDecode-edge">SpecDecode Edge</a></h4>
<p>Research and deployment framework for <b>speculative decoding</b> on a single GPU. Trains Medusa-style draft heads on a frozen Qwen2.5-1.5B target and verifies that output stays token-for-token identical to standard decoding.</p>
<sub><code>PyTorch</code> · <code>Medusa heads</code> · <code>KV-cache rollback</code> · <code>vLLM/Safetensors export</code> · <a href="https://huggingface.co/Adityapande403/SpecDecode-edge">🤗 Model</a></sub>
</td>
<td width="50%" valign="top">
<h4><a href="https://github.com/adityapande403/Embeddie-coder">EmbeddedCoder AI</a></h4>
<p>Offline-first small language model for <b>embedded systems engineering</b>: firmware, RTOS, and hardware triage. Paired with deterministic Modbus / J1939 / OBD-II / AIS-140 decoders, sandboxed GCC checks, and local BM25 datasheet retrieval.</p>
<sub><code>Qwen2.5-Coder</code> · <code>LoRA SFT</code> · <code>BM25 RAG</code> · <code>FastAPI</code> · <a href="https://huggingface.co/Adityapande403/embeddie-coder">🤗 Model</a></sub>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<h4><a href="https://github.com/adityapande403/Universal-JSON-Extractor">Universal JSON Extractor</a></h4>
<p>Schema-guided extraction that turns noisy text (OCR, logs, tickets, scraped HTML) into <b>strictly validated JSON</b>. Prompt-injection isolation, bounded repair, and an abstention policy that refuses to invent missing fields.</p>
<sub><code>Qwen2.5-1.5B</code> · <code>PEFT / DPO / GRPO</code> · <code>Ollama / GGUF</code> · <code>FastAPI</code> · <a href="https://huggingface.co/Adityapande403/universal-json-extractor">🤗 Model</a></sub>
</td>
<td width="50%" valign="top">
<h4><a href="https://github.com/adityapande403/VisDoc-AI">VisDoc AI</a></h4>
<p><b>Visual document retrieval</b> with ColQwen2.5 and late-interaction MaxSim scoring. Searches datasheets, schematics, invoices and balance sheets straight from page images, with no OCR and no text chunking.</p>
<sub><code>ColQwen2.5</code> · <code>MaxSim</code> · <code>INT8 / 1-bit index</code> · <code>PyMuPDF</code> · <code>FastAPI</code> · <a href="https://huggingface.co/Adityapande403/VisDoc-AI">🤗 Model</a></sub>
</td>
</tr>
</table>

### 🛡️ Privacy-First Indic NLP

<table>
<tr>
<td width="50%" valign="top">
<h4><a href="https://github.com/adityapande403/Loc-shield-AI">LocalShield AI</a></h4>
<p>Offline <b>PII detection and redaction</b> before data reaches an external LLM or log pipeline. Hybrid engine: checksum validators (Aadhaar, cards, PAN, IFSC) plus a multilingual DistilBERT tagger for English, Hindi and Hinglish. Four redaction modes and optional encrypted, reversible pseudonymization.</p>
<sub><code>DistilBERT</code> · <code>ONNX INT8</code> · <code>FastAPI</code> · <code>Node.js SDK</code> · <a href="https://huggingface.co/Adityapande403/LocShield-AI">🤗 Model</a></sub>
</td>
<td width="50%" valign="top">
<h4><a href="https://github.com/adityapande403/Indic-mix-AI">IndicMix AI</a></h4>
<p>Language understanding for <b>code-mixed Indian text</b> (Hinglish, Telgish, Benglish and native scripts): intent, moderation, PII redaction, and entity-preserving normalization as three independently trainable model families.</p>
<sub><code>ONNX Runtime</code> · <code>Python + Node.js</code> · <code>FastAPI</code> · <code>edge-ready</code> · <a href="https://huggingface.co/Adityapande403/IndicMix-AI">🤗 Model</a></sub>
</td>
</tr>
</table>

### 🌍 Geospatial, IoT &amp; Computer Vision

<table>
<tr>
<td width="33%" valign="top">
<h4><a href="https://neogeoinfo.com/solutions/optifleet.html">OptiFleet</a></h4>
<p>Real-time IoT fleet platform: low-latency GPS telemetry, route optimization, fuel-efficiency analytics, and vision-based driver monitoring.</p>
<sub><code>IoT</code> · <code>telemetry</code> · <code>CV</code></sub>
</td>
<td width="33%" valign="top">
<h4><a href="https://github.com/adityapande403/multimodal-geospatial-fusion">Multimodal Geospatial Fusion</a></h4>
<p>Deep-learning pipeline fusing satellite imagery, LiDAR, GPR and GNSS. Attention-based multi-scale fusion delivered a <b>20% gain in spatial alignment accuracy</b>, evaluated with RMSE and SSIM.</p>
<sub><code>PyTorch</code> · <code>LiDAR</code> · <code>GPR</code> · <code>GNSS</code></sub>
</td>
<td width="33%" valign="top">
<h4><a href="https://github.com/adityapande403/cv_3d_detect">3D-Print Defect Detection</a></h4>
<p>YOLOv5 real-time defect detection for FFF/FDM printers: <b>&gt;90% detection accuracy</b>, deployed on a Raspberry Pi via TensorFlow Lite / ONNX.</p>
<sub><code>YOLOv5</code> · <code>TFLite</code> · <code>Raspberry Pi</code></sub>
</td>
</tr>
</table>

---

## 📏 Measured, Not Claimed

Every figure below comes from a report or README in the linked repo. The context column says what it was measured on.

| Project | Result | Context |
|---|---|---|
| **SpecDecode Edge** | Token-identical output in 6 of 8 workload categories · **1.08×** on code generation · **2.96 GB** peak VRAM | Frozen Qwen2.5-1.5B, RTX 5060 Ti 16 GB; the other 2 categories diverged only at exact bf16 logit ties |
| **VisDoc AI** | **253 ms → 10.7 ms** at 1,000 pages (23.7×) via two-stage pruning · INT8 index **2×** smaller with no NDCG@5 loss · 1-bit index **16×** smaller | Held-out set plus a 10,000-page scale benchmark |
| **Universal JSON Extractor** | **98%** JSON parse · **86%** schema compliance · **0%** hallucinated fields | 50 held-out samples, 1 epoch of LoRA SFT on 27k synthetic examples |
| **LocalShield AI** | **128.9 MB** INT8 ONNX · **3.95 ms** P50 end-to-end (2.27 ms raw model) · 38 tests passing | CPU-only, full detect-and-redact pipeline |
| **IndicMix AI** | **222 KB** INT8 ONNX · **0.69 ms** P50 full pipeline · 60 tests passing | Windows 11, Intel CPU |
| **EmbeddedCoder AI** | **~2.9 GB** VRAM · **56–60 tok/s** · 20/20 tests passing | i7-14700K + RTX 5060 Ti |

---

## 🛠️ Tech Stack

**Languages**<br/>
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&amp;logo=python&amp;logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&amp;logo=cplusplus&amp;logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&amp;logo=javascript&amp;logoColor=black)

**ML, LLMs &amp; Computer Vision**<br/>
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&amp;logo=pytorch&amp;logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&amp;logo=tensorflow&amp;logoColor=white)
![Hugging Face](https://img.shields.io/badge/Transformers_·_PEFT-FFD21E?style=flat-square&amp;logo=huggingface&amp;logoColor=black)
![ONNX](https://img.shields.io/badge/ONNX_Runtime-005CED?style=flat-square&amp;logo=onnx&amp;logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&amp;logo=opencv&amp;logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&amp;logo=scikitlearn&amp;logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO-Ultralytics-00B4FF?style=flat-square)

**Backend, MLOps &amp; Edge**<br/>
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&amp;logo=fastapi&amp;logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&amp;logo=nodedotjs&amp;logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&amp;logo=docker&amp;logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&amp;logo=postgresql&amp;logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama_·_GGUF-000000?style=flat-square&amp;logo=ollama&amp;logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&amp;logo=nvidia&amp;logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&amp;logo=raspberrypi&amp;logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&amp;logo=pytest&amp;logoColor=white)

**Specialized domains:** Geospatial AI (LiDAR · Satellite · GPR · GNSS) · IoT telemetry · Speculative decoding &amp; quantization · Retrieval (late interaction) · LangChain &amp; agentic systems

---

## 📊 GitHub Activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=adityapande403&amp;show_icons=true&amp;theme=tokyonight&amp;hide_border=true&amp;count_private=true" alt="GitHub stats" />
  <img height="165" src="https://streak-stats.demolab.com/?user=adityapande403&amp;theme=tokyonight&amp;hide_border=true" alt="GitHub streak" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=adityapande403&amp;layout=compact&amp;theme=tokyonight&amp;hide_border=true" alt="Top languages" />
</p>

---

## 📫 Let's Connect

I'm happy to talk about geospatial AI, efficient inference, or shipping ML that has to work offline.

- **Email:** [adityapande403@gmail.com](mailto:adityapande403@gmail.com)
- **LinkedIn:** [linkedin.com/in/aditya-pande](https://linkedin.com/in/aditya-pande)
- **Hugging Face:** [huggingface.co/Adityapande403](https://huggingface.co/Adityapande403)
- **Résumé:** [Download PDF](https://github.com/adityapande403/adityapande403/blob/main/Aditya_Pande_Resume.pdf)

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&amp;height=110&amp;color=0:0d1117,45:12304a,100:1f6feb&amp;section=footer" alt="" />
</p>

<p align="center"><i>Always learning, building, and shipping.</i></p>
