# Contributing to Awesome Obsidian Beta Plugins 🎉

Thanks for your interest in making this the go-to collection of Obsidian beta plugins! Your contributions help everyone discover and track cutting-edge tools.

---

## 📋 Table of Contents

1. [What You Can Do](#what-you-can-do)  
2. [Plugin Submission Workflow](#plugin-submission-workflow)  
3. [Plugin Status Definitions](#plugin-status-definitions)  
4. [Editing `beta-plugins.json`](#editing-pluginsjson)  
5. [Pull Request & Issue Guidelines](#pull-request--issue-guidelines)  
6. [Coding Style & Formatting](#coding-style--formatting)  
7. [CI / Validation](#ci--validation)  
8. [Need Help?](#need-help)  
9. [Code of Conduct](#code-of-conduct)

---

## What You Can Do

This project welcomes contributions in different forms:

- **Submit a new beta plugin** (via BRAT or other GitHub installs).  
- **Update metadata or status** of an existing plugin.  
- **Report issues** (duplicates, outdated entries, formatting errors).  
- **Improve tooling**, workflows, or documentation.

---

## Plugin Submission Workflow

1. Click **New Issue** → choose **🧪 Beta plugin submission** form.  
2. Fill in all details-ID, name, author, GitHub repo, description, and status.  
3. We'll review and merge your issue or PR.  
4. Our GitHub Action (if enabled) validates `plugins.json`.  
5. Watch the status tags; once a beta plugin is accepted upstream, update its status.

---

## Plugin Status Definitions

| Status         | Meaning                                                                 |
|----------------|-------------------------------------------------------------------------|
| `not submitted`| In this list only, no PR submitted upstream.                            |
| `submitted`    | PR created to `obsidian-releases/community-plugins.json` but pending. |
| `blocked`      | PR rejected or waiting on changes.                                      |
| `approved`     | Merged upstream-officially available in Obsidian's plugin browser.      |

---

## Editing `plugins.json`

- Keep the JSON **formatted** and **sorted** alphabetically by `id`.  
- Ensure each plugin object contains:
```json
{
  "id": "",
  "name": "",
  "author": "",
  "description": "",
  "repo": "",
  "status": ""
}
```

- Run `npm install -g jsonlint` and then run

```bash
jsonlint plugins.json
```

## Pull Request & Issue Guidelines

- PRs welcome! Please fork and submit a pull request with your changes.
- One plugin per PR or issue keeps review focused.
- Provide context if changing someone else's submission.
- Use descriptive titles.

## Coding Style & Formatting

- Use 2spaces for JSON formatting.
- Wrap long descriptions to ~80 characters.
- Keep consistent quote style (" for JSON).
- Validate JSON via CI (if available).

## CI / Validation

- If the GitHub Action based on json-schema-validator triggers on your PR, please fix any errors before merging. These include:
- Missing required keys
- Invalid status values
- JSON syntax issues

## Need Help?

- Browse existing issues for context.
- Drop a comment on your submitted PR if you're unsure about changes.
- Feel free to ask questions in issues or on Discord/forums where BRAT is discussed.

## Code of Conduct
This project follows the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to respect everyone by following these rules.
