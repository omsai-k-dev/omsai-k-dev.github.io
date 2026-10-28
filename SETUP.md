# Publish Clear Memo privacy and app-ads.txt on GitHub Pages

These files are prepared locally, not hosted yet. The public contact supplied by the developer is omsai.k.dev / omsai.k.dev@gmail.com. Review the policy against the final app before publishing. No domain, repository settings or public content has been changed automatically.

## Recommended free setup

The application's existing Git remote is `omsai-k-dev/clear-memo`. Use the same GitHub owner for a separate **public website repository** named exactly:

`omsai-k-dev.github.io`

This produces the root site `https://omsai-k-dev.github.io/`. If a user-site repository already exists, preserve it and add these files carefully; do not replace an unrelated homepage. If you use another GitHub account, replace the owner in both the repository name and URLs.

1. Sign in to the intended GitHub account, click **+ → New repository**.
2. Enter `omsai-k-dev.github.io`, choose **Public**, and create it. Do not upload the Android app source to this website repository.
3. Choose **Add file → Upload files**. Upload the **contents** of `website/` at the repository root: `index.html`, `styles.css`, `app-ads.txt`, the `privacy/` folder containing `index.html`, and `.nojekyll` if your file picker shows it. `SETUP.md` is optional. Do not nest everything inside another `website` folder. Commit the upload to `main`.
4. Open **Settings → Pages → Build and deployment**. Choose **Deploy from a branch**, branch **main**, folder **/(root)**, then **Save**.
5. Wait for the deployment to finish. Open and check:
   - Homepage: `https://omsai-k-dev.github.io/`
   - Privacy policy: `https://omsai-k-dev.github.io/privacy/`
   - AdMob file: `https://omsai-k-dev.github.io/app-ads.txt`
6. The text file must show exactly:

```text
google.com, pub-3527968499532188, DIRECT, f08c47fec0942fa0
```

7. Use the privacy URL in **AdMob → Privacy & messaging** when configuring the Clear Memo message. Review and publish the message, then restart the app for a new consent check. Use the same privacy URL in the future Google Play listing.
8. Set the future Play listing's **developer website** to `https://omsai-k-dev.github.io/`. Link the published Play listing in AdMob, then verify app-ads.txt there. Hosting the file alone does not complete store linkage, app review, or verification.

Use this root user-site repository so app-ads.txt is at `/app-ads.txt`. A project site such as `https://omsai-k-dev.github.io/clear-memo/` puts it under a subpath unless a separate root file is also hosted.

This policy page has no scripts, cookies, analytics, external fonts or embedded ads. GitHub Pages itself handles hosting requests under GitHub's privacy practices. Do not put credentials, payment details, personal documents or audio in this public repository.

Official setup guide: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
