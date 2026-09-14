# Atrayee Majumder — academic website

A responsive academic website made with plain HTML and CSS. No installation, JavaScript, or build step is needed. Content is based on the supplied CV. Professional contact email is included. The original CV PDF, home address, phone number, birth date, and referee contacts are not bundled.

## Open and edit

Open `index.html` in your browser after extracting the downloadable package. Edit text and links in `index.html`; edit colours, typography, and layout in `styles.css`. In the Sites source checkout these web files live in `dist/`; in the downloadable GitHub package they are at the top level.

## Upload through GitHub (no terminal required)

1. Sign in to https://github.com and create a new public repository named `YOUR-USERNAME.github.io`, replacing YOUR-USERNAME with your actual lowercase GitHub username. If that repository already exists, preserve or back up its current content before replacing files.
2. Extract the ZIP on your computer.
3. In the repository, select **Add file → Upload files** (or **uploading an existing file** in the empty repository).
4. Upload the extracted `index.html`, `styles.css`, and `favicon.svg` files at the repository root. You may also include this README and `.nojekyll`. Upload the files, not the ZIP or its enclosing folder.
5. Commit the files to `main`.
6. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select **main**, choose **/(root)**, and click **Save**.
7. The site will be available at `https://YOUR-USERNAME.github.io/`. Publication can take up to 10 minutes. Settings → Pages provides the actual published link.

## Push with Git instead

Install Git if needed. Create the public repository as above, but leave it empty: do not initialize it with a README, license, or .gitignore. Open Git Bash or a terminal in the extracted folder containing index.html, then run:

```bash
git init
git add .
git commit -m "Create academic website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
git push -u origin main
```

Replace both occurrences of YOUR-USERNAME. If Git asks for your author identity, configure your name and your GitHub email (or GitHub-provided no-reply email) before retrying the commit. Authenticate through Git's browser or credential-manager prompt; GitHub does not accept your account password for HTTPS Git operations. A personal access token is an alternative when prompted for a password. Never put a token into a remote URL or website file.

Then enable Pages using step 6 above. For future changes:

```bash
git add .
git commit -m "Update website"
git push
```

This new-repository procedure is not intended to overwrite an existing Git history. If a push is rejected because the repository already contains files, clone that repository, copy the website files into it, then commit and push normally. Do not force-push.

## Files

- `index.html`: profile, research, publications, academic experience, teaching, talks, and contact.
- `styles.css`: responsive styling and print layout.
- `favicon.svg`: browser-tab icon.
- `.nojekyll`: tells GitHub Pages to serve static files directly.

## Official instructions

- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
