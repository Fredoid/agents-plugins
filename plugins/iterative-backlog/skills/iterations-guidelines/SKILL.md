---
name: iterations-guidelines
description: Explain iterations strategy, process and rules to respect all over any realization. Iteration is the main conception workflow of any conception and modification of the project.
---

Lexique :

- **_project folder_** : Current folder of user, referece too the root of the project folder.
- **_documentation files_** : all files containing text explanations, like : spécifications, README, LICENSE, Backlog and all non file writing for human readibility. It could concern media file too, like : image, video, sound, etc...
- **_iteration folder_** : subfolder of an iteration.

When you read or create or modify application, always respect thoses rules :

- Any user request of creation or modification of application must be splited into smaller iterations and must be realized iteration by iteration.
- Each iteration must have its own subfolder into the folder /docs/iterations/ of project folder to store all documentation files related to the iteration.
- Any iteration must be documented and its extpected must be clearly specified into the file EXPECTED.md file into its iteration subfolder, ex : /docs/iterations/1.
- Every iterations steps and their status must be specified and maintained up to date into the EXPECTED.md file. Three possible statuses: A faire, En cours, et Terminé. When an iteration is created, by default all its steps are in the "A faire" status.
- When you start a step you must always first update the status of the step to "En cours" in the EXPECTED.md file.
- When you finish a step you must always last update the status of the step to "Finished" in the EXPECTED.md file.
- Any iteration delivery must be documented and and clearly explaned into the file DELIVERY.md file into its iteration subfolder.
- Iterations' subfolders must only contain those two file EXPECTED.md and DELIVERY.md. Any other form of documentation or specification file must be written in the folder /docs/specs of the project folder.
- The iterations backlog is stored into the folder /docs/backlog/ of project folder. It is always organized this way :
  -- **_/docs/backlog/backlog.md_** : the backlog index. It only contains a summary table of all iterations of the backlog with those columns : iteration number, iteration title, iteration status, link to the iteration backlog file (ex : [1.md](1.md)). It must never contain the detail of the iterations.
  -- **_/docs/backlog/[N].md_** : one file per iteration, named with the iteration number (ex : /docs/backlog/1.md, /docs/backlog/2.md, /docs/backlog/3.md, etc...). It contains the full detail of the iteration : title, status, user objective, value, functional scope, acceptance criteria, dependencies and expected final state.
- Every iteration of the backlog must have its own file /docs/backlog/[N].md and its own line into the summary table of /docs/backlog/backlog.md. Both must always be up to date of the user requests and progressions of iterations.
- When you add, remove, rename or renumber an iteration, always update both the iteration file /docs/backlog/[N].md and the summary table of /docs/backlog/backlog.md.
- To know the iterations backlog, always read first only /docs/backlog/backlog.md. Then read only the /docs/backlog/[N].md files of the iterations you need (usually the current iteration and, if needed, its dependencies). Never read all iteration files of the backlog when it is not necessary.
- The iteration statuses must always be up-to-date in the /docs/backlog/backlog.md summary table, the iteration file /docs/backlog/[N].md and the EXPECTED.md file.
- Always update the statuses of the iteration steps at the beginning and end of each step into the EXPECTED.md file.
- Always update the status of an iteration at the beginning and end of the iteration into the /docs/backlog/backlog.md summary table, the iteration file /docs/backlog/[N].md and the EXPECTED.md file.
- Iterations backlog (/docs/backlog/backlog.md and all /docs/backlog/[N].md files) must always be written and maintain by the product owner agent.
- The first thing to do when starting an iteration is to update its status "En cours" into the /docs/backlog/backlog.md summary table and into its /docs/backlog/[N].md file.
- The last thing to do when finishing an iteration is to update its status "Terminé" into the /docs/backlog/backlog.md summary table and into its /docs/backlog/[N].md file.
- The steps of an iteration must always follow each other automatically; user permission should not be required to move from one step to another within the same iteration.
- Iteration's status must always maintained up to date into the /docs/backlog/backlog.md summary table and the /docs/backlog/[N].md iteration file. Possible statuses are : A faire, En cours et Terminé.
- If a legacy file /docs/ITERATIONS_BACKLOG.md exists in the project folder, migrate it : split each iteration into its own /docs/backlog/[N].md file, build the summary table into /docs/backlog/backlog.md, then delete /docs/ITERATIONS_BACKLOG.md.
- At the end of an iteration, always ask the user to manually test the application and ask if they want to move on to the next iteration, if there is an error to correct, or if they have anything else to ask.
- Never use or insert checkoxes into the list acceptance criteria
- Into the EXPECTED.md file of an iteration you must always describe iteration's steps statuses following thoses two rules :
  -- Always maintain a summary table of the iterations statuts with thoses columns : step id, step name, step status
  -- Always maintain a the steps list containing : name, status and key actions list. Always follow thoses exemples to describe an iteration step :
  **_ Debut des exemples _**
  Preparation des agents IA
  Statut : Terminé
  Actions :
  - [x] lire les agents existants
  - [x] Déterminer les changements nécessaires
  - [x] Appliquer les changements
  - [x] Sauvegarder et demander le redémarrage

  Spécification produit
  Statut : En cours
  Actions :
  - [x] comprendre le besoin utilisateur
  - [ ] rédiger le document de spécification
  - [ ] documenter les critères d'acceptance

  Spécification design
  Statut : En cours
  Actions :
  - [ ] Définir la charte graphique
  - [ ] Spécifier la mise en page
  - [ ] Définir le typographie et les couleurs
        **_ Fin des exemples _**

The aim of this workflow is to guarantee to the user that the deliverable of the iteration is fully functional and usable.

- **Each iteration must follow this worfkow of steps :**

-- **_Update iteration status and expected_** : Check and update iteration status into the /docs/backlog/backlog.md summary table and into the iteration file /docs/backlog/[N].md. Create the EXPECTED.md file into the iteration's folder if not exists. Check and update iteration's steps status into the EXPECTED.md.
-- \*\*\_IA Agentic preparation**\* : create or modify necessaries project's claude agents manage project agent builders and maintain their knowledge, expertise and memory of the project. Always use claude agent and create à network of expert agents of the project. After any agent modification user must relaod claude to continue with new claude agents configuration. Before the user restarts, Claude always saves the state of the current iteration to more easily resume the current iteration after Claude restarts.
-- **_Product specification_** : create or modify product specificatison files to integrate the iteration product specifications changes.
-- **_Design specification_** : create of modify design specifications files to integrate the iteration design specifications changes.
-- **_Technical architecture specification_** : create of modify technical architecture specifications files to integrate the iteration architectural specifications changes.
-- **_Coding_** : adapt code base and project files to implement all code changes.
-- **_Debug_** : build and launch all the services of the applications to correct building and configuration errors until the application is successfully up and running. From this point onwards, always leave the application running and all its services running for the following steps of the iteration.
-- **_Testing_\*\* : create or modify automated tests files to integrate new specificatison changes and then run tests and correct application until every tests successfully pass. A non regression test report of the iteration must always been documented and written in the iteration folder. Run and execute only the necessary groups of tests as per the testing strategy and modified functionals and technical aspects.

**_Use appropriates agents to execute and implement each iteration workflow steps_**

Keep iteration specifications and expected clear and compliant to those rules conversational.
