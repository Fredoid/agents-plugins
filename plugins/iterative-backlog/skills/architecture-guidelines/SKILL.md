---
name: architecture-guidelines
description: Explain architecture strategy and rules to respect all over any realization.
---

Lexique :

- **_project folder_** : Current folder of user, referece too the root of the project folder.
- **_documentation files_** : all files containing text explanations, like : spécifications, README, LICENSE, Backlog and all non file writing for human readibility. It could concern media file too, like : image, video, sound, etc...

When create or read file or do any kind of software and IT engineering task, always respect thoses rules :

- All application or any deliverable must always be built over an docker compose v2 architecture. Always use docker compose v2 command to start, stop and manage application.
- All services of the application must always run into Docker container and must be included into the docker compose file.
- All web frontend applications must always be implemented with TypeScript and ReactJS
- All api services must always be implemented with TypeScript
- All mobile applications must always be implemented with Flutter
- All sql database services must always use PostgreSql
- All tasks of scraping, synchronizing, importing or any other importing and transforming data must always be run on backend services. It is strictly forbiden to implement this kind of task into any other kind of service.
- Only api services can communicate with database servicea web and mobile application must never communicate with database directly.
- All frontend or mobile application and backend services must always consume api services to access and manipulate data store in database.
- All docker compose service must always be stored into sperated subfolders of folder /service of the project folder
- Architecture specifications must always be documented and up to date into the folder /docs/architecture of project folder.

Keep project architecture clear and compliant to thoses rules conversational.
