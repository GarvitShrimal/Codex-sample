diff --git a/README.md b/README.md
index c9740cbef7d03df5debd035d60465b6be4e07975..3ef2bb34e4df1c93cd2ed1cd5845ed044fd0232d 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,125 @@
-# Codex-sample
-dih
+# Neon Apex Hyper Racing
+
+A high-intensity futuristic racing game built with Three.js and post-processing bloom/film effects.
+
+## How to view and play
+
+### 1) Start a local web server
+From the project folder, run:
+
+```bash
+python3 -m http.server 4173
+```
+
+Keep this terminal open while you play.
+
+### 2) Open the game in your browser
+Use one of these URLs in the **same machine** where you started the server:
+
+- <http://localhost:4173>
+- <http://127.0.0.1:4173>
+
+### 3) Play
+Use these controls:
+
+- `W` → accelerate
+- `S` → brake
+- `A / D` → steer left/right
+- `Shift` → boost (consumes boost meter, then recharges)
+- `Space` → drift
+- `R` → restart race
+
+## If "This site can't be reached" appears
+
+- Make sure the server is still running in your terminal.
+- If `localhost` fails, try `127.0.0.1`.
+- If you are in a remote/dev container, forward port `4173` and open the forwarded URL instead of localhost on your host machine.
+- Confirm the server is listening with:
+
+```bash
+curl -I http://127.0.0.1:4173
+```
+
+You should see an HTTP response like `200 OK`.
+
+## Step-by-step: upload this code to GitHub
+
+### Prerequisites
+
+- A GitHub account
+- `git` installed locally
+
+Check Git is installed:
+
+```bash
+git --version
+```
+
+### 1) Create a new empty repository on GitHub
+
+1. Sign in to GitHub.
+2. Click **New repository**.
+3. Name it (example: `neon-apex-hyper-racing`).
+4. Keep it **empty** (do not add README/.gitignore/license if you already have this local project).
+5. Click **Create repository**.
+
+### 2) Open your terminal in this project
+
+```bash
+cd /path/to/Codex-sample
+```
+
+### 3) Initialize Git (only if needed)
+
+If this folder is not already a Git repository:
+
+```bash
+git init
+```
+
+### 4) Commit your project files
+
+```bash
+git add .
+git commit -m "Initial commit: Neon Apex Hyper Racing"
+```
+
+### 5) Connect your local repo to GitHub
+
+Copy your GitHub repo URL and run:
+
+```bash
+git remote add origin https://github.com/<your-username>/<your-repo-name>.git
+```
+
+If `origin` already exists, update it:
+
+```bash
+git remote set-url origin https://github.com/<your-username>/<your-repo-name>.git
+```
+
+### 6) Push your code
+
+```bash
+git branch -M main
+git push -u origin main
+```
+
+### 7) Verify upload
+
+1. Refresh your GitHub repository page.
+2. Confirm you can see files like `index.html`, `game.js`, `style.css`, and `README.md`.
+
+## Optional: publish as a live site with GitHub Pages
+
+1. In your GitHub repo, go to **Settings → Pages**.
+2. Under **Build and deployment**, choose **Deploy from a branch**.
+3. Select branch `main` and folder `/ (root)`.
+4. Save and wait for deployment.
+5. Open the generated Pages URL to play online.
+
+## Tips for best experience
+
+- Use a desktop/laptop with hardware acceleration enabled for smoother graphics.
+- If frame rate is low, close other GPU-heavy apps/tabs.
+- The game is rendered with bloom + film post-processing, so it is intentionally GPU intensive.
