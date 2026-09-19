# Q咪 · Q Mimi

**简体中文** · [English](README.en.md)


蓝黄配色的小猫宠物，戴着小小的黄金像素 Q。

![Q咪预览](preview.gif)

[看看 Q咪的动作](https://aha-xiaoq.github.io/projects/q-mimi/)

## 安装并使用

1. 打开 [Q咪网页](https://aha-xiaoq.github.io/projects/q-mimi/)，点击 **安装到 Codex**。
2. 允许浏览器打开 Codex，在客户端点击 **安装**。
3. 点击 **使用此宠物**。如果宠物没有显示，在 Codex 输入 `/pet`。

也可以 [下载压缩包](https://aha-xiaoq.github.io/projects/q-mimi/q-mimi.zip)，解压后双击 **START.html**，使用同一个安装按钮。此导入方式不用输入命令，也不用自己找目录。

需要联网，并已安装支持宠物导入的 Codex 桌面端。没有打开时，先更新客户端后重试。安装和选择宠物需要在客户端确认。

<details>
<summary>备用安装方法与常见问题</summary>

如果客户端不支持导入按钮，可以把解压后的文件夹交给 Codex，并发送：

> 请将这个文件夹里的 Q咪安装为本机自定义宠物。确认实际 CODEX_HOME，把 pet.json 和 spritesheet.webp 放到 pets/q-mimi 下；已有同名文件先备份。保留原图，完成后告诉我如何在宠物列表选择它，并用 /pet 显示。

手动安装：Windows 将 `pet.json` 和 `spritesheet.webp` 放在 `%USERPROFILE%\.codex\pets\q-mimi\`；macOS 对应 `~/.codex/pets/q-mimi/`。若配置过 `CODEX_HOME`，使用该目录下的 `pets/q-mimi/`。覆盖已有文件前先备份。然后在 **设置 → 宠物** 中刷新并选择 **Q咪**，输入 `/pet` 或选择 **Show pet** 显示；菜单名称可能随版本变化。

列表中找不到时，检查两个文件是否直接位于 `q-mimi` 文件夹，再刷新列表。宠物不动时，检查系统的“减少动态效果”设置。本包是桌面端 v2 图集，不适用于要求 1536 × 1872 图片的网页上传入口。

桌面端操作可参考 [官方 Pets 说明](https://learn.chatgpt.com/docs/pets)。导入支持情况取决于客户端版本。

</details>

## 素材

- `pet.json`：宠物配置，标识为 `q-mimi`，图集格式版本为 2。
- `spritesheet.webp`：透明动画图集，1536 × 2288 像素；8 列、11 行，每格 192 × 208 像素。
- `preview.gif`：预览动图，不作为宠物图集使用。

图集包含 9 组常规动作和 16 个观察方向。使用时保留配置与图集的文件名，并将两者放在同一目录。需要宿主支持此自定义宠物格式；这不是独立运行的桌面程序。

## 许可证与署名

Q咪图集、预览、配置及本说明采用 **CC BY-NC 4.0（署名—非商业性使用）**。允许非商业使用、分享和修改；公开分享时请保留署名、来源及许可证链接，并说明是否修改。商业用途请先通过 [Issues](https://github.com/Aha-xiaoQ/q-mimi/issues) 联系授权。

署名示例：**Q咪 · 在下_小Q（Aha_xiaoQ）**，来源：https://github.com/Aha-xiaoQ/q-mimi ，许可：CC BY-NC 4.0。若有修改，请补充修改说明。

完整条款见 [LICENSE](LICENSE)，适用范围见 [NOTICE.md](NOTICE.md)。角色图像由 AI 辅助生成；授权仅涉及授权方有权授予的权利，不保证所有生成元素在所有地区均受著作权保护。本项目不是 OpenAI 官方宠物，也不代表 OpenAI 背书。
