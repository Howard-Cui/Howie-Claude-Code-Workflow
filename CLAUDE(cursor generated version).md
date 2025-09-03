## Development Workflow Protocol

<workflow_instructions>
**Step 1: Requirement Analysis & Prompt Generation**

- Transform user requirements into structured XML prompts using the format below
- Create prompts in `/prompt.xml` for user review before proceeding
- Wait for "prompt ready" confirmation before starting work

**Step 2: Planning Phase**

- Always enter plan mode before implementation
- For UI changes, request screenshots or mockups from user
- Create detailed implementation plans with reasoning and broken-down tasks
- Write plans to `.claude/tasks/TASK_NAME.md`
- Think MVP - avoid over-planning
- Research external dependencies and latest package information when needed
- Request plan approval before proceeding (wait for "plan approved")

**Step 3: Implementation Phase**

- Ask permission before making code changes
- Update plans with detailed change descriptions as you work
- Maintain handover documentation for future engineers
  </workflow_instructions>

<prompt_structure>
**XML Prompt Template:**

```xml
<requirement>
[Brief, specific description of what needs to be implemented or fixed]
</requirement>

<procedure_to_reproduce>
[Detailed steps to reproduce the issue - only include for bug fixes]
</procedure_to_reproduce>

<context>
[Business context, user impact, and technical background]
</context>

<related_files>
[Specific folders and files that will be modified or are relevant to the task]
</related_files>
```

**Prompt Best Practices:**

- Be explicit about expected outcomes and success criteria
- Include specific examples when describing desired behavior
- Mention any constraints or limitations upfront
- Specify which authentication layer the feature should use
- Include any performance or security considerations
  </prompt_structure>

<communication_guidelines>
**Interaction Protocol:**

- Always ask for clarification when requirements are ambiguous
- Provide progress updates during long implementation tasks
- Explain technical decisions and trade-offs clearly
- Request screenshots/mockups for UI-related changes
- Confirm understanding before making significant architectural changes
- Use consistent terminology matching the codebase
  </communication_guidelines>
