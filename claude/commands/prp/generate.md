# Create PRP

## Feature file: $ARGUMENTS

Generate a complete PRP (Product Requirements & Plans) for general feature implementation with thorough
research. Ensure context is passed to the AI agent to enable self-validation and
iterative refinement. Read the feature file first to understand what needs to be
created, how the examples provided help, and any other considerations.

The AI agent only gets the context you are appending to the PRP and training
data. Assuma the AI agent has access to the codebase and the same knowledge
cutoff as you, so its important that your research findings are included or
referenced in the PRP. The Agent has Websearch capabilities, so pass urls to
documentation and examples.

## Research Process

**Sequential Research Phase** (Codebase first, then smart external research)

1. **Codebase Analysis** (Use subagent: `prp-codebase-research`)
    - Search for similar features/patterns in the codebase
    - Identify files to reference in PRP
    - Note existing conventions to follow
    - Check test patterns for validation approach
    - **CRITICAL**: Document what components/libraries/patterns already exist
    - **ASSESS**: Determine knowledge gaps that truly need external research

2. **Smart External Research Decision** (Evaluate AFTER codebase analysis)
   
   **FIRST: Analyze codebase findings to determine if external research is needed:**
   
   **SKIP External Research if:**
   - ✅ Similar components/patterns found in codebase (internal project components)
   - ✅ Clear implementation path from existing code
   - ✅ Standard CRUD/UI operations using existing patterns
   - ✅ Internal utility functions/services already available
   
   **PROCEED with External Research ONLY if:**
   - ❌ New external npm/library integration needed (get current docs)
   - ❌ Existing external library usage but complex/undocumented features needed
   - ❌ Complex algorithm or pattern not in codebase
   - ❌ Security/performance considerations beyond current code
   - ❌ External API integration without existing examples
   - ❌ **No similar patterns/components found in codebase** (need external examples)
   
   **If External Research is needed** (Use subagent: `prp-research-agent`):
   - Focus ONLY on missing knowledge gaps identified above
   - External npm/library documentation for NEW packages or complex features
   - Best practices for COMPLEX patterns not in codebase
   - Security considerations for NEW external integrations
   - **AVOID**: Researching internal project components (use codebase instead)

3. **User Clarification** (Use if needed after research completion)
    - Specific patterns to mirror and where to find them?
    - Integration requirements and where to find them?
    - Which existing service to use and its file path?
    - **NEW**: Confirm if external research is truly needed for identified gaps

## PRP Generation

Using PRPs/templates/prp_document_template.md as template:

### Critical Context to Include and pass to the AI agent as part of the PRP

- **Code Examples**: Real snippets from codebase (PRIMARY FOCUS)
- **Patterns**: Existing approaches to follow (MIRROR THESE)
- **Documentation**: URLs ONLY for new/missing knowledge gaps
- **Gotchas**: Library quirks, version issues from codebase analysis
- **Research Justification**: Explain why external research was/wasn't needed

### Implementation Blueprint

- Start with pseudocode showing approach
- Reference real files for patterns
- Include error handling strategy
- list tasks to be completed to fullfill the PRP in the order they should be
  completed

### Validation Gates (Must be Executable)

**During Codebase Research Phase**, identify and document available project
validation tools:

- Analyze project configuration files for validation commands (package.json,
  Makefile, pyproject.toml, setup.py, Cargo.toml, go.mod, etc.)
- Identify linting, testing, and formatting tools specific to the project's tech
  stack
- Document exact validation commands found in the project
- Include these validation commands directly in the PRP document
- Ensure all code changes will pass project validation standards
- Add specific validation steps to PRP task list with exact commands to run

**CRITICAL AFTER YOU ARE DONE RESEARCHING AND EXPLORING THE CODEBASE BEFORE YOU
START WRITING THE PRP**

**ULTRATHINK ABOUT THE PRP AND PLAN YOUR APPROACH THEN START WRITING THE PRP**

## Output

Save as: `PRPs/{feature-name}.md`

## Quality Checklist

- [ ] All necessary context included
- [ ] Validation gates are executable by AI
- [ ] References existing patterns
- [ ] Clear implementation path
- [ ] Error handling documented

Score the PRP on a scale of 1-10 (confidence level to succeed in one-pass
implementation using claude codes)

Remember: The goal is one-pass implementation success through comprehensive
context.
