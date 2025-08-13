# 🚀 Claude Code PRP Generator

> **AI-Powered Product Requirements with Patterns (PRP) Generator for Claude Code CLI**

Transform the chaos of "vibe coding" into systematic, production-ready development. Generate context-rich PRPs that turn feature ideas into self-executing implementation blueprints, reducing development time from hours to minutes while maintaining code quality.

## 🎯 Why PRP for AI Development?

Traditional AI coding often produces random, disconnected code that doesn't integrate well with your existing codebase. The **Product Requirements with Patterns (PRP)** approach solves this by treating AI like a well-briefed team member:

- **⚡ 10x Faster Development** - From feature idea to production-ready code in one pass
- **🎨 Perfect Pattern Matching** - AI mirrors your existing codebase conventions exactly  
- **🧠 Context-Rich Specifications** - Eliminate back-and-forth iterations with comprehensive context
- **✅ Built-in Quality Gates** - Automated validation ensures production-ready code
- **🔄 Zero Technical Debt** - Follow established patterns instead of creating new ones

> *"Literally 3 prompts and 15 minutes, and I am ready to get feedback on something I would have agonized over for at least 2 hours."* - Modern development with structured AI workflows

## ✨ Features

- **🎯 Universal Templates** - Framework-agnostic PRP templates that work with any language or architecture
- **🔍 Intelligent Research** - Automated codebase analysis and external documentation discovery
- **⚡ Self-Validating** - Built-in validation loops with executable tests and linting integration
- **🧠 Context-Rich** - Information-dense specifications that enable one-pass implementation
- **🔄 Progressive Success** - Start simple, validate, then enhance methodology
- **📋 Task Management** - Integrated TodoWrite tracking for complex multi-step implementations

## 🏗️ Architecture

The PRP Generator follows a three-phase approach:

### 1. **Research & Generation Phase**
```
Feature Specification → Codebase Analysis → External Research → Comprehensive PRP
```

### 2. **Implementation Phase**
```
PRP Loading → Pattern Analysis → Code Generation → Validation Gates → Refinement
```

### 3. **Validation Phase**
```
Syntax Check → Type Check → Tests → Build → Manual Verification
```

## 🚀 Quick Start

### Installation

1. **Copy Commands to Claude Code**
   
   **Option A: Global Installation (Recommended)**
   ```bash
   # Copy commands to your global Claude Code configuration
   cp -r claude/commands ~/.claude/commands/
   ```
   
   **Option B: Project-Specific Installation**
   ```bash
   # Copy commands to your project's .claude directory
   mkdir -p .claude/commands
   cp -r claude/commands/* .claude/commands/
   ```

2. **Copy PRP Templates to Your Project**
   ```bash
   # In your target project directory
   cp -r /path/to/claude-code-prp-generator/PRPs/ ./PRPs/
   ```

### Basic Usage

1. **Generate a PRP**
   ```bash
   # Option A: From feature specification file
   /generate-prp @feature-specification.md
   
   # Option B: Direct task description
   /generate-prp Add user authentication with OAuth2 and JWT tokens
   ```

2. **Execute a PRP**
   ```bash
   # In Claude Code CLI
   /execute-prp @PRPs/my-feature.md
   ```

## 📁 Project Structure

```
claude-code-prp-generator/
├── claude/
│   └── commands/           # Claude Code command definitions
│       ├── generate-prp.md # PRP generation command
│       └── execute-prp.md  # PRP execution command
├── PRPs/
│   └── templates/         # Universal PRP templates
│       └── prp_base.md   # Framework-agnostic base template
├── CLAUDE.md             # Claude Code project guidance
└── README.md            # This file
```

## 🎨 PRP Template Structure

The universal PRP template includes:

- **Goal & Why** - Clear objectives and business value
- **Success Criteria** - Measurable outcomes
- **All Needed Context** - Documentation, references, and gotchas
- **Implementation Blueprint** - Step-by-step tasks with pseudocode
- **Integration Points** - Database, API, routing, and state management
- **Validation Loop** - Executable commands for quality assurance

## 🛠️ Commands

### `/generate-prp <feature-file>`

Creates a comprehensive PRP through automated research:

1. **Codebase Analysis** - Identifies similar patterns and conventions
2. **External Research** - Gathers documentation and best practices
3. **Context Assembly** - Builds information-dense implementation guide
4. **Validation Setup** - Configures project-specific quality gates

### `/execute-prp <prp-file>`

Implements features from PRP specifications:

1. **Load & Understand** - Parse PRP requirements and context
2. **Plan & Track** - Create TodoWrite implementation plan
3. **Pattern Mirroring** - Study and replicate reference implementations
4. **Iterative Implementation** - Code generation with validation loops
5. **Quality Assurance** - Run all validation gates until passing

## 🎯 Best Practices

### Creating Effective PRPs

- **Include Real Examples** - Reference actual files from your codebase
- **Document Gotchas** - Library quirks, version issues, common pitfalls
- **Specify Validation** - Exact commands for linting, testing, building
- **Reference Patterns** - Point to existing implementations to mirror

### Successful Implementation

- **Study References First** - Always read reference files before coding
- **Mirror Exactly** - Follow existing patterns for consistency
- **Validate Frequently** - Run checks after each major change
- **Use TodoWrite** - Track progress on complex multi-step features

## 🔧 Integration with Existing Projects

The PRP Generator works with any tech stack by:

1. **Analyzing Project Structure** - Identifies existing patterns and conventions
2. **Discovering Validation Tools** - Finds project-specific linting and testing commands  
3. **Adapting Templates** - Customizes universal template to project needs
4. **Maintaining Consistency** - Ensures new code follows established patterns

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Test your changes with real projects
4. Commit your changes (`git commit -m 'Add amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Ready to accelerate your AI-driven development?** Start by copying the commands to your Claude Code setup and experience autonomous feature implementation! 🚀
