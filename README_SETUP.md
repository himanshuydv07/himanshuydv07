# 📦 GitHub Profile Package — Setup Guide

**For:** Himanshu Yadav (`himanshuydv07`)
**All links are already filled in. No placeholders remain.**

---

## 🗂️ What's Inside

```
github-profile-package/
├── README.md                         ← Your profile README (upload this)
├── README_SETUP.md                   ← This file
├── LICENSE                           ← MIT License
├── assets/
│   ├── hero.svg                      ← Animated hero banner
│   ├── terminal.svg                  ← Terminal info card
│   ├── architecture.svg              ← SyncSheet architecture diagram
│   ├── divider.svg                   ← Section divider
│   └── footer.svg                    ← Animated footer
└── .github/
    └── workflows/
        ├── snake.yml                 ← Contribution snake animation (auto)
        ├── metrics.yml               ← GitHub metrics SVGs (needs secret)
        └── leetcode.yml              ← LeetCode stats auto-update
```

---

## ✅ Step-by-Step: Go Live in 10 Minutes

### Step 1 — Create the special profile repository

1. Go to **github.com/new**
2. Set the repository name to exactly: **`himanshuydv07`**
   *(It must match your GitHub username exactly — this is what makes it a profile README)*
3. Set visibility to **Public**
4. **Do not** tick "Add a README file"
5. Click **Create repository**

---

### Step 2 — Upload the files

**On your computer, open Terminal / Command Prompt in the unzipped folder, then run:**

```bash
git init
git remote add origin https://github.com/himanshuydv07/himanshuydv07.git
git add .
git commit -m "feat: add GitHub profile README"
git branch -M main
git push -u origin main
```

> If you get an authentication error, use GitHub Desktop or upload files manually via the GitHub website.

**Manual upload (no terminal needed):**
1. On the new repo page, click **"uploading an existing file"**
2. Drag the entire unzipped folder contents (README.md, assets/, .github/)
3. Click **Commit changes**

---

### Step 3 — Enable GitHub Actions

1. In your `himanshuydv07` repo, go to **Settings → Actions → General**
2. Under **Workflow permissions**, select **"Read and write permissions"**
3. Click **Save**

---

### Step 4 — Run the Snake animation (one-time)

1. Go to **Actions** tab in your repo
2. Click **🐍 Snake Contribution** in the left list
3. Click **Run workflow → Run workflow**
4. Wait ~1 minute — it creates an `output` branch with the SVG
5. Your README will now show the animated snake

---

### Step 5 — Set up GitHub Metrics (optional but great)

This generates rich stat SVGs automatically.

1. Create a Personal Access Token:
   - Go to **github.com → Settings → Developer settings → Personal access tokens → Tokens (classic)**
   - Click **Generate new token (classic)**
   - Name it `METRICS_TOKEN`
   - Enable these scopes: ✅ `repo` · ✅ `read:user` · ✅ `read:org`
   - Click **Generate token** and **copy it immediately**

2. Add it as a secret:
   - Go to your `himanshuydv07` repo → **Settings → Secrets and variables → Actions**
   - Click **New repository secret**
   - Name: `METRICS_TOKEN`
   - Value: paste the token
   - Click **Add secret**

3. Go to **Actions → 📊 GitHub Metrics → Run workflow**

---

### Step 6 — Check your profile

Visit **github.com/himanshuydv07** — your profile README is now live!

---

## 🔗 All Your Links (Already in the README)

| Platform | Link |
|----------|------|
| GitHub | https://github.com/himanshuydv07 |
| LinkedIn | https://www.linkedin.com/in/himanshu-ydv04/ |
| Portfolio | https://himanshuyadav-chi.vercel.app/ |
| LeetCode | https://leetcode.com/u/cWv1Md4JO4/ |
| Codeforces | https://codeforces.com/profile/Himanshu_ydv__ |
| GeeksforGeeks | https://www.geeksforgeeks.org/profile/himanshuhuoo |
| Email | himanshuydv0007@gmail.com |

---

## ⚠️ One Thing Still to Do

The **SyncSheet project repo link** points to `github.com/himanshuydv07/syncsheet` — if that repo has a different name, update line 265 in `README.md`:

```md
[![GitHub](https://img.shields.io/badge/GitHub-Source...)](https://github.com/himanshuydv07/YOUR_ACTUAL_REPO_NAME)
```

Same for the **Cinematics Weather** and **Forensics** GitHub links — update them to your actual repo names once you know them.

---

## ❓ Troubleshooting

| Issue | Fix |
|-------|-----|
| SVGs not showing | Make sure `assets/` folder is uploaded alongside `README.md` at repo root |
| Snake animation shows broken image | Run the snake workflow manually first (Step 4) |
| Stats cards show "not found" | Double-check `himanshuydv07` matches your exact GitHub username |
| Metrics workflow fails | Make sure `METRICS_TOKEN` secret is added (Step 5) |
| Actions tab doesn't show | Enable Actions in repo Settings → Actions → General |
