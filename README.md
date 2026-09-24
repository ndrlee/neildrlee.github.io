# Neil Lee — personal website

Plain HTML + CSS. No build step — GitHub Pages serves these files as-is, so there's nothing to install and nothing that can break in a build.

## Files

- `index.html` — Home
- `research.html` — Research
- `policy-consultancy.html` — Policy / Consultancy
- `book.html` — Book
- `about.html` — About
- `assets/style.css` — shared styling
- `assets/Neil_Lee_CV.pdf` — **add your own CV file here** with this exact name, or update the link on `about.html` to match whatever you name it

## Publish it on GitHub Pages

1. On GitHub, create a new repository. If you want it at `https://<your-username>.github.io`, name the repository exactly `<your-username>.github.io`. Any other name works too, it'll just live at `https://<your-username>.github.io/<repo-name>/`.
2. Upload all the files in this folder to the repository (drag-and-drop on the GitHub website works fine, or `git push` if you're comfortable with the command line), keeping the `assets/` folder structure intact.
3. In the repository, go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then **Save**.
5. GitHub will give you a URL (something like `https://<your-username>.github.io/`) — it usually goes live within a minute or two.

## Using your existing domain (neillee.org)

If you'd like `neillee.org` to point at this site instead of Google Sites:

1. In **Settings → Pages** on the repository, enter `neillee.org` under **Custom domain** — this creates a `CNAME` file in the repo automatically.
2. At your domain registrar, update the DNS: an `A` record pointing to GitHub's Pages IP addresses (GitHub's Pages settings page shows you these once you add the custom domain), or a `CNAME` record pointing to `<your-username>.github.io` if you're using a `www` subdomain.
3. DNS changes can take anywhere from a few minutes to 24 hours to take effect.

## Updating content later

Every page is a separate file with plain HTML — open one in any text editor, find the paragraph or list item you want to change, edit the text between the tags, and save. Commit and push (or re-upload on GitHub) and the live site updates automatically, no rebuild needed.

To add a new publication to the Research page, copy an existing `<li>...</li>` line under the relevant `<ul class="pub-list">` and edit it.
