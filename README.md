diff --git a/README.md b/README.md
index c9740cbef7d03df5debd035d60465b6be4e07975..2b1a58a24fe567f78f9721f2cd1d1ea41fbf20bb 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,33 @@
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
+### 2) Open the game in your browser
+Visit:
+
+<http://localhost:4173>
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
+## Tips for best experience
+
+- Use a desktop/laptop with hardware acceleration enabled for smoother graphics.
+- If frame rate is low, close other GPU-heavy apps/tabs.
+- The game is rendered with bloom + film post-processing, so it is intentionally GPU intensive.
