name: "Technical Task Template v1.0.0 - AI-Optimized Development Task Specification"
description: |

# Technical Task Template

> **Purpose**: Comprehensive template for AI-optimized technical task descriptions that provide maximum context for development teams and AI coding assistants.

## Task Identification

**Task ID**: [T-{number}] (e.g., T-001)  
**Task Name**: [Clear, action-oriented name using verb-noun structure]  
**Priority**: [Critical/High/Medium/Low]  

## Context & Background

### Source PRP Document
**Reference**: [docs/prps/{feature-name}.md] - [Link to the PRP document this task was created from]

### Feature Overview
Brief description of the larger feature this task belongs to and its business value.

### Task Purpose
**As a** [role/system]  
**I need** [specific capability]  
**So that** [business outcome/user benefit]  

### Dependencies
- **Prerequisite Tasks**: [List of task IDs that must be completed first]
- **Parallel Tasks**: [Tasks that can be worked on simultaneously]
- **Integration Points**: [External systems/components this task interacts with]
- **Blocked By**: [Any current blockers preventing work]

## Technical Requirements

### Functional Requirements
Using EARS format when applicable:
- **REQ-1**: When [trigger event], the system shall [required response]
- **REQ-2**: While [condition], the system shall [behavior]
- **REQ-3**: Where [location/context], the system shall [action]

### Non-Functional Requirements
- **Performance**: [Response time, throughput, scalability requirements]
- **Security**: [Authentication, authorization, data protection needs]
- **Accessibility**: [A11y standards, WCAG compliance]
- **Compatibility**: [Browser support, device compatibility]

### Technical Constraints
- **Technology Stack**: [Required frameworks, libraries, languages]
- **Architecture Patterns**: [Design patterns to follow]
- **Code Standards**: [Coding conventions, style guides]
- **Database**: [Schema changes, migrations needed]

## Implementation Details

### Files to Modify/Create
```
├── [path/to/file1.ext] - [Purpose: what changes needed]
├── [path/to/file2.ext] - [Purpose: what changes needed]
└── [path/to/new-file.ext] - [Purpose: what this file will do]
```

### Key Implementation Steps
1. **Step 1**: [Action needed] → [Expected outcome]
2. **Step 2**: [Action needed] → [Expected outcome]
3. **Step 3**: [Action needed] → [Expected outcome]

### Code Patterns to Follow
Reference existing implementations:
- **Similar Pattern**: [file_path:line_number] - [What pattern to mirror]
- **Error Handling**: [file_path:line_number] - [Error handling approach to use]
- **Validation**: [file_path:line_number] - [Validation pattern to follow]

### API Specifications (if applicable)
```yaml
# Endpoint details
Method: [GET/POST/PUT/DELETE]
Path: [/api/path/to/resource]
Headers: [Required headers]
Request Body:
  - field: [type] - [description]
Response:
  - status: [200/201/400/etc]
  - body: [response structure]
```

## Acceptance Criteria

### Given-When-Then Scenarios
```gherkin
Scenario 1: [Primary happy path]
  Given [initial context/state]
  When [action is performed]
  Then [expected outcome]
  And [additional verification]

Scenario 2: [Error handling]
  Given [error condition setup]
  When [triggering action]
  Then [error response expected]

Scenario 3: [Edge case]
  Given [edge case context]
  When [action performed]
  Then [expected behavior]
```

### Rule-Based Criteria (Checklist)
- [ ] **Functional**: [Core functionality works as specified]
- [ ] **UI/UX**: [Interface matches designs/wireframes]
- [ ] **Performance**: [Meets performance requirements]
- [ ] **Security**: [Security requirements satisfied]
- [ ] **Error Handling**: [Error cases handled gracefully]
- [ ] **Integration**: [Integrates properly with existing systems]
- [ ] **Mobile**: [Works on mobile devices if applicable]
- [ ] **Accessibility**: [Meets accessibility standards]

## Manual Testing Steps
1. **Setup**: [How to prepare test environment]
2. **Test Case 1**: [Step-by-step testing instructions]
3. **Test Case 2**: [Additional scenarios to verify]
4. **Cleanup**: [How to clean up after testing]

## Validation & Quality Gates

### Code Quality Checks
```bash
# Project-specific commands - customize based on your tech stack
[Add your project's validation commands here]
```

### Definition of Done
- [ ] [Customize based on your team's standards and project requirements]

## Resources & References

### Documentation Links
- **Primary Docs**: [URL] - [Specific sections needed]
- **API Reference**: [URL] - [Relevant endpoints/methods]
- **Design System**: [URL] - [UI components to use]

### Code References
- **Similar Implementation**: [file_path:line_number] - [What to reference]
- **Pattern Examples**: [file_path:line_number] - [Implementation pattern]
- **Error Handling**: [file_path:line_number] - [Error handling approach]

### External Resources
- **Stack Overflow**: [URL] - [Specific solution reference]
- **GitHub Examples**: [URL] - [Relevant code examples]
- **Technical Articles**: [URL] - [Implementation guidance]

## Notes & Comments

### Additional Context
[Any additional information that doesn't fit other sections but is important for implementation]

### Questions for Clarification
- [ ] **Question 1**: [Specific question needing answer]
- [ ] **Question 2**: [Another clarification needed]

### Implementation Notes
[Developer notes, gotchas, or special considerations during implementation]

---

**Template Version**: 1.0  
**Last Updated**: [Date]