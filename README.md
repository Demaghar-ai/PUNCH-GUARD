# Punch Guard

A 2-player, hot-seat boxing mind game. Pick 3 moves each conflict, then watch
them clash beat-by-beat — speed, guard, sway, combos and timing priority all
matter. Pure static HTML/CSS/JS, no build step, no dependencies.

## Run it locally

Just open `index.html` in a browser. That's it — no server, no install.

## Deploy: GitHub + Vercel

### 1. Push to GitHub

From this folder:

```bash
git init
git add .
git commit -m "Punch Guard"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

(Create the empty repo on GitHub first at github.com/new — don't initialize
it with a README, or you'll need to `git pull --rebase` before pushing.)

### 2. Deploy on Vercel

**Option A — Dashboard (easiest):**
1. Go to [vercel.com/new](https://vercel.com/new) and sign in with GitHub.
2. Import the repo you just pushed.
3. Framework preset: leave as **Other** — no build command, no output
   directory needed (it's a single static `index.html`).
4. Click **Deploy**. You'll get a live `*.vercel.app` URL in under a minute.

**Option B — CLI:**
```bash
npm i -g vercel
vercel        # deploys a preview
vercel --prod # deploys to production
```

### 3. Updates

Any future push to `main` on GitHub auto-redeploys on Vercel — no extra
steps needed.

## Project structure

```
index.html    the entire game (HTML + CSS + JS, self-contained)
vercel.json   minimal config (clean URLs)
.gitignore
README.md
```
