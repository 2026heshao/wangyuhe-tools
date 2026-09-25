# WangYuHe 工具箱 · 宣传页

Windows 效率工具(CacheClear / FloatPulse / LaunchDeck / PyPacker)的官方宣传与下载页。

- 部署:GitHub Pages(自动,main 分支推送即上线) → https://2026heshao.github.io/wangyuhe-tools/
- 站点文件:`index.html`;安装包不经仓库分发,统一走 GitHub Releases 直链(源码与 Release 资产见 wangyuhe-tools-src)
- 备用公网单页(仅托管 HTML,不托管 exe):https://shippage.ai/p/yruzls

## 提交注意(实践经验)

- 大文件(如 26-31MB 的安装包)不要提交进仓库:`git push` 大文件容易失败,且会在 `.git` 里留下大量历史对象;移除文件后需 `git gc --prune=now` 才会真正释放
- 小文件可正常 `git push`,也可走 GitHub REST API 上传
