# HealthWise 🧬
### **Precision Clinical Intelligence & Health Memory**

**HealthWise** is a high-end, data-driven clinical health companion designed to "remember and understand the user’s body over time." Moving beyond generic conversational AI, HealthWise leverages the latest in **Mistral AI** micro-models to reason over historical medical records, detect seasonal patterns, and provide structured clinical insights through a premium, glassmorphic interface.

---

## 🌟 The Core Vision: "Clinical Memory"
Most health assistants start every conversation from zero. **HealthWise is different.** It is built on the principle of **State-Aware Healthcare**, where the system:
- **Remembers**: Every past prescription, symptom, and diagnosis is stored as a high-dimensional vector.
- **Reasons**: Cross-references current complaints with historical data to find patterns.
- **Guides**: Uses a "Guided Discovery" protocol to build a comprehensive context tree for new users.

---

## ✨ Specialized Clinical Features

### 🧠 **Context-Aware Reasoning**
When a returning user enters a symptom, HealthWise doesn't just explain it—it analyzes it against their history. 
> *"I noticed you had a similar respiratory incident in Nov 2024. This suggests a seasonal recurring pattern."*

### 🔍 **Guided Discovery Protocol**
For new users with empty records, HealthWise enters **Discovery Mode**, using focused, progressive questions to build a high-trust clinical profile without information overload.

### 🖼️ **Pixtral Vision OCR**
Powered by **Mistral Pixtral-12B**, users can instantly upload prescriptions and medical documents. HealthWise extracts standardized clinical data (medications, dosages, diagnoses) with 95% confidence.

### 🍱 **Ayush Strategy Guardrails**
Integrated traditional wisdom (Ayush) provided as a complementary "Perspective" layer, sanitized by strict medical guardrails to ensure holistic yet safe advice.

### 💎 **Hybrid Clinical UI**
A state-of-the-art glassmorphic dashboard featuring:
- **Insight Cards**: Structured analysis with pattern types, evidence, and recommendations.
- **Guided Chips**: Interactive next-steps based on AI clinical reasoning.
- **Confidence Scoring**: Transparent metrics for all AI-generated insights.

---

## 🛠 High-End Tech Stack

- **Core Framework**: [Next.js 15+](https://nextjs.org/) (App Router)
- **UI Architecture**: [Tailwind CSS 4.0](https://tailwindcss.com/) (Modern CSS-first tokens)
- **AI Orchestration**: 
  - **Reasoning**: `ministral-3b-2512` (Micro-model optimized for clinical precision)
  - **Vision**: `pixtral-12b-2409` (Document OCR)
  - **Embeddings**: `mistral-embed-2312` (1024-dim Vector Search)
- **Database Layer**: [Supabase](https://supabase.com/) & [Prisma](https://www.prisma.io/)
- **Vector Search**: `pgvector` for RAG-driven clinical history retrieval.

---

## 🚀 Rapid Deployment

### 1. Initialize Project
```bash
git clone https://github.com/AkshatVerma-Code/HealthWise.git
cd HealthWise
npm install
```

### 2. Configure Environment
Create `.env.local` with your production-grade credentials:
```env
# AI Infrastructure
MISTRAL_API_KEY=your_mistral_key

# Database Infrastructure (Supabase Direct)
DATABASE_URL="postgresql://postgres.[ID]:5432/postgres"
DIRECT_URL="postgresql://postgres.[ID]:5432/postgres"
```

### 3. Launch Platform
```bash
# Seed the initial clinical patterns
npm run db:seed

# Start the development server
npm run dev
```

---

## 🛡️ Clinical Trust & Safety
HealthWise is built with **Resilience-First** engineering:
- **3-Layer Repair System**: Automatically corrects AI schema fluctuations (nesting, key renaming) before they reach the UI.
- **Professional Fallbacks**: Never dumps raw JSON. In case of parsing errors, the system provides a polished clinical apology.
- **Strict Guardrails**: Every response is passed through a sanitation layer to remove unauthorized medical advice and emphasize professional consultation.

---

## 🩺 Medical Disclaimer
HealthWise is an informational health memory tool and **is not a substitute for professional medical diagnosis**. Always consult a certified healthcare provider for medical decisions. In emergencies, please contact your local emergency services immediately.

---

**Built with ❤️ for the future of Personalized Clinical Intelligence.**
