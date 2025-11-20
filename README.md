# Investmant_Tracker_arun_

 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index a9a1ce8da19fe5c8f658d4404487c9f9b2b3f21c..0e1ddea0c10393507f48f9c07041a7e2751f8af2 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,14 @@
 # Investmant_Tracker
 All about tracking Investments
+
+## Authentication & database prototype
+- A simulated cloud database connection is established automatically when the page loads.
+- Use one of the demo logins to unlock live price fetching:
+  - `demo@tracker.in` / `demo123`
+  - `investor@clearcut.in` / `securepass`
+- Sessions persist locally so you remain signed in on refresh until you log out.
+
+## Run / deploy locally
+- Serve the app from the repo root with any static server (for example: `python3 -m http.server 8080`).
+- Open `http://localhost:8080/index.html` in your browser to use the tracker.
+- For a public URL, follow the recipes in [DEPLOYMENT.md](DEPLOYMENT.md) (GitHub Pages, Netlify drop, or Vercel). This environment cannot publish the link for you.
 
EOF
)
