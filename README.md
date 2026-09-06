# Q咪 · Q Mimi

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

署名示例：**Q咪 · 在下_小Q（Aha-xiaoQ）**，来源：https://github.com/Aha-xiaoQ/q-mimi ，许可：CC BY-NC 4.0。若有修改，请补充修改说明。

完整条款见 [LICENSE](LICENSE)，适用范围见 [NOTICE.md](NOTICE.md)。角色图像由 AI 辅助生成；授权仅涉及授权方有权授予的权利，不保证所有生成元素在所有地区均受著作权保护。本项目不是 OpenAI 官方宠物，也不代表 OpenAI 背书。
