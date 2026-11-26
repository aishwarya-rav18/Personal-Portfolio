# Aishwarya's personal website

A simple personal portfolio made with HTML, CSS, and a tiny bit of JavaScript. It works offline and needs no installation, build command, or web server.

## 1. Open it on your computer

1. Open this project folder in Finder (Mac) or File Explorer (Windows).
2. Double-click `index.html`. It should open in your default browser.
3. If you edit a file, save it and refresh the browser page to see the change.

Keep `index.html`, `styles.css`, `script.js`, and the `images` folder together. The site uses relative paths so it also works from a local folder.

## 2. Add your own words and images

Open `index.html` in a text editor. Search for `EDIT:` to find every spot meant for your information:

- Replace the tagline and both About paragraphs.
- Change the skill labels.
- Change each project name and description. Replace each project link's `href="#contact"` with the actual project URL, and update its `aria-label` to match. Copy a whole `<article class="project-card">...</article>` block to add a project, or delete one to show fewer.
- Replace the Experience and Education entries.
- Replace `hello@example.com` with your email address. Replace the LinkedIn and GitHub homepage URLs with your profile URLs. Remove any link you do not use.
- Update the page `<title>`, meta description, and Open Graph description if you change the site's focus.

The three images in `images/project-one.svg`, `project-two.svg`, and `project-three.svg` are **placeholder artwork**. To use your own pictures, copy them into the `images` folder, then change the matching `<img src="images/project-one.svg">` path in `index.html` to your filename (for example, `images/my-project.jpg`). Update the `alt` text to describe the new image. Recommended image size: about 1200 × 900 pixels. The decorative hero artwork is drawn in CSS in `styles.css`; you can keep it or replace the `.hero-art` area with your own photo. `images/social-preview.svg` is a placeholder sharing image; replace it with your own preview and update the `og:image` path in `index.html` if you want. Some social platforms may require an absolute public URL for the Open Graph image after deployment.

Colors are near the top of `styles.css` in the `:root` block. A dark palette appears near the bottom under `prefers-color-scheme: dark`. All fonts are already installed on typical computers; there are no online font requests.

## 3. Push it to a new GitHub repository

1. Sign in to [GitHub](https://github.com) and select **New repository** from the **+** menu.
2. Give it a name, such as `personal-portfolio`. Choose **Public** if you want anyone to see the code. Leave **Add a README file** unchecked because this project already has one. Select **Create repository**.
3. On your computer, open a terminal in this project folder. On a Mac, you can drag the folder into a Terminal window after typing `cd `, then press Return.
4. Run these commands one at a time, replacing `YOUR-USERNAME` and `YOUR-REPOSITORY` with your own values:

   ```sh
   git init
   git add .
   git commit -m "Add personal website"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
   git push -u origin main
   ```

If Git asks you to sign in, follow GitHub's prompts. For later updates, save your files, then run `git add .`, `git commit -m "Update website"`, and `git push` in this folder.

## 4. Deploy on Netlify

1. Sign in to [Netlify](https://app.netlify.com) and connect your GitHub account if prompted.
2. Select **Add new project** > **Import an existing project**.
3. Choose **GitHub**, then select the repository you created above.
4. Leave the **build command empty**. Set the **publish directory to the project root** (often shown as `.`; if Netlify already indicates the root, leave it unchanged).
5. Select **Deploy**. Netlify will give you a public site address. Every future push to the connected GitHub branch will trigger a new deployment automatically.

Before sharing the site, replace the placeholder text, email, profile links, and project images.
