---
name: claude-agents-guidelines
description: Explain claude agents strategy, usage and and rules to always respect all over any realization and manipulation.
---

When you want to manage, create or modify claude code agents, always respect thoses rules :

- Always use project's claude agents to treat any user request.
- Create, modify, maintain and use project's claude agents
- Always load all skills and guidelines before create or modify claude agent.
- The only allowed agent to manipulate and maintain claude agents file is the default-claude-agents-guardian.
- Do not modifiy default agents prefixed by "default-" and stored into the folder ./claude/agents/default. Your are not allowed to alter those agents, only a humain and a manual action is allowed to modify thoses agents.
- You can only create and modify project's agents stored into the folder ./claude/agents/project.
- Do not modifiy skills stored into the folder ./claude/skills. Your are not allowed to alter those files, only a humain and a manual action is allowed to modify thoses agents.
- Project's agents name must always be prefixed by "project-".
- Each agent file must be small and consice and contain pertinent information regarding to the project.
  No other agent is authorized to modify the project's agent files.
- After agents have been modified or created, you must always stop and ask the user to restart Claude. You will resume work after he has restarted.
- It is forbidden to disregard the advice of the default-claude-agents-guardian agent regarding the creation or modification of agents, even if it hinders project progress or an iteration. Improving the agent network is always preferable.
- You always must ask restarting claude after any agent creation or modification for changes to the agents to take effect.
- If a restart is necessary, you must always mention it in the EXPECTED.md tracking file for the iteration. Mention scrictly : "REDEMARRAGE de Claude requis".
- Always alert user to the necessity of hot reloading claude agents after claude agents' files modification.
- Created agents must always have thoses skills :
  -- claude-agents-guidelines
  -- architecture-guidelines
  -- backend-guidelines
  -- documentation-guidelines
  -- folder-structure-guidelines
  -- global-orchestration-guidelines
  -- iterations-guidelines
  -- testing-guildelines
  -- ux-ui-design-guidelines
  -- activity-monitoring
- Update and improve agents to store and expertise agents withs project's informations likes :
  -- Product and fonctional key points
  -- technical key points
  -- testing key points
  -- databse technical and usage key poonts
  -- Technologies
  -- Project organization
  -- ...any other pertinent informations to help agents to do better work

Few exemples of claude agents :

- **_reactjs-developer_** : developer specialist web reactjs
- **_reactjs-typescript-developer_** : developer TypeScript specialist web reactjs
- **_flutter-developer_** : mobile flutter developer
- **_qa-test-flutter-maestro_** : expert end to end tests with flutter and maestro
- **_ux-ui-director_** : Art director, specialist design and look and feel
- **_postgres-sql-databse_** : Postgres database administrator, expet SQL with postgres
- **_functional-specification-writer_** : Expert in functional and product specification, convert iteration expected into functionals specifications of the iteration
- **_technical-specification-writer_** : Expert in functional and product specification, convert iteration expected, ux-ui and functionals sepcificationinto into technicals specifications of the iteration
- **_docker-compose-specialist_** : Docker compose specialist, expert in docker architecture and docker conpose

Keep project's claude agents clear and compliant to thoses rules.
