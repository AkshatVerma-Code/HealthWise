# HealthWise 🧬
### **Precision Clinical Intelligence & Longitudinal Health Memory**

![HealthWise Hero](file:///Users/rajatnathmishra/.gemini/antigravity/brain/0cca5593-a56b-4efe-9627-312ee0511ae3/healthwise_ui_mockup_1774724651255.png)

**HealthWise** is a production-grade, AI-orchestrated clinical health platform designed to "remember and understand the user’s body over time." Unlike generic chatbots, HealthWise functions as a **Cognitive Health Memory**, reasoning over historical records, detecting seasonal patterns, and providing structured clinical insights through a premium glassmorphic interface.

---

## 🌟 Core Philosophy: "Beyond Records"
Traditional healthcare is fragmented. HealthWise bridges the gap between historical clinical data and daily physiological wellness using three core architectural pillars:

1.  **State-Aware Reasoning**: Every interaction contributes to a growing context tree.
2.  **Guided Discovery**: A progressive onboarding protocol that builds a clinical baseline without information overload.
3.  **Resilience-First AI**: A 3-layer structural repair system that ensures 100% reliable clinical data parsing.

---

## ✨ A-Z Feature Suite

### 🧠 **Clinical Intelligence Engine**
- **Context-Aware Mode**: Automatically detects recurring illnesses by cross-referencing years of history.
- **Discovery Mode**: Conducts structured Socratic questioning for users with no prior data.
- **Pattern Recognition**: Identifies seasonal trends (e.g., "Recurring March URTI") and environmental triggers.

### 🖼️ **Document Intelligence (OCR)**
- Powered by **Mistral Pixtral-12B**, users can upload prescriptions, lab reports, and diet charts.
- Standardizes messy handwritten notes into structured JSON models (Medication, Dosage, Frequency).

### 🍱 **Holistic Integration (Ayush)**
- Provides a complementary "Ayush Perspective" layer based on Ministry of Ayush frameworks.
- Sanitized by strict medical guardrails to ensure holistic advice never compromises safety.

### 💎 **Next-Gen Clinical UI**
- **Insight Cards**: Premium glassmorphic cards displaying diagnoses, evidence, and next steps.
- **Guided Chips**: Dynamic, AI-suggested follow-up questions to deepen the diagnostic context.
- **Health Snapshot**: A real-time visualization of the user's current physiological state.

---

## 🛠 High-End Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Framework** | [Next.js 15+](https://nextjs.org/) (App Router, React 19) |
| **Styling** | [Tailwind CSS 4.0](https://tailwindcss.com/) (CSS-first tokens) |
| **Auth** | [Auth.js v5](https://authjs.dev/) (Google OAuth + Credentials) |
| **Database** | [Supabase](https://supabase.com/) + [Prisma](https://www.prisma.io/) |
| **Vector DB** | `pgvector` for Semantic Clinical Retrieval |
| **AI Reasoning** | `ministral-3b-2512` (Optimized for precision) |
| **AI Vision** | `pixtral-12b-2409` (Standardized OCR) |
| **AI Embedding** | `mistral-embed-2312` (1024-dim vectors) |

---

## 🚀 Installation & Setup (A-Z)

### 1. Prerequisites
- **Node.js**: v20.x or higher
- **Supabase Account**: For Postgres + Vector search
- **Mistral API Key**: For the reasoning and vision engine
- **Google Cloud Console**: For OAuth 2.0 credentials

### 2. Clone & Install
```bash
git clone https://github.com/AkshatVerma-Code/HealthWise.git
cd HealthWise
npm install
```

### 3. Database Initialization
1.  **Create a Supabase Project**.
2.  **Enable pgvector**: Run `CREATE EXTENSION IF NOT EXISTS vector;` in the SQL Editor.
3.  **Run Migrations**:
    ```bash
    npx prisma generate
    npx prisma db push
    ```

### 4. Environment Variables
Create a `.env.local` file with the following high-end configuration:

```env
# --- NEXTAUTH (OAUTH) ---
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your_nextauth_secret
# Required for ngrok/tunnels
AUTH_TRUST_HOST=true

# --- GOOGLE OAUTH ---
GOOGLE_CLIENT_ID="your_google_id"
GOOGLE_CLIENT_SECRET="your_google_secret"

# --- AI INFRASTRUCTURE (MISTRAL) ---
MISTRAL_API_KEY="your_mistral_key"

# --- DATABASE (SUPABASE) ---
# Use port 6543 for pooled connection (Prisma)
POSTGRES_PRISMA_URL="postgresql://postgres.[REF]:[PW]@aws-1-us-east-1.pooler.supabase.com:6543/postgres?pgbouncer=true"
# Use port 5432 for direct connection (Migrations)
POSTGRES_URL_NON_POOLING="postgresql://postgres.[REF]:[PW]@aws-1-us-east-1.pooler.supabase.com:5432/postgres"
```

### 5. Deployment with ngrok (Live Access)
To make your local clinical system "live" for testing:
1.  **Install ngrok**: `brew install ngrok`
2.  **Start Tunnel**:
    ```bash
    # Uses the pre-configured ngrok_live.yml for zero-binding errors
    ngrok http --config ngrok_live.yml 3000
    ```
3.  **Update Google Console**: Add your `ngrok` URL as an Authorized Redirect URI.

---

## 🛡️ Resilience & Safety Protocol

HealthWise implements a **3-Layer Structural Repair System** to ensure UI stability:
1.  **Unwrapping Layer**: Automatically detects and extracts JSON from markdown or nested model outputs.
2.  **Schema Hardening**: Maps fuzzy AI keys (e.g., `greeting` → `message`) to the strict TypeScript interface.
3.  **Professional Apology**: If the AI model fails the reasoning loop, the system returns a sanitized clinical apology rather than a raw error.

---

## 🩺 Medical Disclaimer
HealthWise is a longitudinal health memory and information tool. It **does not provide medical diagnosis**. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition. In case of emergency, contact your local emergency services immediately.

---

**Built with ❤️ by HealthWise Clinical Engineering.**
