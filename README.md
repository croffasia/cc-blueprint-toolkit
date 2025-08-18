# ⚡ Claude Autopilot
> **Transform feature ideas into production code in 15 minutes**

[![GitHub stars](https://img.shields.io/github/stars/croffasia/claude-code-prp-generator?style=social)](https://github.com/croffasia/claude-code-prp-generator)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code](https://img.shields.io/badge/Claude-Code-blue)](https://claude.ai/code)

Stop spending hours on features that should take minutes. One Claude Code command generates a complete implementation plan, another delivers production-ready code with tests.

```bash
/prp:generate "Add user authentication with OAuth2"
# → Complete implementation blueprint

/prp:execute @PRPs/user-auth.md  
# → Working auth system
```

**Before**: 2-4 hours of coding, debugging, and integration  
**After**: 15 minutes → Production-ready feature ✨

## 🔥 Why Developers Love It

- **⚡ 10x Faster Development** - Feature idea to production in one session
- **🎯 Zero "Vibe Coding"** - AI follows your exact patterns and conventions
- **🧠 Opus-Powered Planning** - Deep research and smart blueprints, Sonnet-fast execution
- **✅ Built-in Quality** - Validation gates and linting included automatically
- **🚀 Any Tech Stack** - React, Python, Go, PHP - works everywhere

> *"Literally 3 prompts and 15 minutes, and I am ready to get feedback on something I would have agonized over for at least 2 hours."*

## 🚀 Quick Start

### Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/croffasia/claude-code-prp-generator.git
   cd claude-code-prp-generator
   ```

2. **Copy Commands and Agents to Claude Code**

   **Option A: Global Installation (Recommended)**
   ```bash
   # Copy commands and agents to your global Claude Code configuration
   cp -r claude/commands ~/.claude/commands/
   cp -r claude/agents ~/.claude/agents/
   ```

   **Option B: Project-Specific Installation**
   ```bash
   # Copy commands and agents to your project's .claude directory
   mkdir -p .claude/commands .claude/agents
   cp -r claude/commands/* .claude/commands/
   cp -r claude/agents/* .claude/agents/
   ```

3. **Copy PRP Templates to Your Project**
   ```bash
   # In your target project directory
   cp -r /path/to/claude-code-prp-generator/PRPs/ ./PRPs/
   ```

### Basic Usage

```bash
# 1. Generate a feature plan
/prp:generate "Add user authentication with OAuth2 and JWT tokens"

# 2. Execute the plan  
/prp:execute @PRPs/user-auth.md

# 3. Done! ✨
```

## 🎯 How It Works

### 1. **Create Perfect Plan** (`/prp:generate`)
- Validates your request is complete
- Studies your codebase patterns
- Researches external docs if needed
- Creates detailed implementation plan

### 2. **Execute the Plan** (`/prp:execute`)
- Follows your patterns exactly
- Writes production-ready code
- Runs tests and linting
- Validates everything works

> **Smart Model Selection**: Opus handles complex planning and research, Sonnet executes fast implementation - best of both worlds!

## 💎 What You Get

### 🤖 Specialized AI Agents
- **Surface Discovery Agent** (Opus) - Validates task completeness and identifies missing business logic
- **Codebase Research Agent** (Opus) - Deep pattern discovery and internal architecture analysis
- **External Research Agent** (Opus) - Comprehensive external documentation and best practices research

### ⚙️ Works With Everything
- **Frontend**: React, Vue, Angular, Svelte
- **Backend**: Node.js, Python, Go, PHP, Java
- **Databases**: PostgreSQL, MySQL, MongoDB
- **Cloud**: AWS, Vercel, Railway, any platform

## 📊 Real Results

- **Development Speed**: Dramatically faster feature delivery
- **Code Quality**: Higher (follows existing patterns)
- **Technical Debt**: Zero (uses established conventions)
- **Validation**: Built-in linting and project checks

## 🛠️ Commands

| Command | Purpose | Example |
|---------|---------|---------|
| `/prp:generate` | Create implementation plan | `/prp:generate "Add file upload with S3"` |
| `/prp:execute` | Run the plan | `/prp:execute @PRPs/file-upload.md` |

## 📁 What's Included

```
📦 claude-code-prp-generator/
├── 🤖 claude/agents/           # Smart research agents
├── ⚡ claude/commands/         # Simple commands  
└── 📋 PRPs/templates/          # Universal PRP framework
```

## 🎯 Perfect For

- **Solo Developers** - Get team-level productivity
- **Agencies** - Handle diverse client projects efficiently
- **Startups** - Ship features 10x faster
- **Large Teams** - Maintain consistency across developers

## 🤝 Join the Community

- ⭐ **Star this repo** if it saves you hours
- 🍴 **Fork** to customize for your stack
- 💬 **Issues** for questions and feature requests
- 🔄 **PRs welcome** for new agents and improvements

## 📄 License

MIT License - Use freely in commercial projects

---

**Ready to stop wasting hours on features?** [Install now](#quick-start) and experience autonomous development! 🚀

[![GitHub stars](https://img.shields.io/github/stars/croffasia/claude-code-prp-generator?style=social)](https://github.com/croffasia/claude-code-prp-generator)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code](https://img.shields.io/badge/Claude-Code-blue)](https://claude.ai/code)

**v1.1.0** | *Updated: August 18, 2025*