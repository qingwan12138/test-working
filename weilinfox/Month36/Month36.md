# Month 36 工作报告 26/06/01-26/06/29

+ 更新 Ruyi 0.49.0 测试报告的 IDE 和 VSCode 部分
    + [!95 Update 0.49.0 IDE test status](https://gitee.com/yunxiangluo/ruyisdk-test/pulls/95)
    + [!96 Update 0.49.0 IDE test status](https://gitee.com/yunxiangluo/ruyisdk-test/pulls/96)
+ 测试 Ruyi 0.50.0-beta.20260623 提交测试报告
    + [!97 Add 0.50.0-beta test reports](https://gitee.com/yunxiangluo/ruyisdk-test/pulls/97)
+ ruyi 仓库提交 1 个 issue
    + [Ruyi 0.50.0-beta.20260616: No module named '\_bz2' #473](https://github.com/ruyisdk/ruyi/issues/473)
+ ruyisdk-website 仓库审核 2 个 pr
    + [docs: fix code block rendering in VS Code case1 #495](https://github.com/ruyisdk/ruyisdk-website/pull/495)
    + 修复移动端边栏出现时顶栏和边栏动画透明度不一致的问题 [Navbar and sidebar transparency fix #512](https://github.com/ruyisdk/ruyisdk-website/pull/512)
+ ruyisdk-website 仓库提交 26 个 pr
    + 调整开发板板块的移动端现实 [pages(index): better DevBoards components Mobile layout #497](https://github.com/ruyisdk/ruyisdk-website/pull/497)
    + 将新的开发板板块发布到首页 [pages(index): add DevBoards component to index #498](https://github.com/ruyisdk/ruyisdk-website/pull/498)
    + 更新 vf2 lite 图片 [pages(index): swap vf2 img with vf2lite #500](https://github.com/ruyisdk/ruyisdk-website/pull/500)
    + 优化开发板板块的链接跳转 [pages(index): better mobile title and link jump #501](https://github.com/ruyisdk/ruyisdk-website/pull/501)
    + 优化 ci 调用 github api 的逻辑，选取合适的等待时间并减少调用次数 [ci: wait longer on github api data update #502](https://github.com/ruyisdk/ruyisdk-website/pull/502)
    + 让官网在 api.ruyisdk.cn 失效时保持正常工作 [misc: fix loading failure when api.ruyisdk.cn failed #503](https://github.com/ruyisdk/ruyisdk-website/pull/503)
    + 固定顶栏，增加快速回到顶部按钮 [pages: add back to top button](https://github.com/ruyisdk/ruyisdk-website/commit/3af287b04ec0987b0fae8e0401557a1b5299d74b)
    + 完善新下载页面在 /downloads [pages(downloads): merge some download inform text #513](https://github.com/ruyisdk/ruyisdk-website/pull/513)
    + [pages(downloads): refactor into components #515](https://github.com/ruyisdk/ruyisdk-website/pull/515)
    + [pages(downloads): modify page layout #516](https://github.com/ruyisdk/ruyisdk-website/pull/516)
    + 整理项目结构，去掉多余的中文翻译 [i18n: remove i18n/zh-Hans #517](https://github.com/ruyisdk/ruyisdk-website/pull/517)
    + [pages(index): fix index font broken caused by #507 #518](https://github.com/ruyisdk/ruyisdk-website/pull/518)
    + 整理项目结构，修复部分页面视觉宽度的微小差异 [pages(about,news,News/{Blogs,Events}): modify page layout #519](https://github.com/ruyisdk/ruyisdk-website/pull/519)
    + 修复文档页面列表显示问题 [pages(docs): fix li, ol and ul #520](https://github.com/ruyisdk/ruyisdk-website/pull/520)
    + 新下载页面 IDE 下载链接切换到 api.ruyisdk.cn 的新 endpoint [api.ruyisdk.cn endpoint form eclipse and vscode plugin release info #521](https://github.com/ruyisdk/ruyisdk-website/pull/521)
    + [pages(downloads): better design and layout #523](https://github.com/ruyisdk/ruyisdk-website/pull/523)
    + 完善新下载感谢页面和引导用户阅读文档 [pages(thanks): better download thanks page #525](https://github.com/ruyisdk/ruyisdk-website/pull/525)
    + 去除文档页面代码块的黄色底色，统一所有代码块的视觉风格 [pages(docs): remove yellow background from CodeBlock #526](https://github.com/ruyisdk/ruyisdk-website/pull/526)
    + [pages(thands): fix command line copy #527](https://github.com/ruyisdk/ruyisdk-website/pull/527)
    + 修复新下载页面部分代码块的行复制按钮 [docs(CodeBlock): fix code copy on downloads page #528](https://github.com/ruyisdk/ruyisdk-website/pull/528)
    + 修复新下载页面部分 markdown 维护的内容的代码块语法兼容问题 [pages(downloads): fix markdown codeblock support #529](https://github.com/ruyisdk/ruyisdk-website/pull/529)
    + 修复文档页面架构切换时代码块出现横向滚动条的问题 [pages(docs): fix arch selecte scroll bar #530](https://github.com/ruyisdk/ruyisdk-website/pull/530)
    + 调整下载感谢页面渲染时序，在获取到 uri 参数后再渲染 card [pages(thanks): do not show card before we can get params #531](https://github.com/ruyisdk/ruyisdk-website/pull/531)
    + 新的 报告问题 页面 [pages: new page /issue #534](https://github.com/ruyisdk/ruyisdk-website/pull/534)
    + news 页面翻页增加 url 翻页 [pages(news): add page url param #535](https://github.com/ruyisdk/ruyisdk-website/pull/535)
    + issue 页面添加 meta 英文翻译 [pages(issue): add meta translation for English page #536](https://github.com/ruyisdk/ruyisdk-website/pull/536)
+ ruyisdk-website 仓库提交 1 个 issue
    + [下载页面设计 #522](https://github.com/ruyisdk/ruyisdk-website/issues/522)
+ packages-index 仓库提交 3 个 pr
    + Bianbu for k1 更新的最新 v2.3.3 [board-image/bianbu-{desktop,desktop-lite,minimal}-spacemit-k1{,-sd}: new version v2.3.3 #196](https://github.com/ruyisdk/packages-index/pull/196)
    + 增加 Spacemit Muse Pi Pro 支持和 Bianbu UEFI 镜像支持 [New device spacemit muse pi pro and uefi support for spacemit-k1-v1 strategy #198](https://github.com/ruyisdk/packages-index/pull/198)
    + Bianbu for K3 的支持 draft， 由实习生在 Spacemit K3 Pico-ITX 测试中 [New device Spacemit K3 Pico-ITX #199](https://github.com/ruyisdk/packages-index/pull/199)
+ packages-index 仓库提交 2 个 issue
    + 关联 #198 [Spacemit K1 UEFI image support #197](https://github.com/ruyisdk/packages-index/issues/197)
    + 关联 #199 [New device Spacemit K3 Pico-ITX #199](https://github.com/ruyisdk/packages-index/issues/200)
+ ruyi-backend 仓库提交 1 个 issue
    + [添加 IDE 最新版本查询 endpoint #98](https://github.com/ruyisdk/ruyi-backend/issues/98)

