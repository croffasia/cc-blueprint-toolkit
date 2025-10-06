# Vibe Coding Guide

10 essential tips for building projects with AI assistance

## Core Principles

### 1. Start Simple, Add Complexity Only When Needed
Find the simplest solution first. Don't build complex agentic systems when optimizing single LLM calls works. Add multi-step workflows only when simpler solutions fall short.

### 2. Be Extremely Specific in Your Instructions
The quality of AI output directly reflects the quality of your input. More specific instructions = better results on first attempt.

**Poor examples:**
- "add tests for foo.py"
- "why does ExecutionFactory have such a weird api?"
- "add a calendar widget"

**Good examples:**
- "write test cases for foo.py covering edge cases where user is logged out, avoid mocks"
- "look through ExecutionFactory's git history and summarize how its api came to be"
- "look at how existing widgets are implemented on the home page to understand the patterns. Follow the pattern to implement a calendar widget that lets users select a month and paginate forwards/backwards. Build from scratch without libraries other than the ones already used in the codebase."

### 3. Create and Maintain CLAUDE.md Files
Document everything AI needs to know about your project in the root directory:
- Common bash commands
- Core files and utility functions
- Code style guidelines
- Testing instructions
- Repository etiquette (branch naming, merge vs. rebase)
- Developer environment setup
- Any unexpected behaviors or warnings

Update it continuously. Check it into git so your team benefits.

### 4. Use Plan → Code → Validate Workflow
**Never let AI jump straight to coding.** Follow this sequence:

1. **Explore**: Ask AI to read relevant files (explicitly tell it NOT to write code yet)
2. **Plan**: Ask AI to make a plan (use "think" for extended thinking mode)
3. **Review**: Confirm the plan looks good
4. **Implement**: Ask AI to implement the solution
5. **Commit**: Have AI commit and create PR

### 5. Leverage Visual Context
AI performance improves dramatically with images:
- Paste screenshots (macOS: `cmd+ctrl+shift+4` to screenshot to clipboard, `ctrl+v` to paste)
- Drag and drop images directly into prompts
- Provide file paths to design mocks
- Use visual targets for UI development

### 6. Use Extended Thinking for Complex Problems
Trigger deeper analysis by using specific keywords in your prompts:
- Say **"think"** for extended thinking mode (extra computation time)
- **"think hard"** → more thinking budget
- **"think harder"** → even more analysis
- **"ultrathink"** → maximum thinking budget
- Best for architectural decisions, complex refactoring, tricky bugs, or design tradeoffs

**Example**: "Think harder about how to migrate this authentication system from sessions to JWT without breaking existing users."

### 7. Use Subagents for Complex Research and Validation
Delegate specialized tasks to focused AI agents with separate context windows:
- Create research agents for codebase pattern analysis
- Use validation agents to check task completeness before implementation
- Build review agents that critique code with fresh perspective
- Subagents preserve main context and provide specialized expertise

**Example**: Use a preflight agent to validate your feature spec is complete before generating implementation plans.

### 8. Use /clear to Reset Context
During long sessions, context fills with irrelevant information:
- Use `/clear` frequently between tasks
- Keep context focused on current work
- Prevents AI from being distracted by old conversation

### 9. Let AI Handle Git Operations
AI excels at git workflows:
- **Commit messages**: AI analyzes changes and recent history for context-aware messages
- **History searches**: "What changes made it into v1.2.3?", "Why was this API designed this way?"
- **Complex operations**: Reverting files, resolving conflicts, comparing patches

Many developers now use AI for 90%+ of their git interactions.

### 10. Iterate and Experiment Continuously
Prompt engineering is iterative:
- First version might be good, but 2-3 iterations make it great
- Give AI feedback and refine
- Document what works
- Test different approaches
- Adjust phrasing and see what performs better

## What NOT to Do

- ❌ Don't let AI code without planning first (for complex tasks)
- ❌ Don't use vague instructions
- ❌ Don't ignore the context window (clear regularly)
- ❌ Don't trust AI blindly (you're the architect, AI is the team member)
- ❌ Don't use frameworks without understanding what's under the hood
- ❌ Don't add complexity without measuring if it improves outcomes

## Key Mindsets

**Human as Architect, AI as Force Multiplier**
- You set strategic direction and own architecture
- AI handles specialized, scalable tasks
- You make final decisions on all output
- Context quality determines AI performance

**Maintain Control**
- Always review AI-generated code
- Use permission allowlists thoughtfully
- Test extensively in sandboxed environments
- You're the ultimate quality gate

---

*Remember: The goal is not to replace developers, but to empower them. AI handles the tactical execution while you focus on creative problem-solving and architectural vision.*