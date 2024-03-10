---
share: "true"
---

## Setup to edit this page
---
1. Install [obsidian](https://obsidian.md/)
2. Install [git](https://git-scm.com/)
3. Get invited to [vlab-kaist](https://github.com/vlab-kaist) Organization
4. Clone the [VLMS](https://github.com/vlab-kaist/VLMS) repository and open it with obsidian.
5. Install obsidian community plugin 'Git'.
6. Set up your access token and edit the markdown files.
7. Use obsidian command 'Git: create backup' to push.
   Pushing will automatically build and deploy edited version.

<br/>

   >[!Warning]
   > - You should pull repository before you edit. Settings of plugin 'Git' (**Pull updates on startup**) will be useful.
   > - 'Github Publisher' plugin can make error when collaborating, avoid using it.

## Setup to preview
---
1. Install [Node.js](https://nodejs.org/en)
2. Run 'npm ci' to install dependencies.
3. Run following command to preview page at your local machine.

```bash
npx quartz build --serve
```