<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=omnimind&fontSize=60&fontColor=fff&animation=twinkling&fontAlignY=38&desc=No-code%20AI%20Chatbot%20Builder%20%7C%20WhatsApp%20%2B%20Slack%20%2B%20Web&descSize=16&descColor=fff&descAlignY=60" />

<br/>

[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://mongodb.com)
[![OpenAI](https://img.shields.io/badge/GPT--4-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)
[![Pinecone](https://img.shields.io/badge/Pinecone-RAG-000000?style=for-the-badge)](https://pinecone.io)

![License](https://img.shields.io/badge/License-MIT-00d4ff?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![PRs](https://img.shields.io/badge/PRs-Welcome-7c3aed?style=flat-square)

</div>

---

## 🤖 What is omnimind?

**omnimind** is a multi-tenant SaaS platform that lets anyone build and deploy intelligent AI chatbots — without writing a single line of code. Upload your knowledge base, configure your bot, and deploy to WhatsApp, Slack, or your website in minutes.

> Think of it as **the Notion of AI chatbots** — powerful under the hood, dead simple on the surface.

---

## ✨ Features

- 🧠 **LLM + RAG Architecture** — GPT-4 powered responses grounded in your actual content
- 📁 **Knowledge Base Upload** — Train your bot with PDF, DOCX, or plain text files
- 🌐 **Multi-channel Deployment** — WhatsApp, Slack, and embeddable web widget
- 🏢 **Multi-tenant SaaS** — Each user gets a fully isolated bot and data namespace
- 🔄 **Workflow Automation** — n8n integration for triggering actions on any event
- 📊 **Analytics Dashboard** — Track conversations, queries, and bot performance in real time
- 🔐 **Auth and Role Management** — JWT authentication with usage-based access limits
- ⚡ **Fast Retrieval** — Pinecone vector search for sub-100ms context lookup

---

## 🛠️ Tech Stack

| Layer | Technology |
|:---|:---|
| **Language** | TypeScript |
| **Backend** | Node.js, Express |
| **AI / LLM** | OpenAI GPT-4, LangChain |
| **Vector DB** | Pinecone |
| **Database** | MongoDB |
| **Auth** | JWT |
| **Automation** | n8n |
| **Deployment** | Docker, Vercel |

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- MongoDB (local or Atlas)
- OpenAI API key
- Pinecone API key

### Installation

```bash
git clone https://github.com/shaktivijayas/omnimind.git
cd omnimind
npm install
cp .env.example .env
```

### Environment Variables

```env
OPENAI_API_KEY=your_openai_api_key
PINECONE_API_KEY=your_pinecone_api_key
PINECONE_ENVIRONMENT=us-east-1-aws
PINECONE_INDEX=omnimind
MONGODB_URI=mongodb://localhost:27017/omnimind
JWT_SECRET=your_super_secret_key
PORT=3000
```

### Run Locally

```bash
npm run dev        # development with hot reload
npm run build      # production build
npm start          # production server
```

App runs at `http://localhost:3000`

---

## 📁 Project Structure

```
omnimind/
├── src/
│   ├── agents/         # LangChain agent configs
│   ├── api/            # REST API routes
│   ├── auth/           # JWT middleware
│   ├── bot/            # Core chatbot + RAG pipeline
│   ├── channels/       # WhatsApp, Slack, Web adapters
│   ├── db/             # MongoDB models
│   └── knowledge/      # Document ingestion + vectorization
├── .env.example
├── package.json
└── tsconfig.json
```

---

## 🏗️ Architecture

```
Document Upload ──► Parser ──► OpenAI Embeddings ──► Pinecone
                                                          │
User Query ──► GPT-4 ◄── Retrieved Context (RAG) ◄───────┘
                │
          Channel Adapter
       ┌────────┼────────┐
   WhatsApp   Slack   Web Widget
```

---

## 👨‍💻 Author

**Shakti Vijay A S** — [GitHub](https://github.com/shaktivijayas) · [LinkedIn](https://linkedin.com/in/ShakthiVijay)

<div align="center">
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer&animation=twinkling" />
</div>
