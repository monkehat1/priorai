# PriorAI — Deploy to Website (No Terminal Needed)

Follow these steps exactly and your app will be live on the internet in ~10 minutes.

---

## Step 1 — GitHub (free)

1. Go to **github.com** and create a free account (or log in)
2. Click the **+** icon (top right) → **"New repository"**
3. Name it: `priorai`
4. Leave everything else as default → click **"Create repository"**
5. On the next screen, click **"uploading an existing file"**
6. Open this zip, select ALL the files inside the `priorai-v2` folder
   (index.html, manifest.json, sw.js, netlify.toml, + the icons and netlify folders)
7. Drag them ALL into the GitHub upload box
8. Click **"Commit changes"**

---

## Step 2 — Netlify (free)

1. Go to **app.netlify.com** and sign up free (use your GitHub account to sign in)
2. Click **"Add new site"** → **"Import an existing project"**
3. Click **"GitHub"** → authorize → select your `priorai` repo
4. Leave ALL build settings blank/default
5. Click **"Deploy site"**

Netlify gives you a live URL like: `https://priorai-abc123.netlify.app`

---

## Step 3 — Add your Anthropic API key (so AI works)

1. In Netlify, go to your site → **Site configuration** → **Environment variables**
2. Click **"Add a variable"**
3. Key: `ANTHROPIC_API_KEY`
4. Value: your `sk-ant-...` key
5. Click **Save**
6. Go to **Deploys** → click **"Trigger deploy"** → **"Deploy site"**

---

## Step 4 — Done!

Visit your Netlify URL — your app is live.

Share the link with anyone. On mobile they can tap
"Add to Home Screen" to install it like a native app.

---

## Updating the app in future

1. Make changes to your files
2. Go to your GitHub repo → click the file → click the pencil icon to edit
   OR drag new files into the repo to replace them
3. Netlify auto-redeploys within 30 seconds

---

## Custom domain (optional, ~$10/year)

1. Buy a domain at **namecheap.com** (e.g. priorai.app)
2. In Netlify → Domain management → Add custom domain
3. Follow Netlify's DNS instructions (takes ~10 min)
