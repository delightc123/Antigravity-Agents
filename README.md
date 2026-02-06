# 🚀 Antigravity Agents

> **A comprehensive collection of specialized AI agent profiles designed to supercharge your development workflow with Google Antigravity (Gemini CLI).**

Antigravity Agents is a curated set of custom agent personas that transform your AI coding assistant into a full-fledged development team. Each agent has distinct expertise, behavioral guidelines, and operational constraints — enabling focused, high-quality outputs across every layer of your SaaS product.

---

## 🌟 Why Use Antigravity Agents?

- **Specialized Expertise**: Each agent is a master-level specialist in their domain
- **Consistent Quality**: Agents follow strict operational constraints and best practices
- **Team Collaboration**: Agents are designed to coordinate with each other via the Agent Orchestrator
- **Production-Ready Outputs**: Every deliverable is designed to be clean, documented, and maintainable
- **Atomic Design Principles**: Built-in adherence to Brad Frost's Atomic Design methodology
- **Research-Driven**: Agents continuously reference best practices and modern standards

---

## 📦 What's Included

### Agent Orchestrator

**`Agent-Orchestrator.md`** — _Alexander Reed_

> The central nervous system of your AI organization. Routes tasks to the correct agents, maintains system-wide coherence, resolves conflicts, and ensures outputs meet quality standards.

---

### 🧠 AI & Machine Learning

| Agent                           | Persona        | Focus Area                                                      |
| ------------------------------- | -------------- | --------------------------------------------------------------- |
| **AI_Product_Engineer.md**      | Adrian Volkov  | AI copilots, assistants, prompt systems, AI UX patterns         |
| **LLM_Integration_Engineer.md** | Victor Hammond | LLM API integration, RAG pipelines, tool calling, observability |
| **ML_Pipeline_Engineer.md**     | —              | ML model training, deployment, data pipelines                   |

---

### 📈 Analytics & Growth

| Agent                     | Persona        | Focus Area                                             |
| ------------------------- | -------------- | ------------------------------------------------------ |
| **Analytics_Engineer.md** | —              | Data pipelines, dashboards, metrics infrastructure     |
| **Growth_Engineer.md**    | Natalie Foster | Conversion optimization, A/B testing, onboarding flows |

---

### ⚙️ Backend & Infrastructure

| Agent                         | Persona     | Focus Area                                                        |
| ----------------------------- | ----------- | ----------------------------------------------------------------- |
| **Backend.md**                | Marcus Liu  | APIs, Supabase, business logic, webhooks, background jobs         |
| **Database_Architect.md**     | —           | Schema design, migrations, query optimization, data modeling      |
| **Infra_Cloud_Architect.md**  | —           | Cloud infrastructure, CI/CD, scaling, deployments                 |
| **Security_Engineer.md**      | Daniel Osei | Zero-trust security, authentication, RBAC, encryption, compliance |
| **Billing_Payments_Agent.md** | —           | Payment integration, subscriptions, invoicing                     |

---

### 🎨 Frontend Development

| Agent                       | Persona    | Focus Area                                                     |
| --------------------------- | ---------- | -------------------------------------------------------------- |
| **Frontend.md**             | Daniel Kim | Next.js, React 18, TypeScript, SSR, performance, Atomic Design |
| **Mobile_App_Architect.md** | —          | Flutter, mobile-first design, cross-platform development       |
| **Performance_Engineer.md** | —          | Core Web Vitals, bundle optimization, runtime performance      |

---

### 🎯 Product Strategy & Management

| Agent                   | Persona    | Focus Area                                                     |
| ----------------------- | ---------- | -------------------------------------------------------------- |
| **Product_Manager.md**  | Laura Chen | PRDs, roadmapping, feature prioritization, MVP scoping         |
| **SaaS_Architect.md**   | —          | System architecture, technical decisions, scalability planning |
| **Sprint_priotizer.md** | —          | Sprint planning, backlog grooming, task prioritization         |
| **Meta.md**             | —          | Cross-agent coordination, strategic alignment                  |

---

### ✨ UI/UX Design

| Agent                            | Persona       | Focus Area                                                      |
| -------------------------------- | ------------- | --------------------------------------------------------------- |
| **UI.md**                        | Olivia Harper | Visual design, component implementation, Glassmorphism, 3D      |
| **UX.md**                        | Ethan Clarke  | User flows, wireframes, information architecture, accessibility |
| **Design_System_Architect.md**   | —             | Design tokens, theming, component library governance            |
| **Cinematic_Motion_Director.md** | Isabella Cruz | GSAP, scroll animations, cinematic storytelling, transitions    |
| **3D_Experience_Engineer.md**    | —             | Three.js, WebGL, immersive 3D experiences                       |
| **Whimsy_Injector.md**           | —             | Micro-interactions, delightful animations, brand personality    |
| **Accessibility_Engineer.md**    | —             | WCAG compliance, a11y auditing, inclusive design                |

---

### 🧪 QA & Reliability

| Agent                            | Persona    | Focus Area                                           |
| -------------------------------- | ---------- | ---------------------------------------------------- |
| **QA_Automation_Engineer.md**    | —          | Unit/E2E testing, regression safety, test automation |
| **Error_Observability_Agent.md** | Sophia Lin | Monitoring, logging, incident response, SLO/SLA      |

---

## 🔧 Installation

### Option 1: Global Installation (Recommended)

Install the agents globally so Antigravity uses them across **all your workspaces**.

#### Step 1: Clone the Repository

```bash
# Navigate to your Antigravity config directory
cd ~/.gemini

# Clone the agents repository
git clone https://github.com/YOUR_USERNAME/antigravity-agents.git .agents
```

> **Note**: Replace `YOUR_USERNAME` with your actual GitHub username.

