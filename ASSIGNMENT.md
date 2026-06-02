# Assignment "Agent instructions"
## Instructions
1. Prompt in Agent mode in the plugin to create an AGENTS.md and generate instructions.
2. General instructions are generated in AGENTS.md, discuss the generated content and change to your taste. 
3. Make sure to have the following sections in your AGENTS.md:
   - Commands
     - In this project are 2 projects which separately need specific build commands. Tell them which folder needs which command to run the application.
   - Guardrails
     - Define guardrails for the agents to follow. For example, if you want to limit the number of API calls, or if you want to restrict certain actions, you can define those guardrails here. Also compliancy rules can be set here.
   - System Overview
     - Provide a high-level overview of the system, including its purpose, main components, and how they interact with each other. This section should give agents a clear understanding of the system's architecture and functionality.
   - System Architecture
     - Provide a detailed description of the system's architecture, including the technologies used, the structure of the codebase, and any relevant design patterns. This section should help agents understand how the system is built and how different components work together.
   - Development Guidelines
     - Provide guidelines for development, including coding standards, best practices, and any specific tools or libraries that should be used. This section should help agents maintain consistency and quality in their code.
   - Testing Guidelines
     - Provide guidelines for testing, including the types of tests that should be written (unit tests, integration tests, etc.), the testing framework to be used, and any specific testing strategies or practices that should be followed. This section should help agents ensure that their code is well-tested and reliable.
   - Security & Authentication
     - Provide guidelines for security and authentication, including any specific security measures that should be implemented, how authentication should be handled, and any relevant best practices for securing the application. This section should help agents ensure that the application is secure and that user data is protected.

# Assigment "Create a SKILLS.md"
## Instructions
1. Create a skills folder in the .github folder.
2. Create a specify-feature folder in the skills folder.
3. Create a SKILLS.md file in the specify-feature folder.
4. In the SKILLS.md file, define the skills that are required to specify a feature:
```
--- 

name: specify-feature 

description: Generates a comprehensive functional description of a feature 

--- 

 

## Instructions 

1. Generate a kebab-case name for the feature (e.g. view-profile) 

2. Create a spec folder with that name under `.github/specs/` if it does not exist already. 

3. Copy the spec template from `.github/templates/spec.template.md` into the new spec folder. 

4. Read the template. If parts are not clear in the feature specification from the user and for other questions to make the feature clear, use the #askQuestions tool (max 20 times) for every unclear part. 

5. Fill in the template for this feature and save it to a file named `spec.md` in the spec folder. Write everything in brief sentences, only keeping the essential phrasing to be descriptive and unambiguous. 

6. Use #runSubagent tool to spawn a subagent (standard agent type). Ask the subagent to check the generated spec.md against the template. It should detect things that are missing and things that are undesired like technical details. 
```
5. Create a template folder in the .github folder.
6. Create a spec.template.md file in the template folder.
7. In the spec.template.md file, define a template for the feature specification assisted with an Agent.
8. Tweak the template file with an agent until you're satisfied.