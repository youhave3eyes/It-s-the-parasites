# itstheparasites.com

Parasite education website and detox guide.

## Files

| File | What it is |
|---|---|
| `index.html` | The homepage walkthrough |
| `guide.html` | The Parasite Detox Guide page |
| `parasite-detox-guide.pdf` | The downloadable e-book |
| `CNAME` | Connects the site to the itstheparasites.com domain |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Put it online with GitHub Pages

1. Create a new repository on GitHub (for example `itstheparasites`).
2. Click **Add file → Upload files**, drag in everything from this folder, and commit.
   - `.nojekyll` is a hidden file. If your computer hides it, you can skip it. The site still works.
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, and save.
4. In a minute or two the site is live at `https://YOUR-USERNAME.github.io/itstheparasites/`.

## Connect your domain

The `CNAME` file already says `itstheparasites.com`. At your domain registrar, add these DNS records:

- Four **A** records for `@` pointing to:
  `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- A **CNAME** record for `www` pointing to `YOUR-USERNAME.github.io`

Then in **Settings → Pages**, enter `itstheparasites.com` as the custom domain and tick **Enforce HTTPS** once it's available.

If you don't own the domain yet, delete the `CNAME` file before uploading.

## Making changes

- **Your herb kit:** in `guide.html`, search for `Coming soon` and replace the placeholder text with your kit name, price and a buy link.
- **Affiliate links:** search `guide.html` for `iherb.com` and `mountainroseherbs.com` and swap in your own links.
- **Your own videos:** upload an `.mp4` (for example `videos/cricket.mp4`), then in `index.html` find the `REAL={` list and add `video:"videos/cricket.mp4",` to that entry. It will play inside the pop-up instead of linking out.
