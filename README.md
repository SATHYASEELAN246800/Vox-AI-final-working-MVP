
---

# 🌺 **VoxAI SalesIQ — Luxury AI Platform (Built for Ragul)**

### **A Fully AI-Powered Sales, Support & Automation Suite using 100% FREE HuggingFace Models**

Welcome to **VoxAI SalesIQ**, a next-generation luxury AI platform designed and developed by **Sathya Seelan**, created as a special project **for his brother Ragul**.
This application combines **enterprise-grade UI**, **free & open-source AI models**, **RAG search**, **full CRUD**, **voice AI**, **image/document AI**, and **workflow automation**—all running without paid APIs.

---

## 🚀 **Core Highlights**

* **Ultra-Luxury Frontend UI** (Animated Landing Page + Premium Cards)
* **100% Free Hugging Face Spaces AI Models (No OpenAI Required)**
* **Real-Time Chat AI** with Context, Memory & Personas
* **RAG-Based Knowledge Base Search**
* **Document Summarization + OCR + Image Analysis**
* **Real-Time Translation AI**
* **Voice-to-Text & Text-to-Speech**
* **AI Suggestions + Workflow Automation**
* **CRUD operations** for all business modules
* **SalesIQ Style Analytics, Leads, Conversations, Visitors, Reports**
* **Zoho-style Admin Features**
* **No backend server required — or optional free backend** (Deta Space / Render Free Tier)

---

# 🧠 **AI Models Used (Free & Open-Source)**

All AI is powered **100% by Hugging Face Spaces**, using free inference API endpoints:

### **Chat & General AI**

| Feature           | Model                                | Space                  |
| ----------------- | ------------------------------------ | ---------------------- |
| General Chat      | `mistralai/Mistral-7B-Instruct-v0.3` | HF Space Inference API |
| Long Context Chat | `meta-llama/Llama-3.1-8B-Instruct`   | HF Space               |
| Persona Chat      | `NousResearch/Hermes-2-Pro-Mistral`  | HF Space               |

---

### **Knowledge Base + RAG**

| Feature       | Model                                    |
| ------------- | ---------------------------------------- |
| Embeddings    | `sentence-transformers/all-MiniLM-L6-v2` |
| Vector Search | Local/Cloud ChromaDB                     |
| RAG QA        | Llama-3.1 / Mistral via HF API           |

---

### **Image & Docs AI**

| Feature            | Model                                    |
| ------------------ | ---------------------------------------- |
| OCR                | `tesseract` via HF                       |
| Image Caption      | `Salesforce/blip-image-captioning-large` |
| Visual Q&A         | `Salesforce/blip-vqa-base`               |
| Document Summaries | `google/pegasus-xsum`                    |

---

### **Voice AI**

| Feature        | Model                           |
| -------------- | ------------------------------- |
| Speech-to-Text | `openai/whisper-small` HF Space |
| Text-to-Speech | `coqui-ai/TTS`                  |

---

### **Translation**

| Feature                | Model                         |
| ---------------------- | ----------------------------- |
| Multilingual Translate | `Helsinki-NLP/opus-mt` family |

---

### **AI Suggestions**

| Feature                         | Model            |
| ------------------------------- | ---------------- |
| Automatic Replies               | Mistral Instruct |
| Email/Message Rewrite           | Llama-3.1        |
| Workflow Automation Suggestions | Hermes-2-Pro     |

---

# ⚙️ **Tech Stack**

### **Frontend**

* **Remix.run (React Framework)**
* **Tailwind CSS (Luxury Gradient Theme)**
* **ShadCN UI Components**
* **Framer Motion (Animations)**
* **Lucide Icons**
* **Chart.js (Analytics)**

### **AI Integration**

* **Hugging Face Inference API (Free)**
* **RAG Search using ChromaDB**
* **Vector DB for Knowledge Base**

### **Backend (Optional but Free)**

Choose any:

* **Deta Space (Free NoSQL + Serverless)**
* **Render Free Tier + Python FastAPI**
* **Supabase Free Tier (Postgres + Auth)**

### **Authentication (Optional)**

