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

The v0.9.5.1 Windows x64 portable pre-release is temporarily withdrawn while remaining
release checks and feedback setup are completed. The user verified its local launch
and About destinations on October 7, 2026. Its existing assets are preserved in a draft
release; the EXE is self-contained and unsigned. The site shows the pause instead of
offering an unavailable download.

The manifest keeps the existing checker fields (`version`, `downloadUrl`,
`releaseNotesUrl`). During this pause, `version` is null and `status` is
`download-paused`. Existing clients return an unsuccessful update check without
advertising an unavailable update or claiming they are up to date. Resume with the
numeric release version and explicit pre-release URL only after publication and
desktop launch verification. GitHub's `/releases/latest` route does not select
pre-releases.

Automatic update checks remain off by default. Publish future manifest versions only
after their downloads are available. Include the actual SHA-256 and signing status
with each released binary. Windows installer and Microsoft Store distribution are
separate future milestones.

Upload only deliberately selected distribution files to public releases. Never upload
the Distribution Prep ZIP, source archives, build folders, signing keys or private logs.

## Feedback

support.html is the ordinary-user feedback page. It prepares bug reports and
suggestions in the browser, with preview, copy and text-file download. Drafts
are not uploaded or stored automatically; no GitHub account is needed.

The owner confirmed the dedicated support inbox ffsnotnowhelpdesk@outlook.com on
October 8, 2026. The email option opens the visitor's mail app for their own review
and send; it is not background delivery. If the encoded email-draft URL would be
longer than 2000 characters, the page asks the visitor to save and attach the text
file themselves. A visible address and copy instructions support visitors whose
browser does not open an email app. The privacy page explains email delivery and
storage. No test email has been sent by the assistant.

Optional GitHub forms remain under Advanced. Templates are in
.github/ISSUE_TEMPLATE/. Submissions and attachments there are public and require
a GitHub account. No private app source is published here.
