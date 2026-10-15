# snowready-support

雪备 SnowReady 的公开支持页与隐私政策。纯 HTML/CSS，无构建工具、前端框架、统计脚本或外部字体。

## 文件

- `index.html`：支持页，联系邮箱及常见问题。
- `privacy.html`：隐私政策，提供者按用户指定署名为 3KEC。
- `styles.css`：两页共用样式。
- `.nojekyll`：关闭 Jekyll 处理。

## GitHub Pages 发布

当前为待发布网页稿；准备文件不代表已在 GitHub 上线。公开前，运营者需确认政策中的资料处理与反馈保留/删除做法，并核实实际发布版本、主体信息和第三方服务安排。

1. 将上述四个网页文件放在仓库 `main` 分支根目录并推送。
2. 在仓库 **Settings → Pages → Build and deployment** 中选择 **Deploy from a branch**。
3. Branch 选择 **main**，Folder 选择 **/(root)**，保存。
4. 等待部署成功；若 HTTPS 设置可用，启用 **Enforce HTTPS**。
5. 用未登录的浏览器分别访问下面两个地址，确认正文、样式、邮件地址和内部链接正常。

预计地址（部署成功后方可使用）：

- App Store Support URL：`https://mm2m123.github.io/snowready-support/`
- App Store Privacy Policy URL：`https://mm2m123.github.io/snowready-support/privacy.html`

不要填写 GitHub 仓库地址、blob 地址或 `.git` 链接作为政策 URL。

GitHub 官方配置说明：<https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site>

## 本地预览

在仓库目录运行 `python3 -m http.server 8000 --bind 127.0.0.1`，访问 <http://127.0.0.1:8000/>。这是本机预览，不等于 GitHub Pages 已发布。

## 发布前复核

- 3KEC 为用户指定公开署名；若适用要求需要完整法定主体信息，在公开前补齐。
- 隐私政策未承诺“完全不收集数据”，未承诺第三方不保留 IP，也未把关闭同步描述为删除资料。
- QWeather 的 API 具体日志保留、地区处理及账号许可需运营者确认；官方开发者条款链接指向其隐私政策。
- 邮件保留/删除规则是拟采用的运营政策，公开后需要按其执行。
- App 内隐私入口、天气凭据整改、CloudKit Production 和商店隐私标签不包含在本仓库网页准备中。
