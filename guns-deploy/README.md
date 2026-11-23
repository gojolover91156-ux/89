# 🌐 guns.lol → GitHub Pages Auto-Deployer

Drop your guns.lol zip file here and your site goes live automatically on GitHub Pages.

---

## 🚀 First-time setup (do once)

### 1. Create your GitHub repo

- Go to [github.com/new](https://github.com/new)
- Name it anything, e.g. `my-site`
- Set it to **Public**
- Click **Create repository**

### 2. Upload this repo's files

Upload everything from this folder into your new GitHub repo:
```
.github/
  workflows/
    deploy.yml
README.md
```

### 3. Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. Click **Save**

That's it! Now every time you push a zip, your site deploys automatically.

---

## 📦 How to update your site

1. Download a fresh zip from your guns.lol profile
2. **Delete the old zip** from your repo (if any)
3. Upload the new zip to the **root** of your repo (same level as this README)
4. GitHub Actions will automatically extract it and deploy

Your site will be live at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

---

## ✅ Checklist

- [ ] Repo is **Public**
- [ ] GitHub Pages source is set to **GitHub Actions**
- [ ] Zip file is in the **root** of the repo (not inside a folder)
- [ ] Only **one** zip file exists in the root at a time

---

## ❓ Troubleshooting

| Problem | Fix |
|---|---|
| Action fails with "No .zip file found" | Make sure your zip is in the repo root, not a subfolder |
| Site shows blank page | Check the Actions tab for errors; make sure your zip has an `index.html` |
| Old version still showing | GitHub Pages can take 1–2 minutes to update after a deploy |
| Action never ran | Go to **Actions** tab → select the workflow → click **Run workflow** |
