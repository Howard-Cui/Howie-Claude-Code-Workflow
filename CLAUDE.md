## Overall workflow:

### First step: Transfer my question to a proper prompt

- Before you start work, please transform my requirements into an AI-friendly prompt in XML format
- For different job types, construct your prompt using different structures - please reference the **Prompt Structure** section below
- After you provide me with the prompt in XML format, I will review it and ask you to consume the prompt. Then you will start the plan and review process - for details about this process, see the **Plan & Review** section below
- After you finish the plan and review process, you will move to the implementation phase. While implementing, please ask for my permission before changing code in my codebase and follow the **_While implementing_** section in **Plan & Review**

## Plan & Review

### Before starting work

- Always enter plan mode to create a plan
- If the task involves UI changes or building UI elements, please ask me for an image or screenshot of the UI
- After creating the plan, make sure you write it to .claude/tasks/TASK_NAME.md
- The plan should be a detailed implementation plan with reasoning behind decisions, as well as broken-down tasks
- If the task requires external knowledge or certain packages, research to get the latest information (use Task tool for research)
- Don't over-plan - always think MVP
- Once you write the plan, first ask me to review it. Do not continue until I approve the plan
- I will tell you "plan approved" once I think the plan is acceptable, and you will proceed to the implementation process. Otherwise, I will ask you to make changes to your plan

### While implementing

- You should update the plan as you work
- After you complete tasks in the plan, you should update and append detailed descriptions of the changes you made, so following tasks can be easily handed over to other engineers

## Prompt Structure

### Prompt categories:

- requirement: this section will contain a brief description of my requirements
- procedure_to_reproduce: this section will contain steps to reproduce the issue - this field only exists if the task is related to bug fixing
- context: Business context and logic background - you can generate one for me. If you have no idea what the business context is, just leave this field blank and I will fill in the details myself
- related_files: list all folders and files that are highly related to the tasks and requirements

### Write to an XML file:

- After generating the prompt, please write it to the /prompt.xml file. If this file doesn't exist, create it and write the content
- I will make some changes to this XML file. After I tell you "prompt ready", please read that file to get the prompt and proceed to the next step
