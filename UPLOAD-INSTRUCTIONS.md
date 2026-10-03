# How to get this onto GitHub

No terminal, no tokens, no command line. Five minutes.

## 1. Create the repository
Go to **github.com/new**

- Repository name: `psc-ai-systems`
- Description: `Production AI systems designed, built and deployed solo. Agent orchestration, autonomous pipelines, full-stack applications.`
- Set it to **Public** (the whole point is that people can see it)
- Do **not** tick "Add a README", you already have one
- Click **Create repository**

## 2. Upload the files
On the empty repo page, click **uploading an existing file**.

Unzip the folder on your computer, then drag **the contents** of `psc-ai-systems` into the browser window, not the folder itself. GitHub preserves the subfolders.

Scroll down, commit message `Initial commit`, click **Commit changes**.

## 3. Make it look intentional
On the repo page, click the gear icon beside **About** on the right:

- Add the description again
- Website: `penelopesloan.biz`
- Topics: `ai` `llm` `claude` `agents` `automation` `nextjs` `supabase` `n8n` `solutions-architecture`

## 4. Turn the estimator into a live demo
**Settings** → **Pages** → Source: `Deploy from a branch` → Branch: `main`, folder: `/ (root)` → **Save**

After a minute the tool is live at:
`https://[your-username].github.io/psc-ai-systems/tools/themis-estimator/`

Put that link in the README and in your resume. A working demo beats a description.

## 5. Pin it
On your GitHub profile, **Customize your pins** and pin this repo so it is the first thing anyone sees.

---

## Before you upload, two minutes of checking

**Never commit secrets.** No API keys, no tokens, no `.env` files, no client data. The `.gitignore` covers the usual suspects but it only protects files you add later, not files you drag in today. Look before you drop.

**Fill the TO ADD notes.** Each system doc ends with an HTML comment listing what would make it stronger: a diagram, a sanitised screenshot, an agent list. Those comments are invisible on GitHub, so they are safe to leave, but the docs get considerably more convincing once you fill them.

**Check the honest note.** `docs/stack.md` ends with a paragraph naming what you are still growing into. I believe it helps you rather than hurts you, because hiring managers trust self-aware candidates and it pre-empts the exact question a technical interviewer would otherwise catch you with. If you disagree, delete it, it is your call not mine.
