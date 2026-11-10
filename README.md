# 奶思去广告合集 · Shadowrocket 转换版

使用 [Script-Hub](https://github.com/Script-Hub-Org/Script-Hub) 的 `Rewrite-Parser.js`，将 [fmz200/wool_scripts 的 QX 去广告重写合集](https://github.com/fmz200/wool_scripts/blob/main/QuantumultX/rewrite/rewrite.snippet) 转成 Shadowrocket 模块。原规则作者：奶思及上游贡献者。本仓库不是上游官方发布。

## 订阅链接

```text
https://raw.githubusercontent.com/Akon5237/shadowrocket-adblock/main/Naisi-Shadowrocket.sgmodule
```

在 Shadowrocket 中打开「配置 → 模块 → +」，粘贴上面的链接，下载并启用。按需开启 HTTPS 解密，安装并信任自己生成的证书。重新连接后，完全退出并重开目标 App。避免叠加多个针对同一 App 的去广告合集。

## 版本与限制

- 转换日期：2026-11-10；原规则文件标注日期：2026-10-31。
- 这是静态转换快照，未设置自动同步上游。刷新模块只会获取本仓库最新提交。
- 模块仍引用上游远程脚本，因此不是完全离线文件。
- 结构检查：2,761 条分流规则、1,326 条 URL 重写、247 条脚本配置、1 条 Map Local，并包含 MITM 域名列表。
- 转换器提示 3 条原始规则缺少有效策略，保留为注释：`aoodoo.feng.com`、`push.feng.com`、`aoodoo.weiphone.com`。
- 未在 iPhone 上实测；格式转换不保证全部 App 版本有效，原规则及其潜在误拦仍然保留。出现正常功能异常时，停用本模块排查。

## 修改记录与许可

转换使用 Script-Hub 的 `qx-rewrite` → `shadowrocket-module` 目标。保留原作者与来源信息，调整模块显示名称，并将 `#!raw-url` 指向本仓库的已转换文件，避免更新时误下载原始 QX 格式。

本仓库中的转换规则遵循上游 GPL-3.0 许可，见 [LICENSE](LICENSE)。远程引用脚本的权利与许可归各自作者所有。
