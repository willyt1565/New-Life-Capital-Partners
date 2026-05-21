# Deployment Guide — New Life Capital Partners

This site is **plain HTML/CSS/JS**, so it hosts on **GitHub Pages** for free with
full HTTPS. No build step, no server.

- **Repository:** https://github.com/willyt1565/New-Life-Capital-Partners
- **Live URL (after step 2):** https://willyt1565.github.io/New-Life-Capital-Partners/
- **Custom domain (later):** https://newlifecapitalpartners.com

---

## Step 1 — Push the site to GitHub

Open Terminal and paste this block. It runs from your project folder.

```bash
cd "/Users/ann/Documents/Claude/Projects/NLCP"
git init
git branch -M main
git remote add origin https://github.com/willyt1565/New-Life-Capital-Partners.git
git add .
git commit -m "Launch: homepage prototype — Refined Dark Luxury"
git push -u origin main
```

**If it asks for a username and password:** GitHub no longer accepts your
account password here. Use a **Personal Access Token** as the password —
create one at GitHub → Settings → Developer settings → Personal access tokens →
Tokens (classic) → Generate new token, with the `repo` scope ticked. On a Mac
the token is saved to your keychain after the first use, so you only do this once.

**If `git remote add` says the remote already exists:** run
`git remote set-url origin https://github.com/willyt1565/New-Life-Capital-Partners.git`
and then re-run from `git add .`.

---

## Step 2 — Turn on GitHub Pages

1. Open the repository on GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Branch: **main**, folder: **/ (root)**. Click **Save**.
5. Wait about a minute, then refresh. Your site is live at:
   **https://willyt1565.github.io/New-Life-Capital-Partners/**

---

## Step 3 — Updating the site (every change after launch)

Whenever files change, publish the update with three commands:

```bash
cd "/Users/ann/Documents/Claude/Projects/NLCP"
git add .
git commit -m "Describe what changed here"
git push
```

GitHub Pages redeploys automatically within about a minute.

---

## Step 4 — Connect the custom domain (do this when ready)

The `CNAME` file is currently kept out of the repo (via `.gitignore`) so the
site stays viewable at the GitHub URL. To connect `newlifecapitalpartners.com`:

**a) At your domain registrar**, add these DNS records:

| Type  | Host / Name | Value |
|-------|-------------|-------|
| A     | @           | 185.199.108.153 |
| A     | @           | 185.199.109.153 |
| A     | @           | 185.199.110.153 |
| A     | @           | 185.199.111.153 |
| CNAME | www         | `willyt1565.github.io` |

**b) In GitHub → Settings → Pages → Custom domain**, enter
`newlifecapitalpartners.com` and **Save**. GitHub creates its own `CNAME` file
in the repo automatically.

**c)** Once the domain verifies (minutes to 24 hours), tick **Enforce HTTPS**.
That issues the free SSL certificate and gives you full `https://`.

---

## Quick reference

| Task | Where |
|------|-------|
| Repository | https://github.com/willyt1565/New-Life-Capital-Partners |
| GitHub URL | https://willyt1565.github.io/New-Life-Capital-Partners/ |
| Pages settings | Repo → Settings → Pages |
| Push an update | `git add .` → `git commit -m "..."` → `git push` |

> Prefer not to run commands yourself? A GitHub connector can let me manage the
> repository directly — just ask and I'll walk you through connecting it.
