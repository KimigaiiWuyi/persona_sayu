# persona_sayu

<p align="center">
  <a href="https://github.com/KimigaiiWuyi/persona_sayu"><img src="./ICON.png" width="256" height="256" alt="persona_sayu"></a>
</p>
<h1 align="center">早柚人格整包 persona_sayu</h1>
<h4 align="center">🚧面向早柚核心(gsuid_core)的AI人格整包：角色卡 + 表情包 + 形象参考🚧</h4>

## 丨这是什么

[早柚核心(gsuid_core)](https://github.com/Genshin-bots/gsuid_core) AI 人格「早柚」的完整资源仓库，格式为 `gsuid-persona-bundle` v1.0。

包含人格的全部资产：

- **角色卡**：`persona.md`（核心定义、语言结构、社交行为、触发场景）
- **人格配置**：`config.json`（AI 行动模式 / 工具装配 / 说话强度等）、`persona.json`（称呼与失败台词）
- **形象资产**：`avatar.png`（头像）、`image.png`（立绘参考）、`appearance.txt`（AIGC 外观特征卡）
- **声线参考**：`audio.ogg`
- **表情包**：`packs/早柚/`（30 张 + `tags.json` 情绪/场景标签）

> **注意：框架目前不能直接加载 git 仓库作为人格**，需要打包成 zip 后通过 WebConsole 导入（见下）。

## 丨目录结构

```
.
├── ICON.png            # 仓库图标（仅 README 展示，不参与导入）
├── README.md
├── manifest.json       # 整包清单：format / version / persona_name（导入入口）
├── persona.md          # 角色卡正文（导入必需）
├── config.json         # 人格行为配置
├── persona.json        # 称呼与失败台词配置
├── avatar.png          # 头像 256×256
├── image.png           # 形象立绘参考
├── appearance.txt      # 外观特征卡（生图/认图用）
├── audio.ogg           # 声线参考
└── packs/
    └── 早柚/           # 表情包目录（图片 + tags.json）
```

## 丨相关

- 宿主框架：[gsuid_core](https://github.com/Genshin-bots/gsuid_core)
