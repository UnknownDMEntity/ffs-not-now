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

v0.9.5.4 is the Windows x64 portable pilot release. It is self-contained and
unsigned; the exact EXE is 51,736,687 bytes with SHA-256
C5A124EB80BC0537C12664E804B0E89EB84F0CEA34CA355E708035E6D6967A16.
New users get Windows sign-in startup after the first launch and Toast reminders.
Existing saved choices are preserved. The owner confirmed launch and matching
preferences on the development laptop; its startup command points to the new EXE.
DeepAV prevented this exact build until the owner saved a false-positive entry.
The restored file matched the original checksum. Earlier v0.9.5.3 remains
available; v0.9.5.1 assets remain in their withdrawn draft.

The manifest retains the checker fields version, downloadUrl and releaseNotesUrl.
It uses numeric version 0.9.5.4 and the explicit /releases/tag/v0.9.5.4 page.
status=pilot and sha256 are informational: existing clients do not use them for
channel filtering or automatic binary verification. Any FFS user who chooses a
check uses this same endpoint; the pilot label is not an access restriction.

Checks are optional and off by default. They announce a newer version and offer
the release page; downloading and switching EXEs remain manual. Publish and
verify future assets before advancing the manifest. /releases/latest does not
select pre-releases. Installer/Store packaging remains a future milestone.

Public assets contain only the selected EXE, checksum and user instructions.
Keep source archives, Distribution Prep ZIPs, build folders, keys and private logs
out of this public repository and its releases.

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
