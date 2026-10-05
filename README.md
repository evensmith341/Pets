# Pets

Codex 自定义动画宠物集合。目前包含 **蓝色大肥鱼**：戴着蓝色鲸鱼帽、围着蓝白围巾的软萌女孩。

## 动画预览

![蓝色大肥鱼的动画状态](previews/blue-whale-girl/all-states.gif)

包含 9 种标准动画状态：待机、等待、运行、向左跑、向右跑、跳跃、挥手、失败、审查。

![16 个注视方向](previews/blue-whale-girl/look-directions.gif)

另含 16 个注视方向。使用 Codex v2 精灵图格式，透明 WebP，尺寸为 1536 × 2288 像素。

## 安装

1. 从 [最新 Release](https://github.com/evensmith341/Pets/releases/latest) 下载 `blue-whale-girl.zip`。
2. 解压后，将整个 `blue-whale-girl` 文件夹放到 Codex 用户目录下的 `pets` 文件夹中。默认路径：
   - Windows：`%USERPROFILE%\.codex\pets\blue-whale-girl\`
   - macOS / Linux：`~/.codex/pets/blue-whale-girl/`
   - 如果设置了 `CODEX_HOME`，使用该目录下的 `pets/blue-whale-girl/`。
3. 确认 `pet.json` 与 `spritesheet.webp` 直接位于 `blue-whale-girl` 文件夹中，避免多套一层目录。
4. 打开 Codex 的 **设置 → Pets（宠物）**，点击刷新，再选择 **蓝色大肥鱼**。

如果已有同名宠物，请先备份原文件。请使用支持 v2 自定义宠物的 Codex 桌面版本。

也可以通过 Git 获取文件：

```sh
git clone https://github.com/evensmith341/Pets.git
```

然后按上述步骤，将仓库中的 `pets/blue-whale-girl` 文件夹复制到 Codex 用户目录。

## 下载校验

Release 同时提供 `SHA256SUMS.txt`，用于核对下载文件是否完整。

Windows PowerShell：

```powershell
Get-FileHash -Algorithm SHA256 .\blue-whale-girl.zip
```

macOS / Linux：

```sh
shasum -a 256 blue-whale-girl.zip
```

## 文件结构

```text
pets/blue-whale-girl/
├── pet.json             # 名称与精灵图配置
└── spritesheet.webp     # 最终动画精灵图
previews/blue-whale-girl/
├── all-states.gif        # 9 种状态预览
└── look-directions.gif   # 16 个注视方向预览
```

角色外观依据用户提供的参考图制作。仓库只收录完成的宠物文件和预览，不包含生成过程中的中间版本。
