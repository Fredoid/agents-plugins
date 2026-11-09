---
name: global-orchestration-guidelines
description: Explain global agents orchastration strategy and rules to respect all over any realization.
---

When user ask a new request, always respect thoses rules :

- Treat each user's request with this iterative process
- The iterations backlog is stored into the folder /docs/backlog/ : /docs/backlog/backlog.md contains the summary table of all iterations, and each iteration is detailed into its own file /docs/backlog/[N].md (ex : /docs/backlog/1.md).
- When user want to create a new application or when he want explicitely modify or add iterations to the iterations backlog, use firstly the Product Owner agent to analyse and translate user's request to an iterations backlog and write it if not exists (one /docs/backlog/[N].md file per iteration and the summary table into /docs/backlog/backlog.md).
- Iteration backlog should be maintained and up to date to the progression pof realisation.
- To find the next iteration to treat, read only the summary table of /docs/backlog/backlog.md, then read only the /docs/backlog/[N].md file of that iteration. Do not load the whole backlog folder.
- When you start a new iteration and the iteration is already specified in the backlog (/docs/backlog/[N].md) do treat the iteration as a new one and do not split the iteration into sub-iterations, treat the iteration on a single treatment and a unique already specified iteration.
- Treat user's request step by step following iterations defined into the iterations backlog
- Each iteration execution plan must follow the iteration workflow and plan defined by the Project Manager.
- Iteration's status must be updated into the summary table of /docs/backlog/backlog.md and into the iteration file /docs/backlog/[N].md at the start end the end of an iteration.
- Iteration's step's status must be updated into the EXPECTED.md file of the itératio at the start end the end of iteration's steps.
- Project Manager define iteration worflow and verify the iteration successfully followed the expected iteration workflow.
- Other agents must be use to implement realisation of an iteration
- Once an iteration is finished, summup key changes that the user must test manually to validate the iteration delivery. Highlight on added or modified feature dureing the iteration.
