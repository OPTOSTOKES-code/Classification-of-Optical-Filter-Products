# 项目代理文档（V3 / GitHub 公开库版）

## 1. 目录定位

- `V3` 是面向 GitHub 公开库和 GitHub Pages 的轻量资料站。
- 目标是用少量精选内容展示 OPTOStokes 的产品方向，引导客户访问 `https://www.optofilters.com/`。
- `V3` 不替代主站，不复制 `split-catalog-v1` 的完整目录和交互功能。

## 2. 合规边界

- 不发布私有客户资料、报价单、账号、密码、内部配置、服务器信息或未公开数据。
- 不使用自动跳转、隐藏链接、短链、钓鱼式表单或可疑脚本。
- 不把 GitHub 仓库做成纯广告跳转页；每个页面必须有独立资料价值。
- 不伪装成 GitHub、Google、第三方认证机构或独立评测站。
- 不臆造型号详情页 URL；只链接已确认存在的官网页面。

## 3. 内容策略

- 只展示精选型号和选择逻辑，不展示完整产品数据库。
- 页面应优先提供应用路径、波段方向、代表型号和下一步选型问题，让客户产生继续浏览官网的理由。
- 英文内容采用克制的 B2B 工程语气。
- 链接数量保持克制，优先指向：
  - `https://www.optofilters.com/optical-filters-catalog.html`
  - `https://www.optofilters.com/optical-filters/bandpass-filters.html`
  - `https://www.optofilters.com/optical-filters/ir-optical-filters.html`
  - `https://www.optofilters.com/optical-filters/pcr-optical-filters.html`
  - `https://www.optofilters.com/single/contact-us.html`

## 4. 技术约束

- 输出为纯静态文件，可直接用于 GitHub Pages。
- 不引入构建步骤。
- 不使用第三方 CDN、远程字体或外部 JS。
- 所有文件使用 UTF-8 without BOM。
- `index.html`、`assets/styles.css`、`data/featured-products.json` 是核心发布文件。

## 5. 发布前检查

1. 打开 `index.html`，确认本地显示正常。
2. 检查所有官网链接可访问。
3. 检查无 `<script>`、自动跳转、隐藏 iframe、收集表单。
4. 检查编码无 BOM、无 `�`、无已知 mojibake。
5. 如果发布 GitHub Pages，建议启用仓库 Settings -> Pages -> Deploy from branch。
