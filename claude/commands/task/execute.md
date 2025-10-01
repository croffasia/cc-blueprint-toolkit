---
description: Execute individual development tasks from task breakdown documents
argument-hint: [path/to/task-file.md or docs/tasks/{feature-name}.md]
allowed-tools: TodoWrite, Read, Write, Edit, MultiEdit, Glob, Grep, Bash, NotebookEdit
---

# Execute Development Task

Implement a specific development task using the detailed task specification.

## Task File: $ARGUMENTS

## Execution Process

1. **Load Task Document**
    - Read the specified task breakdown file from `docs/tasks/` 
    - Understand task context, requirements, and acceptance criteria
    - Review all referenced files and code patterns
    - Load the comprehensive task template structure
    - Identify specific task within document if multiple tasks present

2. **Task Analysis**
    - Extract the specific task requirements and constraints
    - Review Given-When-Then acceptance criteria scenarios
    - Study referenced code patterns and file locations
    - Understand integration points and dependencies

3. **Implementation Planning**
    - Use TodoWrite tool to create focused implementation plan
    - Break down the single task into micro-steps if needed
    - **CRITICAL**: Study all referenced files specified in task description
    - **PATTERN MATCHING**: Identify exact patterns to mirror from existing code
    - Plan implementation approach following established conventions

4. **Focused Implementation**
    - **BEFORE coding**: Read reference files to understand exact structure
    - **MIRROR PATTERNS**: Follow existing code patterns exactly
    - Implement only the specific task requirements (no scope creep)
    - Apply error handling patterns from reference implementations
    - Follow code organization and naming conventions from examples

5. **Acceptance Criteria Validation**
    - Execute each Given-When-Then scenario manually
    - Verify rule-based criteria checklist completion
    - Execute validation commands specified in task

6. **Quality Gates**
    - Run project-specific validation commands
    - Fix any linting, type-checking, or build errors
    - Ensure task-specific Definition of Done criteria met
    - Verify integration with existing systems

7. **Task Completion**
    - Mark task as completed in TodoWrite
    - Verify all acceptance criteria satisfied
    - Document any implementation notes or gotchas discovered
    - Report completion status with validation results

## Task Execution Best Practices

- Stay strictly within task boundaries - no additional features
- Reference existing patterns extensively before writing new code
- Test incrementally as you build each component
- Follow the exact file structure specified in task document
- Verify dependencies are satisfied before starting

Note: For complex tasks with multiple dependencies, ensure prerequisite tasks are completed first or coordinate with team members.