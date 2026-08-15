<!-- ==================== HEADER / TERMINAL BANNER ==================== -->
<div align="center">

```ascii
   ____ ___  _   _  ____  _____   _     _____ _____ _   _ _____ 
  / ___/ _ \| \ | |/ ___|| ____| | |   | ____|  ___| \ | |_   _|
 | |  | | | |  \| | |  _ |  _|   | |   |  _| | |_  |  \| | | |  
 | |__| |_| | |\  | |_| || |___  | |___| |___|  _| | |\  | | |  
  \____\___/|_| \_|\____||_____| |_____|_____|_|   |_| \_| |_|  
```

# **Shivaaay Shayantanchak**
### **Quantitative Financial Engineer & Autonomous AI Agent Developer**
📍 *Bengaluru, Karnataka, India*

[![Finance & Quant](https://img.shields.io/badge/Domain-Quantitative_Finance-059669?style=for-the-badge&logo=line&logoColor=white)](#01-quantitative--computational-finance)
[![CFA Program](https://img.shields.io/badge/Credential-CFA_Candidate-D97706?style=for-the-badge&logo=analytics&logoColor=white)](#02-financial-analysis--cfa-core)
[![AI Agents](https://img.shields.io/badge/AI-Multi--Agent_Swarms-7C3AED?style=for-the-badge&logo=openai&logoColor=white)](#03-autonomous-ai-agents--llm-systems)
[![Full-Stack Dev](https://img.shields.io/badge/Stack-Full--Stack_TypeScript-2563EB?style=for-the-badge&logo=typescript&logoColor=white)](#04-full-stack--systems-development)

---

```bash
$ systemctl status developer-profile.service
● developer-profile.service - Quant + CFA + AI Agent Developer Profile (Shayantanchak)
     Loaded: loaded (/etc/systemd/system/developer-profile.service; enabled)
     Active: active (running) since 2026-08-16
     Engine: Multi-Agent LLM Router + High-Frequency Financial Computing
     Location: Bengaluru, KA, IND
     Status: "Building financial models and agentic fintech infrastructure"
```

</div>

<br/>

<!-- ==================== 01. FINANCE ==================== -->
## 📈 01. Quantitative & Computational Finance

> *Bridging mathematical finance with scalable computation to model markets, evaluate risk, and optimize portfolios.*

### 🛠 Core Competencies
* **Portfolio Theory & Optimization:** Markowitz Mean-Variance, Black-Litterman Model, Sharpe & Sortino Ratio Optimization.
* **Derivatives & Stochastic Calculus:** Options Pricing (Black-Scholes-Merton PDE, Monte Carlo Simulations, Binomial Trees), Greeks Calculation ($\Delta, \Gamma, \Theta, \nu$).
* **Financial Risk Analytics:** Value at Risk (VaR - Historical, Parametric, Monte Carlo), Expected Shortfall (CVaR), Stress Testing.
* **Integer Minor-Unit Accounting:** Building zero-drift financial ledgers maintaining exact integer precision (cents/satoshis) for zero IEEE-754 floating-point errors.

### 📐 Selected Quant Formula Snippets
<details>
<summary><b>Click to expand: Black-Scholes Call/Put Pricing Implementation (Python / NumPy)</b></summary>

```python
import numpy as np
from scipy.stats import norm

def black_scholes(S: float, K: float, T: float, r: float, sigma: float, option_type: str = "call") -> float:
    """Calculates Black-Scholes option price for European Options."""
    d1 = (np.log(S / K) + (r + 0.5 * sigma ** 2) * T) / (sigma * np.sqrt(T))
    d2 = d1 - sigma * np.sqrt(T)
    if option_type == "call":
        return S * norm.cdf(d1) - K * np.exp(-r * T) * norm.cdf(d2)
    elif option_type == "put":
        return K * np.exp(-r * T) * norm.cdf(-d2) - S * norm.cdf(-d1)
```
</details>

---

<!-- ==================== 02. CFA PROGRAM ==================== -->
## 🎓 02. Financial Analysis & CFA Core

> *Applying institutional rigor, ethical standards, and deep financial reporting analysis to asset valuation.*

### 🏆 CFA Journey & Focus Areas
- **Status:** CFA Program Candidate
- **Core Mastery:**
  - **Financial Reporting & Analysis (FRA):** Balance Sheet Deconstruction, Cash Flow Quality, Multi-Entity Consolidation, IFRS vs. US GAAP reconciliation.
  - **Corporate Issuer & Valuation:** Discounted Cash Flow (DCF) Modeling, Comparable Company Multiples (P/E, EV/EBITDA), LBO Floor Valuation.
  - **Fixed Income & Equity:** Yield Curve Dynamics, Duration/Convexity Management, Credit Default Swap (CDS) spreads.
  - **Ethical & Professional Standards:** Strict adherence to CFA Institute Code of Ethics.

### 📊 Valuation & Financial Modeling Projects
* **[WertBot](https://github.com/Shayantanchak/WertBot):** Integrated Football Field valuation generator comparing 52-Week High/Low, DCF Intrinsic Fair Value, Wall Street Targets, and LBO floors.
* **Dynamic Excel Export Engine:** Native spreadsheet export preserving active formula auditing (`=SUM(...)`, `=XIRR(...)`).

---

<!-- ==================== 03. AI AGENTS ==================== -->
## 🤖 03. Autonomous AI Agents & LLM Systems

> *Engineering autonomous multi-agent swarms, dynamic persona routers, and deterministic LLM tool callers for financial and business intelligence decision making.*

### 🧠 Agentic Architecture Stack
```
                           ┌───────────────────────────┐
                           │   Dynamic LLM Router      │
                           │ (Vertex AI / Gemini / GPT)│
                           └─────────────┬─────────────┘
                                         │
       ┌──────────────────┬──────────────┼──────────────┬──────────────────┐
       ▼                  ▼              ▼              ▼                  ▼
┌──────────────┐   ┌──────────────┐ ┌──────────┐ ┌──────────────┐ ┌──────────────┐
│  Agent PFM   │   │Card Concierge│ │Quant Algo│ │Market Research│ │Risk Guard    │
│ (Burn Rates) │   │ (MCC Matrix) │ │(Alloc.   │ │ (10-K/10-Q   │ │(Idempotency) │
└──────────────┘   └──────────────┘ └──────────┘ └──────────────┘ └──────────────┘
```

### ⚡ Key AI Agent Innovations & Projects
* **[Agent-Analytica](https://github.com/Shayantanchak/Agent-Analytica):** Autonomous multi-agent Business Intelligence platform built with Streamlit and OpenAI LLMs to replace traditional data analytics workflows.
* **[WertBot AI Router](https://github.com/Shayantanchak/WertBot):** Central routing mechanism orchestrating domain-specialized agents (Personal Finance Advisor, Credit Card Concierge, Global Quant Advisor, SEC Filings Analyzer).
* **[PhishLens-X](https://github.com/Shayantanchak/Phishlens-X):** Modern enterprise ML platform intercepting zero-day payloads in the browser using Explainable AI (XAI) fusion scoring.

---

<!-- ==================== 04. DEVELOPMENT ==================== -->
## 💻 04. Full-Stack & Systems Development

> *Building resilient, high-throughput monorepos, low-latency background workers, and secure microservice architectures.*

### 🧰 Technology Radar

| Category | Technologies & Tools |
|---|---|
| **Languages** | TypeScript, JavaScript (Node.js/Bun), Python, SQL (PostgreSQL), C++ / Rust |
| **Backend & Microservices** | NestJS, Express, gRPC (Protobuf), REST APIs, Redis Caching, Worker Threads |
| **Frontend & UI** | React 18, Vite, TailwindCSS, Recharts, Streamlit, Framer Motion |
| **Database & Infra** | PostgreSQL 16 (JSONB, Minor-unit schemas), Docker, Nginx, Linux, GitHub Actions CI/CD |
| **Security & Auth** | WebAuthn / Passkeys (FIDO2), JWT, Idempotency Headers, Immutable Audit Logging |

### 🚀 Featured Repositories

| Repository | Tech Stack | Description |
|---|---|---|
| 💳 **[WertBot](https://github.com/Shayantanchak/WertBot)** | `TypeScript` `NestJS` `React` `PostgreSQL` | Enterprise-grade, AI-powered financial co-pilot, card reward concierge, and neobanking platform. |
| 📊 **[Agent-Analytica](https://github.com/Shayantanchak/Agent-Analytica)** | `Python` `Streamlit` `OpenAI` | Fully autonomous multi-agent Business Intelligence platform. |
| 🛡 **[PhishLens-X](https://github.com/Shayantanchak/Phishlens-X)** | `TypeScript` `ML` `XAI` | Enterprise ML platform detecting zero-day browser payloads with Explainable AI scoring. |
| 💼 **[shayantanportfolio](https://github.com/Shayantanchak/shayantanportfolio)** | `TypeScript` `Next.js` `Framer Motion` | Interactive 3D engineering portfolio. |

---

<!-- ==================== METRICS & TELEMETRY ==================== -->
## 📊 Real-Time Developer Telemetry

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Shayantanchak&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="175" alt="GitHub Stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Shayantanchak&layout=compact&theme=tokyonight&hide_border=true" height="175" alt="Top Languages" />

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Shayantanchak&theme=tokyonight&hide_border=true" height="150" alt="Streak Stats" />

</div>

---

<!-- ==================== CONNECT ==================== -->
## 📫 Connect & Collaborate

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shayantan-c-b7839a1a5)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Shayantanchak)

</div>
