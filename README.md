# Q咪 · Q Mimi

[中文](#中文) · [English](#english)

## 中文

蓝黄配色的小猫宠物，戴着小小的黄金像素 Q。

![Q咪预览](preview.gif)

[看看 Q咪的动作](https://aha-xiaoq.github.io/projects/q-mimi/)

## 在 Codex 桌面端使用

这是一套自定义宠物素材，不是独立桌面程序，也不需要重新生成图片。需要支持 v2 自定义宠物的 Codex 桌面端；以下本地目录方式以 Windows 为例。

1. [下载素材包](https://aha-xiaoq.github.io/projects/q-mimi/q-mimi.zip)，解压。
2. 在资源管理器地址栏输入 `%USERPROFILE%\.codex\pets`。目录不存在时创建它，再在里面创建 `q-mimi` 文件夹。
3. 把解压得到的 `pet.json` 和 `spritesheet.webp` 放入该文件夹。已有同名宠物时先备份，不要直接覆盖自己的修改。
4. 打开 Codex 的宠物选择界面，刷新列表并选择 **Q咪**。支持此入口的版本可从 **Settings（设置）→ Pets（宠物）** 进入；菜单名称可能随版本调整。
5. 在输入框输入 `/pet`，或在命令菜单中选择 **Wake Pet**，唤醒宠物；再次输入 `/pet` 可隐藏它。

最终目录应是下面这样，不能多套一层解压文件夹：

```text
%USERPROFILE%\.codex\pets\q-mimi\
├── pet.json
└── spritesheet.webp
```

如果显式配置了 `CODEX_HOME`，改用该实际目录下的 `pets/q-mimi/`。macOS 默认对应 `~/.codex/pets/q-mimi/`；本项目未对所有系统和客户端版本逐一验证。

也可以把解压后的文件夹交给 Codex，并发送下面这段话：

> 请把这个文件夹中的 Q咪安装为本机自定义宠物。先确认实际 CODEX_HOME，将 pet.json 和 spritesheet.webp 放到 pets/q-mimi 下；如已有同名文件先备份。不要重新生成图片，不要直接修改全局状态文件。完成后告诉我如何在宠物列表选择并唤醒它。

### 没有显示，怎么办？

- **列表没有 Q咪：**检查目录层级和文件名，确保两个文件在一起；刷新宠物列表，必要时退出并重新打开应用。
- **选中了但桌面没出现：**用 `/pet` 或 Wake Pet 唤醒；选择与显示是两个步骤。
- **宠物静止：**检查系统的“减少动态效果”设置；实际动作由应用状态触发，不会像网页预览一样依次播放所有动作。
- **没有 Pets 或 `/pet` 入口：**先确认是支持宠物的桌面客户端及版本，不要把网页或 IDE 插件当作相同安装入口。本包使用 1536 × 2288 的 v2 图集，不适用于要求 1536 × 1872 图集的网页上传入口。

入口说明参考 [OpenAI 官方 Pets 文档](https://learn.chatgpt.com/docs/pets)。原 Codex 文档链接现重定向到该页面，页面使用 ChatGPT 桌面端名称；请以自己安装版本的实际界面为准。本地文件安装方式依据 Codex 随附的宠物打包规范。

## 素材

- `pet.json`：宠物配置，标识为 `q-mimi`，图集格式版本为 2。
- `spritesheet.webp`：透明动画图集，1536 × 2288 像素；8 列、11 行，每格 192 × 208 像素。
- `preview.gif`：预览动图，不作为宠物图集使用。

图集包含 9 组常规动作和 16 个观察方向。使用时保留配置与图集的文件名，并将两者放在同一目录。需要宿主支持此自定义宠物格式；这不是独立运行的桌面程序。

## 许可证与署名

Q咪图集、预览、配置及本说明采用 **CC BY-NC 4.0（署名—非商业性使用）**。允许非商业使用、分享和修改；公开分享时请保留署名、来源及许可证链接，并说明是否修改。商业用途请先通过 [Issues](https://github.com/Aha-xiaoQ/q-mimi/issues) 联系授权。

署名示例：**Q咪 · 在下_小Q（Aha_xiaoQ）**，来源：https://github.com/Aha-xiaoQ/q-mimi ，许可：CC BY-NC 4.0。若有修改，请补充修改说明。

完整条款见 [LICENSE](LICENSE)，适用范围见 [NOTICE.md](NOTICE.md)。角色图像由 AI 辅助生成；授权仅涉及授权方有权授予的权利，不保证所有生成元素在所有地区均受著作权保护。本项目不是 OpenAI 官方宠物，也不代表 OpenAI 背书。

## English

Q Mimi is a blue-and-yellow cat pet wearing a small golden pixel Q.

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
