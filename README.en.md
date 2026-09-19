# Q Mimi

[简体中文](README.md) · **English**

Q Mimi is a blue-and-yellow cat pet wearing a small golden pixel Q.

![Q Mimi preview](preview.gif)

[Preview the animations](https://aha-xiaoq.github.io/projects/q-mimi/?lang=en).

## Install and use

1. Open the [Q Mimi page](https://aha-xiaoq.github.io/projects/q-mimi/?lang=en) and click **Install in Codex**.
2. Allow your browser to open Codex, then click **Install**.
3. Click **Use this pet**. If the pet is hidden, enter `/pet` in Codex.

Prefer a download? [Download the ZIP](https://aha-xiaoq.github.io/projects/q-mimi/q-mimi.zip), extract it, and double-click **START.en.html** for the same install button. No commands or folder setup needed for this import flow.

Requires an internet connection and Codex desktop with pet import support. If nothing opens, update the app and try again. The app asks you to confirm installation and selection.

<details>
<summary>Alternative installation and troubleshooting</summary>

If your client does not support the import button, give Codex the extracted folder and ask:

> Install Q Mimi from this folder as a local custom pet. Confirm the actual CODEX_HOME, copy pet.json and spritesheet.webp into pets/q-mimi, and back up any existing files first. Keep the artwork unchanged. Tell me how to select it in Pets and show it with /pet.

For manual installation, put `pet.json` and `spritesheet.webp` together in `%USERPROFILE%\.codex\pets\q-mimi\` on Windows, or `~/.codex/pets/q-mimi/` on macOS. If `CODEX_HOME` is configured, use `pets/q-mimi/` inside that directory. Back up existing files before replacing them. In **Settings → Pets**, refresh and select **Q咪**, then enter `/pet` or choose **Show pet**. Labels may vary by app version.

If Q Mimi is missing, check that the two files are directly inside `q-mimi` and refresh the pet list. If motion is reduced, check your system's reduced-motion setting. This v2 desktop atlas is not compatible with web uploaders requiring a 1536 × 1872 image.

See the [official Pets guide](https://learn.chatgpt.com/docs/pets) for desktop controls. Import support varies by client version.

</details>

### Files

- `pet.json`: Configuration with the identifier `q-mimi` and sprite format version 2. The picker name remains **Q咪**.
- `spritesheet.webp`: Transparent 1536 × 2288 animation atlas, with 8 columns and 11 rows of 192 × 208 cells.
- `preview.gif`: Animated preview, not the installation atlas.

The atlas includes nine regular action groups and sixteen look directions. Keep the configuration and atlas together with their original filenames. A compatible host application is required.

### License and attribution

The Q Mimi atlas, preview, configuration and documentation are licensed under **CC BY-NC 4.0 (Attribution–NonCommercial)**. Noncommercial use, sharing and adaptation are permitted. When sharing publicly, retain attribution, source and license links, and indicate changes. For commercial permission, contact the author through [Issues](https://github.com/Aha-xiaoQ/q-mimi/issues).

Suggested credit: **Q Mimi · 在下_小Q (Aha_xiaoQ)**. Source: https://github.com/Aha-xiaoQ/q-mimi . License: CC BY-NC 4.0. Add a description of any changes you made.

See [LICENSE](LICENSE) for the full terms and [NOTICE.md](NOTICE.md) for scope. The character imagery was created with AI assistance. Permission covers only rights the licensor can grant; no claim is made that every generated element is copyright-protected in every jurisdiction. This is not an official OpenAI pet and is not endorsed by OpenAI.
