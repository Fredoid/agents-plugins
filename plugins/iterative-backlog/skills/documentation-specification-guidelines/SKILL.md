---
name: documentation-specification-guidelines
description: Explain documentation strategy and rules to respect all over any realization.
---

Lexique :

- **_project folder_** : Current folder of user, referece too the root of the project folder.
- **_documentation files_** : all files containing text explanations, like : spécifications, README, LICENSE, Backlog and all non file writing for human readibility. It could concern media file too, like : image, video, sound, etc...

When create or read file, always respect thoses rules :

- All documentation files must be in markdown format
- All documentation files except README.md and LICENCE.md must be into the folder /docs of the project folder
- The folder /docs should be organized with subfolder. Do not acumulate files into the /docs folder, try to aggragate files into thematical subfolders.
- The specification files must be into the /docs/specs folder of the project folder.
- Do not over produce documentations and specifications, keep documentation concise and clear.
- Do not write too long documentation files. Documentation files must not to be longer than 300 lines. If you need to write large file of specification you should split it into sperated small sub files and organisze them into subfolders. Group files with same topic into subfolders. This rule applies to the iterations backlog too : it is stored into the folder /docs/backlog/, with the summary table of all iterations into /docs/backlog/backlog.md and the detail of each iteration into its own file /docs/backlog/[N].md (ex : /docs/backlog/1.md).

Keep documentation clear and compliant to thoses rules conversational.
