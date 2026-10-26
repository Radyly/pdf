# Browser PDF Editor — GitHub Pages

A static, browser-based PDF editor. It can combine PDF files, reorder pages, add annotations/text/images/signatures, and download the edited result.

## Publish with GitHub Pages

1. Sign in to [GitHub](https://github.com) and create a new repository, e.g. `pdf-editor`.
2. Upload `index.html` and `.nojekyll` to the **main** branch (you can upload `README.md` too).
3. Open **Settings → Pages**. Under **Build and deployment**, set **Source: Deploy from a branch**, **Branch: main**, **Folder: /(root)**. Click **Save**.
4. Open `https://YOUR-USERNAME.github.io/pdf-editor/` when deployment is finished. For a repo named `YOUR-USERNAME.github.io`, use `https://YOUR-USERNAME.github.io/`.

## Use

Open/Add PDF → edit or arrange pages → Export / Save PDF → Download PDF. To return to editing later, select **Save project** and restore the downloaded `.project.json` file.

## Data/privacy

No backend or account is required. PDF content is processed in the browser and is not sent to a server by this application. The HTML bundles the PDF libraries so it does not require external CDN scripts. GitHub still serves the website files and may receive standard access logs.

## Limitations

- This is a static browser app, not a shared server that saves files online. Downloads are saved on each visitor's device.
- 'Cover' visually hides text, but does not securely redact sensitive PDF contents.
- The 'Exact appearance' export flattens pages, so original text is not selectable; choose 'Preserve original selectable text' if needed.
- Existing digital signatures may be invalidated by editing.
- Use modern Chrome or Edge for best results; browser download settings can affect save behavior.
- Huge PDFs may exceed browser memory limits.

Libraries included in the original HTML: `pdf-lib` (MIT), PDF.js (Apache-2.0). Retain their license notices.
