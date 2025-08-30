# ⚡ Claude Autopilot
> **Transform feature ideas into production code in 15 minutes**

[![GitHub stars](https://img.shields.io/github/stars/croffasia/claude-code-prp-generator?style=social)](https://github.com/croffasia/claude-code-prp-generator)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code](https://img.shields.io/badge/Claude-Code-blue)](https://claude.ai/code)
[![Threads / Open Source Alternatives](https://img.shields.io/badge/Threads-OpenSourceAlternatves-black)](https://www.threads.com/@opensourcealternatives)

Stop spending hours on features that should take minutes. One Claude Code command generates a complete implementation plan, another delivers production-ready code with tests.

```bash
/brainstorm Add user authentication with OAuth2
# → Smart feature planning session → docs/brainstorming/2025-08-22-user-auth.md

/prp:generate @docs/brainstorming/2025-08-22-user-auth.md
# OR directly: /prp:generate Add user authentication with OAuth2
# → Complete implementation blueprint → docs/prps/user-auth.md

/prp:execute @docs/prps/user-auth.md  
# → Working auth system (direct PRP execution for simple features)

/task:execute @docs/tasks/user-auth.md
# → Execute all tasks from breakdown (for complex features)
```

**Before**: 2-4 hours of coding, debugging, and integration  
**After**: 15 minutes → Production-ready feature ✨

> ⭐ **Found this helpful? Star the repo and hit Watch** to get notified of new updates!

## 🔥 Why Developers Love It

- **⚡ 10x Faster Development** - Feature idea to production in one session
- **🎯 Zero "Vibe Coding"** - AI follows your exact patterns and conventions
- **🧠 Opus-Powered Planning** - Deep research and smart blueprints, Sonnet-fast execution
- **✅ Built-in Quality** - Validation gates and linting included automatically
- **🚀 Any Tech Stack** - React, Python, Go, PHP - works everywhere

## 🚀 Quick Start

### How to Install

**🚀 Easiest Way (Recommended)**

Simply use this prompt in your Claude Code project:

```
Install Claude PRP Generator from https://github.com/croffasia/claude-code-prp-generator:
1. Clone the repository
2. Copy with replacement:
    2.1 claude/commands/* to .claude/commands/ 
    2.2 claude/agents/* to .claude/agents/
    2.3 docs/templates/* to ./docs/templates/
3. Study how all toolkit commands work and show me usage examples: /brainstorm, /prp:generate, /prp:execute, /task:execute
```

**📋 Manual Installation**

1. **Clone the Repository**
   ```bash
   git clone https://github.com/croffasia/claude-code-prp-generator.git
   cd claude-code-prp-generator
   ```

2. **Copy Commands and Agents to Claude Code**

   **Option A: Global Installation**
   ```bash
   # Copy commands and agents to your global Claude Code configuration
   cp -r claude/* ~/.claude/
   ```

   **Option B: Project-Specific Installation**
   ```bash
   # Copy commands and agents to your project's .claude directory
   cp -r claude/* .claude/
   ```

3. **Copy Templates to Your Project**
   ```bash
   # In your target project directory
   cp -r /docs/* ./docs/
   cp -r /docs/* ./docs/
   ```


## 🎯 Commands

### 1. **Think Through Your Feature** (`/brainstorm`)
- Smart AI Scrum Master guides you through structured planning
- Asks the right questions to uncover hidden requirements
- Creates comprehensive feature documentation → `docs/brainstorming/feature-session.md`
- Perfect for solo developers who need a thinking partner

### 2. **Create Perfect Plan** (`/prp:generate`)
- Validates your request is complete (may ask clarifying questions)
- Studies your codebase patterns
- Researches external docs if needed
- Creates detailed implementation plan → `docs/prps/feature-name.md`
- Breaks down into technical tasks → `docs/tasks/feature-name.md`

### 3. **Execute the Plan** (`/prp:execute`)
- Follows your patterns exactly
- Writes production-ready code
- Runs tests and linting
- Validates everything works

### 4. **Execute Tasks** (`/task:execute`)
- Breaks down complex features into manageable tasks
- Executes task-by-task with validation
- Perfect for large implementations
- Systematic progress tracking

> **Smart Model Selection**: Opus handles complex planning and research, Sonnet executes fast implementation - best of both worlds!

## 🎯 How It Works

### 🧠 Full Feature Development Flow
**brainstorm → prp:generate → execute**

1. **Start with Ideas** - Use `/brainstorm` when you need to explore and refine feature concepts
2. **Generate Implementation Plan** - Use `/prp:generate` to create detailed technical specifications  
3. **Choose Your Execution Path**:
   - **Simple Features**: `/prp:execute` - Direct implementation for straightforward tasks
   - **Complex Features**: `/task:execute` - Step-by-step implementation with progress tracking

### 🚀 Quick Implementation Flow
**prp:generate → execute**

Skip brainstorming when you have clear requirements:
1. **Generate Plan**: `/prp:generate`
2. **Execute**: Choose `/prp:execute` for simple features or `/task:execute` for complex ones

> **Pro Tip**: Use `/task:execute` for higher quality first-pass implementations on complex features

## 💎 What You Get

### 🤖 Specialized AI Agents
- **Preflight PRP Agent** (`preflight-prp`) - Validates task completeness and identifies missing business logic
- **Codebase Research Agent** (`codebase-research`) - Deep pattern discovery and internal architecture analysis
- **External Research Agent** (`research-agent`) - Comprehensive external documentation and best practices research
- **Team Lead Task Breakdown Agent** (`team-lead-task-breakdown`) - Breaks down PRP documents into manageable development tasks

> **Note**: All agents are configured to use Opus for optimal planning quality. You can remove the `model: opus` line from agent files to use your default Claude Code model instead.

### ⚙️ Works With Everything
- **Frontend**: React, Vue, Angular, Svelte
- **Backend**: Node.js, Python, Go, PHP, Java
- **Mobile**: React Native, Flutter, Swift, Kotlin

## 📊 Real Results

- **Development Speed**: Dramatically faster feature delivery
- **Code Quality**: Higher (follows existing patterns)
- **Technical Debt**: Zero (uses established conventions)
- **Completeness**: AI asks clarifying questions to fill gaps
- **Validation**: Built-in linting and project checks

## 📁 What's Included

```
📦 claude-code-prp-generator/
├── 🤖 claude/agents/           # Smart research agents
├── ⚡ claude/commands/          # Claude Code Commands  
└── 📚 docs/templates/          # Templates
```

## 🎯 Perfect For

- **Solo Developers** - Get team-level productivity + AI thinking partner for feature planning
- **Agencies** - Handle diverse client projects efficiently
- **Startups** - Ship features 10x faster with structured planning
- **Large Teams** - Maintain consistency across developers

## 🤝 Join the Community

- ⭐ **Star this repo** if it saves you hours
- 🍴 **Fork** to customize for your stack
- 💬 **Issues** for questions and feature requests
- 🔄 **PRs welcome** for new agents and improvements

## 📄 License

MIT License - Use freely in commercial projects

## 💝 Support the Project

If this toolkit saved you hours of development time, consider supporting with a crypto donation:

- **USDT TRC-20**: `TMSdmfoEVkC4sA1ejmhimcZC4eSremmkjV`
- **USDT Ton Network, TON**: `UQCqxsLGm8ftJvItaZaNrfE2o1RE2G2SV0FHP8pfXluXOAZv`
- **USDT ERC20**: `0x625d8E7e800E863d1b00D90c8937A10094D9380C`

---

**Ready to stop wasting hours on features?** [Install now](#quick-start) and experience autonomous development! 🚀

[![GitHub stars](https://img.shields.io/github/stars/croffasia/claude-code-prp-generator?style=social)](https://github.com/croffasia/claude-code-prp-generator)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code](https://img.shields.io/badge/Claude-Code-blue)](https://claude.ai/code)
[![Threads / Open Source Alternatives](https://img.shields.io/badge/Threads-OpenSourceAlternatves-black)](https://www.threads.com/@opensourcealternatives)

**v1.3.0** | *Updated: August 30, 2025*