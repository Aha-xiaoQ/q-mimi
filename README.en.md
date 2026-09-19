# Q Mimi

[简体中文](README.md) · **English**

Q Mimi is a blue-and-yellow cat pet wearing a small golden pixel Q.

![Q Mimi preview](preview.gif)

[Preview the animations](https://aha-xiaoq.github.io/projects/q-mimi/?lang=en).

### Use in Codex desktop

This is a custom pet asset pack, not a standalone desktop application. You do not need to regenerate any images. It requires a Codex desktop version that supports v2 custom pets. The local-folder instructions below use Windows as an example.

1. [Download the asset pack](https://aha-xiaoq.github.io/projects/q-mimi/q-mimi.zip) and extract it.
2. Enter `%USERPROFILE%\.codex\pets` in the File Explorer address bar. Create the directory if needed, then create a `q-mimi` folder inside it.
3. Put `pet.json` and `spritesheet.webp` in that folder. Back up any existing files with the same names before replacing them.
4. Open the pet picker in Codex, refresh the list and select **Q咪**. Versions with this entry may use **Settings → Pets**; labels and locations can vary by version.
5. Enter `/pet`, or choose **Wake Pet** from the command menu, to show the pet. Enter `/pet` again to hide it.

The final folder structure should be:

```text
%USERPROFILE%\.codex\pets\q-mimi\
├── pet.json
└── spritesheet.webp
```

Do not leave an extra extracted folder between `q-mimi` and these files. If you explicitly configured `CODEX_HOME`, use `pets/q-mimi/` inside that actual directory instead. The default macOS location is `~/.codex/pets/q-mimi/`. Not all operating systems and client versions have been individually tested.

Alternatively, give Codex the extracted folder and this request:

> Install Q Mimi from this folder as a custom pet on this computer. First confirm the actual CODEX_HOME, then place pet.json and spritesheet.webp in pets/q-mimi. Back up existing files with the same names. Do not regenerate the images or directly edit global state files. When finished, explain how to select and wake the pet.

### Troubleshooting

- **Q咪 is missing from the list:** Check the folder nesting and filenames. Keep both files together, refresh the pet list, and restart the app if needed.
- **Selected but not visible:** Use `/pet` or Wake Pet. Selecting a pet and displaying it are separate steps.
- **The pet is still:** Check the system's reduced-motion setting. Animations respond to app activity; they do not necessarily cycle through every action as the web preview does.
- **No Pets or `/pet` entry:** Check that your desktop client and version support pets. Web and IDE interfaces may use different installation methods. This pack uses a 1536 × 2288 v2 atlas and is not compatible with a web uploader that requires a 1536 × 1872 atlas.

See the [official OpenAI Pets documentation](https://learn.chatgpt.com/docs/pets). The former Codex documentation link redirects there, and that page uses the ChatGPT desktop name; follow the interface available in your installed version. The local-folder method follows the pet packaging specification bundled with Codex.

### Files

- `pet.json`: Configuration with the identifier `q-mimi` and sprite format version 2. The picker name remains **Q咪**.
- `spritesheet.webp`: Transparent 1536 × 2288 animation atlas, with 8 columns and 11 rows of 192 × 208 cells.
- `preview.gif`: Animated preview, not the installation atlas.

The atlas includes nine regular action groups and sixteen look directions. Keep the configuration and atlas together with their original filenames. A compatible host application is required.

### License and attribution

The Q Mimi atlas, preview, configuration and documentation are licensed under **CC BY-NC 4.0 (Attribution–NonCommercial)**. Noncommercial use, sharing and adaptation are permitted. When sharing publicly, retain attribution, source and license links, and indicate changes. For commercial permission, contact the author through [Issues](https://github.com/Aha-xiaoQ/q-mimi/issues).

Suggested credit: **Q Mimi · 在下_小Q (Aha_xiaoQ)**. Source: https://github.com/Aha-xiaoQ/q-mimi . License: CC BY-NC 4.0. Add a description of any changes you made.

See [LICENSE](LICENSE) for the full terms and [NOTICE.md](NOTICE.md) for scope. The character imagery was created with AI assistance. Permission covers only rights the licensor can grant; no claim is made that every generated element is copyright-protected in every jurisdiction. This is not an official OpenAI pet and is not endorsed by OpenAI.
