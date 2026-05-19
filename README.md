# nutwise-legal

**松鼠储财**（英文品牌名 **Nutwise**）的 App Store 法务与支持静态页。本仓库仅托管 HTML，不包含主应用源码。

## 网站首页（索引）

GitHub Pages 入口与下方「页面导航」一致：

| 说明 | 打开 |
|------|------|
| **网站首页**（`index.html`） | https://hans-sunzihan.github.io/nutwise-legal/ |
| 隐私政策 | https://hans-sunzihan.github.io/nutwise-legal/privacy.html |
| 用户协议 | https://hans-sunzihan.github.io/nutwise-legal/terms.html |

首页提供两张卡片，分别进入隐私政策与用户协议；子页顶部面包屑可返回首页。

## 品牌说明

| 名称 | 角色 |
|------|------|
| 松鼠储财 | 中文产品名（法务页与 App Store 主名称） |
| Nutwise | 英文品牌名（替代原 sCost 对外英文称呼） |
| nutwise-legal | 本仓库名（仅表示法务静态资源） |

主工程仓库：[Hans-Sunzihan/Nutwise](https://github.com/Hans-Sunzihan/Nutwise)。命名关系见主仓库 README「品牌与命名」一节。

## 关于 nutwise.ai

[nutwise.ai](https://nutwise.ai) 为**规划中的未来官网**，当前未申请域名。**提审与 App 构建请使用上表 GitHub Pages 地址**，勿填写 nutwise.ai，直至 DNS 与 Pages 自定义域名均已配置完成。

## 仓库文件与页面对应

| 文件 | 线上路径 |
|------|----------|
| `index.html` | `/` |
| `privacy.html` | `/privacy.html` |
| `terms.html` | `/terms.html` |

## 更新流程

由主仓库 `Nutwise` 同步 HTML 后推送：

```bash
git clone https://github.com/Hans-Sunzihan/nutwise-legal.git
/path/to/Nutwise/scripts/sync-legal-pages.sh ./nutwise-legal
cp /path/to/Nutwise/docs/legal/nutwise-legal.README.md ./nutwise-legal/README.md
cd nutwise-legal && git add -A && git commit -m "chore: 同步法务页" && git push
```

## App Store 填写参考

- 隐私政策 URL：`https://hans-sunzihan.github.io/nutwise-legal/privacy.html`
- 用户协议 URL：`https://hans-sunzihan.github.io/nutwise-legal/terms.html`
- 支持 URL：`https://hans-sunzihan.github.io/nutwise-legal/`

更完整字段见主仓库 `docs/app_store_metadata.md`。
