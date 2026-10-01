# FFS, Not Now! — Public site/support repository

This repository is intended to be public.

It contains:
- the GitHub Pages website;
- privacy/release information;
- update manifest;
- public bug/feature issue templates;
- eventually release binaries.

It intentionally does not contain the private application source code.

## Enable GitHub Pages

In this repository, open **Settings → Pages**. Under **Build and deployment**,
choose **Deploy from a branch**, select **main** and **/(root)**, then **Save**.

After deployment, check:

- Website: https://unknowndmentity.github.io/ffs-not-now/
- Privacy: https://unknowndmentity.github.io/ffs-not-now/privacy.html
- Release notes: https://unknowndmentity.github.io/ffs-not-now/release-notes.html
- Support: https://unknowndmentity.github.io/ffs-not-now/support.html
- Manifest: https://unknowndmentity.github.io/ffs-not-now/update-manifest.json

These addresses require Pages to be enabled; uploading files alone does not enable it.
The `.nojekyll` file allows the prepared static site to be served directly.

GitHub's setup instructions:
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Release status and update manifest

[v0.9.5.1](https://github.com/UnknownDMEntity/ffs-not-now/releases/tag/v0.9.5.1) is a
Windows x64 portable pre-release. The selected EXE is self-contained and unsigned.
Its assets include `FFS_Not_Now.exe`, `SHA256SUMS.txt` and `README.txt`.

The manifest uses the existing checker schema (`version`, `downloadUrl`,
`releaseNotesUrl`) and points to the explicit pre-release URL. GitHub's
`/releases/latest` route does not select pre-releases.

Automatic update checks remain off by default. Publish future manifest versions only
after their downloads are available. Include the actual SHA-256 and signing status
with each released binary. Windows installer and Microsoft Store distribution are
separate future milestones.

Upload only deliberately selected distribution files to public releases. Never upload
the Distribution Prep ZIP, source archives, build folders, signing keys or private logs.

## Feedback

Bug and feature forms live in `.github/ISSUE_TEMPLATE/`. Submissions and attachments
are public; the site and forms explain this before users share diagnostics.
