# Aishwarya's personal website

A simple personal portfolio made with HTML, CSS, and a tiny bit of JavaScript. It works offline and needs no installation, build command, or web server.

## 1. Open it on your computer

1. Open this project folder in Finder (Mac) or File Explorer (Windows).
2. Double-click `index.html`. It should open in your default browser.
3. If you edit a file, save it and refresh the browser page to see the change.

Keep `index.html`, `styles.css`, `script.js`, and the `images` folder together. The site uses relative paths so it also works from a local folder.

## 2. Edit your words and images

Open `index.html` in a text editor. The introduction draws on your LinkedIn pitch, and the career details come from your CV. Edit any wording or figures there as your experience changes:

- Edit the hero introduction and About paragraphs.
- Change the focus area and tool labels.
- Edit the three selected impact cards. Their links lead to the contact section because these client engagements do not have public project pages. Copy a whole `<article class="project-card">...</article>` block to add another, or delete one to show fewer.
- Update the Experience and Education entries.
- Update the email address, LinkedIn URL, and GitHub URL in the Contact section if they change.
- Update the page `<title>`, meta description, and Open Graph description if you change the site's focus.

Your portrait is `images/aishwarya-portrait.jpg`. To change it, copy a new picture into the `images` folder and change the hero `<img src>` in `index.html`. The three project illustrations are **placeholder artwork**; replace them with images you have permission to publish and update each image's `src` and descriptive `alt` text. Recommended project image size: about 1200 × 900 pixels. `images/social-preview.svg` is the sharing image; replace it and update the `og:image` path if you want. Some social platforms may require an absolute public URL for the Open Graph image after deployment.

Colors are near the top of `styles.css` in the `:root` block. A dark palette appears near the bottom under `prefers-color-scheme: dark`. All fonts are already installed on typical computers; there are no online font requests.

## 3. Push updates to GitHub

This folder is already connected to [your Personal-Portfolio repository](https://github.com/aishwarya-rav18/Personal-Portfolio). After making changes, open a terminal in this folder. On a Mac, you can drag the folder into a Terminal window after typing `cd `, then press Return. Run:

```sh
git add .
git commit -m "Update website"
git push
```

If Git asks you to sign in, follow GitHub's prompts. You can also upload changed files directly through the repository's **Add file** > **Upload files** menu.

## 4. Deploy on Netlify

1. Sign in to [Netlify](https://app.netlify.com) and connect your GitHub account if prompted.
2. Select **Add new project** > **Import an existing project**.
3. Choose **GitHub**, then select `aishwarya-rav18/Personal-Portfolio`.
4. Leave the **build command empty**. Set the **publish directory to the project root** (often shown as `.`; if Netlify already indicates the root, leave it unchanged).
5. Select **Deploy**. Netlify will give you a public site address. Every future push to the connected GitHub branch will trigger a new deployment automatically.

Before sharing the site, review the public career details and replace any project artwork you do not want to use.