* Magic Link
* JWT
* Local DB Auth

---

# 🗂️ **Modules & Features (All Tabs)**

### ✓ Dashboard

Luxury animated dashboards with INR, USD, EUR revenue cards.

### ✓ Client Chat (AI Chat + Memory)

* User chat → Mistral Reply
* Persona support
* Stored conversation history

### ✓ Conversations

* CRUD for conversation logs
* Sentiment analysis
* Visitor tracking

### ✓ Leads

* Lead generator AI
* CRUD
* Auto follow-up suggestions

### ✓ Knowledge Base (RAG)

* Upload documents
* Auto-embed → Vector DB
* Ask questions about docs

### ✓ Analytics

* Visitor metrics
* Sales metrics
* Lead conversion

### ✓ Admin History

* Logs
* CRUD
* Admin workflow changes

### ✓ Workflow

* Automated workflow builder
* AI-generated automations

### ✓ Voice Settings

* TTS/STT model settings
* Voice sample testing

### ✓ Image & Docs

* OCR
* Image Caption
* Visual Q&A
* Document Summary

### ✓ Translation

* Real-time language convert

### ✓ Surveys

* AI-generated survey questions
* Export to CSV

### ✓ AI Suggestions

* Auto-reply
* Rewrite
* Smart summary

### ✓ Visitor Behavior

* Heatmap
* Time spent
* Pages viewed

### ✓ AI Personas

* Create custom personas with short system prompts

### ✓ Reports

* Download PDF reports
* Filter by date, region

### ✓ Zoho Info

* Company overview
* SalesIQ-style features

### ✓ General AI

* Open chat playground

### ✓ AI Status

* Model uptime
* API tests
* Current latency

### ✓ Settings

* Theme
* User settings
* API toggle

---

# 🎨 **Luxury GUI Enhancements**

* Mild golden gradient backgrounds
* Luxury 3D glass cards
* Animated transitions
* Neon border hover
* Soft shadows
* Premium typography

---

# 🧪 **Dummy Data (Indian Names)**

Used across Leads, Surveys, Conversations, and Personas:

* Ragul
* Sathya Seelan
* Aravind
* Priya
* Niveditha
* Karthikeyan
* Dhinesh Kumar
* Lavanya
* Sriram
* Naveen

---

# 🔌 **API Usage Example (HuggingFace Inference)**

### **Chat Completion API**

```js
const response = await fetch(
  "https://api-inference.huggingface.co/models/mistralai/Mistral-7B-Instruct-v0.3",
  {
    method: "POST",
    headers: { "Authorization": `Bearer ${HF_TOKEN}` },
    body: JSON.stringify({ inputs: userMessage })
  }
);

const result = await response.json();
return result[0].generated_text;
```

---

# 🏗️ **CRUD Example (Leads Module — Deta Space)**

```js
import { Deta } from "deta";

const deta = Deta(DETA_KEY);
const leads = deta.Base("leads");

export const addLead = (data) => leads.put(data);
export const getLead = (id) => leads.get(id);
export const deleteLead = (id) => leads.delete(id);
export const listLeads = () => leads.fetch();
```

---

# 📊 **Revenue Example Cards**

* ₹12,45,000 revenue
* $42,500 monthly revenue
* €38,700 quarterly revenue

---

# 🏁 Deployment

You may deploy on:

* **Vercel** (frontend)
* **Deta** (backend)
* **Render** (FastAPI backend)
* **Supabase** (DB + Auth)

---

# ❤️ **Created for Ragul**

This project is designed, engineered, and polished with love by **Sathya Seelan**, dedicated to his brother **Ragul**, with a vision to build a world-class luxury AI ecosystem using 100% free and open technology.


---
sathyav5 orginal source base44 = https://app.base44.com/apps/69193c41ed6ebecdf7fdd106/editor/preview/dashboard

sathyav6demo copy source base44 = https://app.base44.com/apps/69198738e66921b8353affc2/editor/preview/dashboard 

deployed link from sathyav6 demo base44 = https://ragul-vox-ai-zoho-corporation.base44.app



---
