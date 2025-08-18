name: "Universal PRP Template v1.1.0 - Framework-Agnostic Implementation Guide"
description: |

## Purpose

Universal template optimized for AI agents to implement features across any tech
stack with sufficient context and self-validation capabilities to achieve
working code through iterative refinement.

## Core Principles

1. **Context is King**: Include ALL necessary documentation, examples, and
   caveats
2. **Validation Loops**: Provide executable tests/lints the AI can run and fix
3. **Information Dense**: Use keywords and patterns from the codebase
4. **Progressive Success**: Start simple, validate, then enhance
5. **Framework Agnostic**: Adaptable to any language, framework, or architecture
6. **Global rules**: Be sure to follow all rules in CLAUDE.md

---

## Discovery Summary

### Initial Task Analysis

[Brief summary of user's original request and initial assessment]

### User Clarifications Received

[Document any questions asked during Phase 1 and user responses]

- **Question**: [What was unclear about the business logic?]
- **Answer**: [User's clarification]
- **Impact**: [How this affects implementation approach]

### Missing Requirements Identified

[List any requirements that were initially missing but discovered during Phase
1]

## Goal

[What needs to be built - be specific about the end state and desires]

## Why

- [Business value and user impact]
- [Integration with existing features]
- [Problems this solves and for whom]

## What

[User-visible behavior and technical requirements]

### Success Criteria

- [ ] [Specific measurable outcomes]

## All Needed Context

### Research Phase Summary

[Summary of Phase 1 discovery findings and Phase 2 research decisions]

- **Codebase patterns found**: [Similar components/patterns identified]
- **External research needed**: [Yes/No with justification]
- **Knowledge gaps identified**: [What wasn't available in codebase]

### Documentation & References (list all context needed to implement the feature)

```yaml
# MUST READ - Include these in your context window
- url: [Official API docs URL]
  why: [Specific sections/methods you'll need]

- file: [path/to/example.py]
  why: [Pattern to follow, gotchas to avoid]

- doc: [Library documentation URL]
  section: [Specific section about common pitfalls]
  critical: [Key insight that prevents common errors]

- docfile: [PRPs/ai_docs/file.md]
  why: [docs that the user has pasted in to the project]
```

### Current Codebase tree (run `tree` in the root of the project) to get an overview of the codebase

```bash

```

### Desired Codebase tree with files to be added and responsibility of file

```bash

```

### Known Gotchas of our codebase & Library Quirks

```[LANGUAGE]
# CRITICAL: [Library name] requires [specific setup]
# Example: React requires useEffect for side effects
# Example: FastAPI requires async functions for endpoints
# Example: This ORM doesn't support batch inserts over 1000 records
# Example: Next.js App Router uses server components by default
# Example: Express.js middleware order matters
# Example: Vue 3 Composition API vs Options API patterns
```

## Implementation Blueprint

### Data models and structure

Create the core data models/types/interfaces to ensure type safety and
consistency.

```[LANGUAGE]
# Backend Examples:
 - Database models (ORM/ODM)
 - API schemas/DTOs
 - Validation schemas
 - Domain entities

# Frontend Examples:
 - TypeScript interfaces/types
 - Component props types
 - API response types
 - Store/state types
 - Form validation schemas
```

### list of tasks to be completed to fullfill the PRP in the order they should be completed

```yaml
Task 1:
MODIFY [path/to/existing_file]:
   - FIND pattern: "[existing_pattern_to_locate]"
   - INJECT after line containing "[specific_line_marker]"
   - PRESERVE existing [method_signatures/props/interfaces]

CREATE [path/to/new_file]:
   - MIRROR pattern from: [path/to/similar_file]
   - MODIFY [class/component/function] name and core logic
   - KEEP [error_handling/styling/structure] pattern identical

INSTALL dependencies (if needed):
   - ADD: [package_name@version] to [package.json/requirements.txt/Cargo.toml]
   - CONFIGURE: [specific_setup_needed]

UPDATE configuration:
   - MODIFY: [config_file_path]
   - ADD: [new_config_options]

   ...(...)

Task N:
...

```

### Per task pseudocode as needed added to each task

```[LANGUAGE]
# Task 1 - [Backend API Example]
# Pseudocode with CRITICAL details - don't write entire code
function/method new_feature(param: InputType) -> OutputType {
    // PATTERN: Always validate input first (see [validation_file_path])
    validated = validateInput(param);  // throws ValidationError

    // GOTCHA: This library requires [specific_setup]
    try {
        // PATTERN: Use existing [pattern_name] (see [reference_file])
        result = await [service/api].call(validated);

        // CRITICAL: [Important constraint/rate limit/etc]
        // PATTERN: Standardized response format
        return formatResponse(result);  // see [response_utils_path]
    } catch (error) {
        // PATTERN: Error handling (see [error_handler_path])
        return handleError(error);
    }
}

# Task 1 - [Frontend Component Example]
# Component structure with CRITICAL details
function NewFeatureComponent({ props }: Props) {
    // PATTERN: State management (see [existing_component_path])
    const [state, setState] = useState(initialState);

    // PATTERN: Side effects (see [hooks_path])
    useEffect(() => {
        // GOTCHA: [Cleanup/dependency specific detail]
        // CRITICAL: [Performance/render constraint]
    }, [dependencies]);

    // PATTERN: Event handlers (see [handlers_path])
    const handleAction = useCallback(() => {
        // PATTERN: Error boundaries (see [error_boundary_path])
    }, [dependencies]);

    return (
        // PATTERN: Component structure (see [similar_component])
        // CRITICAL: Accessibility/styling constraints
    );
}
```

### Integration Points

```yaml
# Backend Integration Points
DATABASE (if applicable):
  - migration: '[SQL/NoSQL migration details]'
  - index: '[Index creation for performance]'
  - schema: '[Schema changes needed]'

API/ROUTES:
  - add to: [routes_file_path]
  - pattern: '[route_registration_pattern]'
  - middleware: '[auth/validation middleware needed]'

CONFIG:
  - add to: [config_file_path]
  - pattern: '[environment_variable_pattern]'
  - secrets: '[secret/key management]'

# Frontend Integration Points
ROUTING:
  - add to: [router_config_path]
  - pattern: '[route_definition_pattern]'
  - guards: '[auth/permission guards needed]'

STATE_MANAGEMENT:
  - add to: [store/context_path]
  - pattern: '[state_update_pattern]'
  - actions: '[action_creators/mutations needed]'

STYLES:
  - add to: [styles_path]
  - pattern: '[css/styling_pattern]'
  - theme: '[theme_integration_needed]'

COMPONENTS:
  - register in: [component_registry_path]
  - export from: [index_file_path]
  - props: '[prop_interface_definitions]'
```

## Validation Loop

### Level 1: Syntax & Style

```bash
# Run these FIRST - fix any errors before proceeding
# [PROJECT_SPECIFIC_COMMANDS] - Examples:
# JavaScript/TypeScript: npm run lint, npm run type-check
# Python: ruff check [files] --fix, mypy [files]
# Go: go fmt, go vet, golangci-lint run
# Rust: cargo fmt, cargo clippy
# PHP: composer run phpcs, composer run phpstan
# Java: mvn checkstyle:check, mvn spotbugs:check

[linter_command] [file_paths]        # Syntax and style checking
[type_checker_command] [file_paths]  # Type checking (if applicable)

# Expected: No errors. If errors, READ the error and fix.
```

## Final validation Checklist

- [ ] All tests pass: `[project_test_command]`
- [ ] No linting errors: `[project_lint_command]`
- [ ] No type errors: `[project_type_check_command]` (if applicable)
- [ ] Build succeeds: `[project_build_command]` (if applicable)
- [ ] Manual test successful: [specific_test_command_or_url]
- [ ] Error cases handled gracefully
- [ ] Logs are informative but not verbose
- [ ] Documentation updated if needed
- [ ] Dependencies properly declared in [package_file]

---

## Anti-Patterns to Avoid

- ❌ Don't create new patterns when existing ones work
- ❌ Don't skip validation because "it should work"
- ❌ Don't ignore failing tests - fix them
- ❌ Don't mix paradigms (sync/async, class/functional) inconsistently
- ❌ Don't hardcode values that should be config/environment variables
- ❌ Don't catch all exceptions - be specific about error handling
- ❌ Don't ignore accessibility requirements (for frontend)
- ❌ Don't skip security considerations (input validation, auth)
- ❌ Don't forget to handle loading and error states (for frontend)
- ❌ Don't ignore performance implications (N+1 queries, large bundles)
