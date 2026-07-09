# Augmenting Legacy: Localized Latent Compute & Knowledge Retrieval in Practice

Architectural AI Infrastructure framework developed at **Pei Cobb Freed & Partners Architects**.

## 🏛️ Executive Overview

Modern architectural practice sits at the intersection of decades of design heritage and rapid computational acceleration. This repository maps a comprehensive framework for embedding a firm’s unique design DNA directly into local AI generation pipelines, while simultaneously unlocking massive technical drawing archives using cloud-native machine learning infrastructure.

Rather than relying on generic, off-the-shelf public AI models, this architecture establishes a closed-loop system divided into two core paradigms:
1. **Generative Design Continuity:** Preserving and iterating on historical design language using custom-trained latent diffusion frameworks.
2. **Operational Intelligence:** Unlocking legacy archives and institutional knowledge via semantic vector search, localized Large Language Models (LLMs), and cloud-native document parsing.

## 🛠️ System Architecture & Tech Stack

```
                [ PCF HISTORICAL ARCHIVES ]
                    /                 \
        ( Design Images )            ( Technical Drawings/PDFs )
            /                         \
    [ ComfyUI LoRA Training ]        [ AWS Bedrock Embedding Pipeline ]
            |                           |
[ ControlNet + Multi-Model Canvas ]  [ OpenSearch API (Text/Image Input) ]
            |                           |
 ( Rapid Concept Generation )        ( Multi-Modal Document Retrieval )
```

## 📁 Repository Structure

```text
├── .github/
├── workflows/
│   ├── comfyui_lora_inference.config     # Standardized multi-ControlNet pipeline blueprint
│   ├── image_canvas_inpaint_flux.json    # Modular multi-engine image canvas editor
│   └── README.md                         # Workflow dependencies and node setups
├── slack-bot/
│   ├── app/
│   │   ├── main.py                       # Slack event listener and routing
│   │   ├── llm_sql_translator.py         # Local LLM structured prompt routing to SQL
│   │   └── vector_search.py              # Local semantic project history matching
│   ├── schema/
│   │   └── mock_project_db.sql           # Sanitized schema of operational databases
│   └── README.md                         # Bot deployment and local model variables
├── aws-bedrock-pipeline/
│   ├── cloudformation/
│   │   └── infrastructure.yaml           # Bedrock + OpenSearch environment definition
│   ├── lambda/
│   │   ├── pdf_vector_encoder.py         # Text/Visual chunking and vector processing
│   │   └── open_search_query.py          # Multi-modal (Image/Text) search router
│   └── README.md                         # AWS architecture and Armakuni R&D specs
└── README.md                             # Main Documentation
```

## 🚀 Core Pillars

### 1. Generative Design & Aesthetic Continuity

To prevent the dilution of our firm’s signature architectural language when using generative models, we bypass generic base outputs in favor of a hyper-localized diffusion ecosystem.

* **Custom DNA LoRA Training:** Custom Low-Rank Adaptations (LoRAs) are trained via AI-Toolkit using curated high-resolution datasets of our historical design portfolio. This embeds explicit spatial relationships, materiality preferences, and massing behaviors unique to our practice directly into the latent space weights.
* **Controlled Spatial Iteration:** To transform raw sketches or strict programmatic envelopes into articulated spaces, we utilize **ControlNet** chains (Depth, Lineart, and Canny) mapped over our proprietary LoRA weights. This guarantees that spatial constraints are mathematically respected while iterating.
* **Multi-Model Precision Editing:** For granular design changes, workflows are integrated into an open canvas environment utilizing specialized models depending on the task:
    * **Flux / Flux 2 Klein & Z Image Turbo:** For lightning-fast base iterations and sharp, contemporary architectural forms.
    * **Qwen Image Edit & Google Nano Banana Engines:** For intelligent regional inpainting, contextual object replacement, and localized material testing without changing global composition.

### 2. Knowledge Management & Project Intelligence (Slack Bot)

To bridge the gap between historical data silos and daily office operations, we developed an internal Slack bot that allows our teams to cross-reference our entire historical project database in real time.

* **Hybrid Search Routing:** The bot accepts natural language questions and processes them simultaneously through two channels:
    * **Semantic Vector Search:** Finds contextual matching across narrative text, project briefs, and geographical data.
    * **Local LLM Text-to-SQL:** A highly specialized local LLM parses the user input, extracts entity parameters, and dynamically constructs structurally sound SQL queries to fetch relational data (e.g., square footage, construction dates, project leads) from our core databases.


* **Frictionless UX:** By serving as a native application within Slack, employees can safely query sensitive institutional records without navigating fragmented database UIs.

### 3. Cloud-Native Legacy Blueprints Search (AWS R&D)

In a joint research and development initiative with **AWS** and their specialized sub-partner **Armakuni**, we engineered a prototype cloud-native interface to convert decades of physical and localized digital legacy drawings into an active, searchable knowledge base.

* **Vector Pipeline:** Legacy blueprints, construction documents, and schematic PDFs are ingested, chunked, and vectorized via **AWS Bedrock**.
* **Multi-Modal Retrieval via OpenSearch:** The system exposes an API capable of true multi-modal querying. Architects can input a line of text (e.g., *"brise-soleil structural detailing"* ) OR upload a snippet of an image/drawing file. The **Amazon OpenSearch** engine matches the vector mathematical representation and returns the top relevant high-resolution drawings instantly.
* **Infrastructure Modernization:** This pipeline forms the backbone of our ongoing architectural migration from vulnerable localized storage arrays into highly scalable, cloud-compute environments.

## 🔒 Security & Data Sovereignty Disclaimer

This repository serves as a **functional architectural blueprint** for AI integration within legacy corporate environments. All code provided in the `/slack-bot` and `/aws-pipeline` directories consists of sanitized, open-source abstractions, boilerplate code, and mock schemas.

* **No proprietary weights** (LoRA models trained on firm archives) are hosted here.
* **No sensitive client data or internal database strings** are included in any codebase configuration file.

## 👥 Contributors & Acknowledgments

* **Lead AI Architect & Infrastructure Systems Engineer:** Xiao Qin, George Podolak, Will Garris, Michael Lyon
* **Cloud Infrastructure Engineering Partner:** AWS / Armakuni R&D Team

*Developed under the technological innovation initiatives of Pei Cobb Freed & Partners Architects.*
