> **Architecting the future of prompt-driven infrastructure.**

Prompter is a premium SaaS DevTools platform engineered to help principal architects and senior developers design, formalize, and deploy highly structured schema-driven prompts.

<img width="1919" height="906" alt="image" src="https://github.com/user-attachments/assets/5eb42f28-6dcb-426d-afe1-f3e5e7a202eb" />
 

## 🚀 Features

- **Architecture Engine:** Define high-fidelity, highly reproducible LLM prompt architectures.
- **Microservice Mapping:** Turn simple ideas into concrete Mermaid.js structural flowcharts with precise component abstractions.
- **History & Retention:** Access an intuitive sidebar with 1-click retrieval of up to 25 of your past iterations synchronously.
- **Enterprise Authenticated:** Built with robust JWT tokens and Row-Level-Security (RLS) policies targeting 0-trust deployments via Supabase.
- **Dynamic & Edge-Ready UI:** React 19 + Tailwind v4 + Vite stack packed with rich mesh gradients, micro-animations, and glassmorphism.

<img width="1917" height="900" alt="image" src="https://github.com/user-attachments/assets/3d2fb56e-c26c-4626-aeb7-fa77a213e0c5" />
<img width="1919" height="906" alt="image" src="https://github.com/user-attachments/assets/db4415a9-dca7-42d8-b93c-4fb3b311bf87" />
<img width="1919" height="906" alt="image" src="https://github.com/user-attachments/assets/431bfe06-5356-4b7d-b742-369230215e20" />

## 🛠 Tech Stack

- **Frontend:** React 19, TypeScript, Vite
- **Styling:** Tailwind CSS v4, Custom CSS variables
- **Authentication & Database:** Supabase (`pg_graphql`, PostgREST API)
- **AI Processing:** Groq inference engine (`llama-3.1-8b-instant`)
- **Visuals:** Canvas confetti, Sonner toasts, and Lucide/Material icons

---

## 💻 Getting Started (Local Development)

### 1. Clone the repository
```bash
git clone https://github.com/oasis-parzival/Prompter.git
cd prompter
```

### 2. Install dependencies
```bash
npm install
```

### 3. Environment Configuration
Copy `.env.example` to `.env` and fill in your secure integration keys:
```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_PUBLISHABLE_KEY=your_supabase_anon_key
VITE_GROQ_API_KEY=your_groq_api_key
```
*Note: Never push your live `.env` to Version Control! Ensure `.gitignore` is tracking it.*

### 4. Seed your Database
Navigate to your Supabase web console and execute the SQL file located in `supabase/schema.sql` into your project's SQL editor to trigger table and RLS generation.

### 5. Run the Local Server
```bash
npm run dev
```

## 📸 Component Showcase
<img width="1919" height="906" alt="image" src="https://github.com/user-attachments/assets/db4415a9-dca7-42d8-b93c-4fb3b311bf87" />


### Architecture
- `<Sidebar />`: Fully real-time bounded project tracking component.
- `<Dashboard />`: The core LLM loop mapping structural states to UI visually using Mermaid.
- `<AuthContext />`: Robust multi-tab compatible context lock avoiding React 18 strict mode deadlocks natively.

## 📄 License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
