# Repository structure

This repository contains a Power BI Project (PBIP) for the `sales` report.

- `apm.yml` defines the agent package, Fabric skills, and MCP dependencies.
- `sales.pbip` is the Power BI Desktop project entry point.
- `sales.Report/` contains the report definition. `definition.pbir` links the report to the semantic model. Under `definition/pages/`, `pages.json` controls page order, each page folder contains `page.json`, and each `visuals/<id>/` folder contains a visual definition. Bookmarks and report resources are stored beside the pages.
- `sales.SemanticModel/` contains the semantic model in TMDL format. `definition/model.tmdl` is the model manifest. Tables, relationships, expressions, functions, roles, cultures, and perspectives are split into matching files under `definition/`.
- `DAXQueries/` and `TMDLScripts/` contain saved development queries and scripts. 

When editing, change the report JSON for layout or visual behavior and the TMDL files for data-model behavior. Preserve generated page, visual, bookmark, and verified-answer identifiers unless the task explicitly requires replacing them.
