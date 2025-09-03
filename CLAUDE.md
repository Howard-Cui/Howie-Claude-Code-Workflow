## Overall workflow:

### First step: transfer my question to a proper prompt

- Before you start work, please transfer my requirement to a AI friendly prompt in XML format
- For different job types, you will construct your prompt into different structures, please reference to the **Prompt Structure** section below.
- After you giving me the prompt in XML format, I will jusitfy it and let you to consume the prompt, you will start on plan and review process, for details about plan and review process, I will explain in **Plan & Review** section below, please follow it.
- After you finished plan and review process, you will jump to implementing process, while you are implementing, please ask my permission to change code in my code bases and also follow the **_While implmenting_** part in **Plan & Review** Section.

## Plan & Review

### Before starting work

- Always in plan mode to make a plan
- If the task is about UI changes or building UI elements, please ask me for a image or screenshot of UI
- After get the plan, make sure you write the plan to .claude/tasks/TASK_NAME.md
- The plan should be a detailed implementation plan and the reasoning behind them, as well as taks broken down.
- If the task require external knowledge or certian package, also research to get latest knowledge (Use Task tool for research)
- Don't over plan it, always think MVP.
- Once you write the plan, firstly ask me to review it. Do not continue until I approve the plan.
- I will tell you "plan approved" once I think the plan is ok, and you will go to the implementation process, otherwise I will keep ask you to do some changes on your plan.

### While implmenting

- You should update the plan as you work.
- After you complete tasks in the plan, you should update and append detailed descriptions of the changes you made, so following tasks can be easily hand over to other engineers.

## Prompt Structure

### Prompt categories:

- requirement: this section will contain the brief of my requirement.
- procedure_to_reproduce: this section will contain steps that reproduce the issues, so this field will only exist if this task is related to bug fixing.
- context: Business context and logic background, you can generate one for me, if you have no idea what the business context is, just leave this field blank, I will fill in the details myself.
- related_files: list all the folders and files that highly related with the tasks and requirements.

### Write into a XML file:

- After prompt generated, please write it into /prompt.xml file, if this file is not existing, create one and write it into it.
- I will make some change on this xml file, after I tell you "prompt ready", please go to read that file to get the prompt and go to next step.
