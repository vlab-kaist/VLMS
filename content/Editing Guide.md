---
share: "true"
---

## Setup to edit this page
---
1. Install [obsidian](https://obsidian.md/)
2. Install [git](https://git-scm.com/)
3. Get invited to [vlab-kaist](https://github.com/vlab-kaist) Organization
4. Clone the [VLMS](https://github.com/vlab-kaist/VLMS) repository and open it with obsidian.
5. Install obsidian community plugin 'Github Publisher'.
6. Set up your access token and edit the markdown files.
7. Pushing automatically build and deploy edited version.

For 'Github Publisher' Settings, set File Path to 'Obsidian Path' so that file structure is reflected to the page.
## Setup to preview
---
1. Install [Node.js](https://nodejs.org/en)
2. Run 'npm ci' to install dependencies.
3. Run following command to preview page at your local machine.
```bash
npx quartz build --serve
```