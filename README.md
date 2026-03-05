# Hola, soy Andres Vallarino 👋

### Desarrollador Frontend & AI Engineer · Buenos Aires, Argentina 🇦🇷

Construyo productos digitales con foco en **experiencia de usuario**, **arquitecturas modernas** y las últimas prácticas de **Inteligencia Artificial**. Me especializo en React, pero lo que realmente me diferencia es la integración de **sistemas multi-agente de IA** en aplicaciones reales deployadas en producción.

---

## 🤖 Arquitectura Multi-Agente  

Diseño e implemento sistemas donde múltiples agentes de IA colaboran, se delegan tareas y se corrigen entre sí de forma autónoma.

```
         ┌──────────────────────────────────────┐
         │          ORQUESTADOR PRINCIPAL        │
         │           orchestrator.js             │
         │   planifica → ejecuta → valida        │
         └───────────────┬──────────────────────┘
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
   ┌────────────┐ ┌────────────┐ ┌────────────┐
   │  PLANNER   │ │   PROMPT   │ │   CRITIC   │
   │   AGENT    │ │   AGENT    │ │   AGENT    │
   │            │ │            │ │            │
   │ Estructura │ │ Construye  │ │ Evalúa y   │
   │ el plan de │ │ el prompt  │ │ mejora la  │
   │ pasos      │ │ dinámico   │ │ respuesta  │
   └────────────┘ └────────────┘ └────────────┘
                         │
                  ┌──────▼──────┐
                  │ AgentContext │
                  │  (memoria    │
                  │ compartida)  │
                  └──────┬──────┘
                         │
                ┌────────▼────────┐
                │  Claude 3 Haiku  │
                │  Anthropic API   │
                │  via Serverless  │
                │  Vercel Function │
                └─────────────────┘
```

**Patrones implementados:**
- 🧠 **Memoria compartida** entre agentes via `AgentContext` (store centralizado)
- 🔄 **Loop de ejecución dinámico** - el Planner decide en runtime qué agentes correr y en qué orden
- ✅ **Autocorrección** - el Critic revisa la calidad y reescribe si no es suficiente
- 🔀 **Fallback inteligente** - modo `DEMO_MODE` sin consumir tokens API para portfolio
- ⚡ **Serverless** - endpoint `/api/generate-reading.js` deployado como Vercel Function
- 🔐 **Variables de entorno seguras** - `ANTHROPIC_API_KEY` nunca expuesta al frontend

---

## 🚀 Proyectos Destacados

### 🔮 [Arcana Mística](https://github.com/AndyV01/arcana-mystica) - [LIVE DEMO](https://arcana-mystica.vercel.app)

App de Tarot con **sistema multi-agente de IA** real integrado. Las interpretaciones son generadas por 3 agentes especializados que planifican, ejecutan y se autocorrigen usando **Claude 3 Haiku** via Anthropic API en una Serverless Function de Vercel.

`React 18` `Vite 5` `Multi-Agent AI` `Anthropic API` `Serverless` `Node.js` `i18n EN/ES`

- 🤖 Orquestador + 3 agentes (Planner · Prompt · Critic) con contexto compartido
- 🔮 78 cartas, 4 tiradas, flip 3D, numerología y zodíaco personalizado
- 🌟 Carta del día · Horóscopo semanal · Diario persistente · Tarjeta para compartir
- ⚡ Vercel Serverless Function con API key segura en variables de entorno

### 🤖 [Job Assistant AI](https://github.com/AndyV01/job-assistant-ai)
Sistema multi-agente con LLM tool calling real (Groq + LangChain), CV Optimizer y datos reales via Adzuna API. Backend Python + FastAPI, Frontend React, deployado en Railway y Vercel.

 `Python` `FastAPI` `LangChain` `LagGraph` `Groq API` `RAG` `Adzuna API` `React` `Vite` `TailwindCSS`

🔗 [Repo](https://github.com/AndyV01/job-assistant-ai) | 🌐 [Demo](https://job-assistant-ai-tzle.vercel.app/)

### 🛒 [E-Commerce React](https://github.com/AndyV01/E-commerce_React)
Tienda online completa con carrito, filtros y gestión de estado.
`React` `JavaScript` `CSS`

### 💼 [Portfolio Next.js](https://portfolio-nextjs-nine-lac.vercel.app/)
Portfolio profesional con SSR y optimización de imágenes.
`Next.js` `TypeScript` `Vercel`

---

## 🛠 Stack Tecnológico

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)

**IA & Agentes**

![Anthropic](https://img.shields.io/badge/Anthropic_API-CC785C?style=for-the-badge&logo=anthropic&logoColor=white)
![Multi-Agent](https://img.shields.io/badge/Multi--Agent_AI-7C3AED?style=for-the-badge&logo=openai&logoColor=white)
![Serverless](https://img.shields.io/badge/Serverless-FD5750?style=for-the-badge&logo=serverless&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=chainlink&logoColor=white) 
![LangGraph](https://img.shields.io/badge/LangGraph-4B8BBE?style=for-the-badge&logoColor=white)
![RAG](https://img.shields.io/badge/RAG_FAISS-00ADD8?style=for-the-badge&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logoColor=white)
![LLMToolCalling](https://img.shields.io/badge/LLM_Tool_Calling-7B61FF?style=for-the-badge&logoColor=white)


**Backend & Deploy**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white)

---

## 🌱 Aprendiendo ahora

- **Arquitecturas Multi-Agente** - orquestación, memoria compartida, autocorrección
- **LangChain / LangGraph** - frameworks para pipelines de agentes complejos
- **LLM Tool Calling** - agentes con tools reales via LangChain + Groq
- **TypeScript avanzado** - tipos genéricos y patrones de diseño

---

## 📫 Contacto

[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://portfolio-nextjs-nine-lac.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AndyV01)

---

<div align="center">

*"El código es poesía - cada función una estrofa, cada proyecto una historia."*

⭐ Si algún proyecto te sirvió, un star hace la diferencia

</div>

<!--
**AndyV01/AndyV01** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