#### Step 2: Add the Global Rule

Add the following rule to your Antigravity global settings. Create the file if it doesn't exist:

**File: `~/.gemini/settings.json`** (or your global Antigravity config)

Alternatively, add this to your **global Antigravity rules**:

```
Always work with agent_orchestrator.md and switch between subagents when working
Always work with your agents and switch between agents in .agents/ and work with Agent-Orchestrator.md
```

You can add these rules via the Antigravity settings UI or by editing your global memory/rules file:

**File: `~/.gemini/MEMORY_global.md`** or add to your user rules:

```markdown
Always work with agent_orchestrator.md and switch between subagents when working
ALways work with you agent and switch between agent in .agents/ and work with agents_orchestrator.md
```

#### Step 3: Verify Installation

Start Antigravity in any workspace and verify the agents are recognized:

```bash
# In any project directory
antigravity

# Ask Antigravity to list available agents
> "What agents do you have access to?"
```

---

### Option 2: Per-Workspace Installation

If you prefer to have the agents only in specific workspaces:

#### Step 1: Clone Directly to Your Workspace

```bash
# Navigate to your project root
cd /path/to/your/project

# Clone the agents repository
git clone https://github.com/YOUR_USERNAME/antigravity-agents.git .agents
```

#### Step 2: Add Workspace-Level Rules

Create or edit `.gemini/settings.json` or add a `MEMORY.md` file in your workspace root with:

```markdown
Always work with agent_orchestrator.md and switch between subagents when working
Always work with your agents and switch between agents in .agents/ and work with Agent-Orchestrator.md
```

Alternatively, you can add this to your workspace's Antigravity configuration.

---

## 📖 Usage

### Basic Workflow

1. **Start with the Orchestrator**: When working on complex tasks, Antigravity will consult the Agent Orchestrator to determine which specialized agents to invoke.

2. **Direct Agent Invocation**: You can explicitly request a specific agent:

   ```
   > "Use the Frontend agent to implement this React component"
   > "Switch to the Security Engineer for an auth review"
   > "Have the UX agent design the user flow for onboarding"
   ```

3. **Multi-Agent Collaboration**: Complex features automatically trigger coordination:
   ```
   > "Build a dashboard with real-time analytics"
   # This may invoke: Frontend, Backend, UI, UX, and Analytics agents
   ```

### Example Prompts

```plaintext
# Frontend Development
"Use Daniel Kim (Frontend agent) to build a responsive dashboard page with GSAP animations"

# Backend API
"Have Marcus Liu (Backend agent) implement a Supabase Edge Function for user authentication"

# UI Design
"Ask Olivia Harper (UI agent) to create a Glassmorphic card component with dark mode support"

# Security Review
"Get Daniel Osei (Security Engineer) to audit the authentication flow for vulnerabilities"

# Full Feature
"Orchestrate the team to build a complete user settings page with profile updates,
password change, and notification preferences"
```

---

## 🏗️ Agent Structure

Each agent file follows a consistent structure:

```markdown
## Agent Name: [Name] – [Title]

**Persona:** [Description of the agent's personality and approach]

**Operational Constraints:** [Hard rules the agent must follow]

**Responsibility:** [What the agent owns]

**Skills:** [Technical capabilities]

**Role:** [Position in the team hierarchy]

**Steps:** [Execution workflow]

**Tasks:** [Specific deliverables]

**Requirements:** [Quality standards]

**Behavioral Guidelines:** [How the agent behaves]

**Few-Shot Examples:** [Sample use cases]

**Output Protocol:** [What deliverables look like]

**Tone:** [Communication style]

**Ensures Consistency & Alignment:** [Cross-agent coordination]

**Tools:** [Technologies and frameworks used]
```

---

## 🤝 Agent Relationships

```
                    ┌─────────────────────────────────────┐
                    │       Agent Orchestrator            │
                    │       (Alexander Reed)              │
                    │    Routes & Coordinates All         │
                    └─────────────────┬───────────────────┘
                                      │
        ┌─────────────────────────────┼─────────────────────────────┐
        │                             │                             │
        ▼                             ▼                             ▼
┌───────────────┐           ┌───────────────┐           ┌───────────────┐
│   Product     │           │   Design      │           │  Engineering  │
│   Strategy    │◄─────────►│   (UI/UX)     │◄─────────►│  (FE/BE/Infra)│
└───────────────┘           └───────────────┘           └───────────────┘
        │                             │                             │
        ▼                             ▼                             ▼
┌───────────────┐           ┌───────────────┐           ┌───────────────┐
│   Analytics   │           │     AI/ML     │           │  QA/Security  │
│   & Growth    │           │  Integration  │           │  & Reliability│
└───────────────┘           └───────────────┘           └───────────────┘
```

---

## 🎯 Best Practices

1. **Let the Orchestrator Work**: For complex tasks, let the Agent Orchestrator route to the right specialists
2. **Be Specific**: When invoking agents directly, be clear about what you need
3. **Trust the Constraints**: Each agent has operational rules — they're designed for production-quality output
4. **Iterate with Handoffs**: Allow agents to collaborate by trusting their coordination protocols
5. **Review Outputs**: While agents aim for production-ready code, always review critical changes

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙏 Credits

Created and maintained by the community. Feel free to fork, customize, and contribute!

---

## 🐛 Issues & Contributions

Found a bug or want to add a new agent? Open an issue or submit a pull request!

```bash
# Fork the repo
# Create your feature branch
git checkout -b feature/new-agent

# Commit your changes
git commit -m "Add DevOps Agent"

# Push to the branch
git push origin feature/new-agent

# Open a Pull Request
```

---

**Happy Building! 🎉**

_Transform your AI assistant into a full development team with Antigravity Agents._
