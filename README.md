# Find UI Motion Catalog

`find-ui-motion` Codex Skill 的独立网站清单和具体案例索引。目录与 Skill 分开发布，使网站失效、新网站加入或案例链接更新时，不必重新打包整个 Skill。

## 当前工作副本

- Catalog：`2026.08.8`
- 网站：18 个
- 具体案例：3100 个
- Schema：1

`manifest.json` 指向当前已发布版本 `2026.08.8`，并记录 Release 资源的 SHA-256。

## 文件

- `sites.json`：网站状态、入口、能力、技术栈、许可边界和健康检查日期。
- `examples.jsonl`：具体案例直达链接、动效分类、触发提示、证据策略和权利边界。
- `manifest.json`：最新发布版本、最低 Skill 版本、不可变 Release 资源地址和 SHA-256。

本仓库不保存来源网站的截图、视频、Lottie、Rive、代码片段或模型权重。

## 更新机制

Skill 从以下稳定地址检查最新 manifest：

```text
https://raw.githubusercontent.com/jjacy2024/find-ui-motion-catalog/main/manifest.json
```

发现更高版本时，Skill 只提醒用户。只有用户明确要求更新后，才会下载 Release 资源、验证 SHA-256、校验 schema 与案例引用并写入本地缓存；内置目录始终作为回退。

## 维护规则

- 单次超时或反爬响应不等于网站失效，应先人工复核。
- 具体案例必须使用稳定的公开直达链接；分类页只能作为明确标注的定位入口。
- 不因数量目标加入重复、弱相关、不可访问或无权展示的案例。
- 网站级许可不能代替案例级许可；复制、安装或下载前仍需重新检查当前条款。
- 每次发布必须生成新的版本号、不可变 Release 资源和匹配的 SHA-256。

对应 Skill：

https://github.com/jjacy2024/find-ui-motion-skill
