# InfoMD

A Markdown viewer and editor for Windows. Double-click a `.md` file and it opens, formatted and
ready to read or edit. There is no vault to set up, no account, and no telemetry.

This page holds the installers and the update feed only. The source code is not published here.

## Download

**[Get the latest version](https://github.com/jrauseo/infomd-releases/releases/latest)**

Under **Assets**, pick one:

| File | Use it when |
|---|---|
| `InfoMD_<version>_x64-setup.exe` | You are installing it for yourself. No admin rights needed. |
| `InfoMD_<version>_x64_en-US.msi` | IT is deploying it with Intune or Group Policy. |

Requires Windows 10 or 11, 64-bit.

## Install

1. Download `InfoMD_<version>_x64-setup.exe` and run it.
2. Windows shows a blue **"Windows protected your PC"** box. Click **More info**, then
   **Run anyway**. Your browser may also ask you to **Keep** the download first.
3. Follow the installer. It installs for your user account only.

**About that warning:** these early builds are not yet signed with a publicly trusted
certificate, so Windows cannot identify the publisher. That is expected for now and will go away
once signing is in place. If you want to check your download, compare its SHA-256 with
`SHA256SUMS.txt` on the release page:

```powershell
Get-FileHash .\InfoMD_0.1.0_x64-setup.exe -Algorithm SHA256
```

## Open Markdown files with InfoMD

Windows does not let an installer make itself the default app, so do this once:

1. Right-click any `.md` file.
2. Choose **Open with > Choose another app**.
3. Pick **InfoMD**, then **Always**.

From then on, double-clicking a Markdown file opens it in InfoMD.

## Using it

**Three ways to view a document** (switch with the buttons in the toolbar, or `Ctrl+E`):

| Mode | What you see |
|---|---|
| Live | Formatting shown as you type. The Markdown symbols appear only on the line you are on. |
| Source | The raw Markdown text. |
| Reading | The finished page, read-only. |

**Formatting without knowing Markdown:** the Format panel on the right has buttons for bold,
italic, headings, lists, quotes, links, images, tables and code blocks, like the toolbar in
Word.

**Working with a folder of notes (optional):** `Ctrl+Shift+O` opens a folder. You get a file
tree, search across every note, and `[[links]]` between notes. Nothing is added to the folder.

**Shortcuts**

| Keys | Action |
|---|---|
| `Ctrl+O` | Open a file |
| `Ctrl+N` | New file |
| `Ctrl+S` | Save |
| `Ctrl+Shift+S` | Save as |
| `Ctrl+W` | Close tab |
| `Ctrl+E` | Switch mode |
| `Ctrl+F` | Find |
| `Ctrl+Shift+O` | Open a folder |
| `Ctrl+P` | Go to a file in the folder |
| `Ctrl+Shift+F` | Search the folder |
| `Ctrl+B` / `Ctrl+I` / `Ctrl+K` | Bold / italic / link |
| `Ctrl+Shift+P` | Print |

**Export to PDF:** the PDF button in the toolbar saves the document as a PDF.

## Updates

InfoMD checks this page for a newer version when it starts. You can also check by hand: click the
**i** button at the bottom left, then **Check for updates**. The automatic check can be turned off
in the same window. Checking for updates is the only time InfoMD uses the network.

## Uninstall

**Settings > Apps > Installed apps**, find **InfoMD**, and choose **Uninstall**.

## Feedback

Found a problem or have a request? [Open an issue](https://github.com/jrauseo/infomd-releases/issues).

---

Copyright © 2026 Infonaligy Partners, Inc. All rights reserved. InfoMD is early software and is
provided as is, without warranty.
