# BalancePet 主题仓库

BalancePet 的**主题**都在这里：一个主题一个目录，打包后挂在本仓库的 Releases 上，`catalog.json` 是它们的目录。

| 主题 | 材质 | 说明 |
| --- | --- | --- |
| [BalancePet 云母](themes/balancepet-mica) | 云母 / 云母 Alt / 实色 | 系统云母底层、Fluent 控件与青绿色强调色 |
| [BalancePet 亚克力](themes/balancepet-acrylic) | 亚克力 / 实色 | 为亚克力设计的通透配色：低不透明度表面、明亮描边、更强的分层阴影 |

## 安装

1. 从 [Releases](https://github.com/GoldenMoon-cell/BalancePet-Themes/releases) 下载 `balancepet.theme.<名字>-<版本>.zip`
2. 在「设置 → 外观」**导入主题 ZIP**，或把 ZIP 拖到「设置 → 扩展」页面
3. 在「设置 → 外观」的**当前主题**里选中它

需要 BalancePet **1.0.0** 或更高版本。材质由宿主调用系统接口实现，主题只声明它支持哪几种。

## 自己做一个

复制 `themes/balancepet-mica` 当起点，改 `manifest.json` 的 `id` 与名称、改 `theme.json` 的配色，然后跑 `tools/package-theme-extension.ps1`。
颜色是 `#RRGGBB` 或 `#AARRGGBB`；`backdrops` 声明支持哪些材质（`mica`／`mica-alt`／`acrylic`／`solid`），宿主只给用户列出这些，`solid` 始终可用作回退。

## 许可证

MIT