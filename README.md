<div align="right">
  <a title="简体中文" href="README.md"><img src="https://img.shields.io/badge/-%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-545759?style=for-the-badge" alt="简体中文"></a>
  <a title="English" href="README_EN.md"><img src="https://img.shields.io/badge/-English-A31F34?style=for-the-badge" alt="English" /></a>
</div>

# ✔[UptimeFlare](https://github.com/allovend/UptimeFlare)

一个更先进、无服务器且免费的正常运行时间监控和状态页面解决方案，由Cloudflare Workers提供支持，具有用户友好的界面。

🎉 **[更新 2026/01/03]** 我刚刚将UptimeFlare从KV迁移到D1数据库。我还将TerraForm CloudFlare提供程序更新为V5，并改进了部署流程。优化了数据结构，解决了长期存在的性能问题。

新用户可以直接部署，而现有用户只需执行简单的自动迁移过程(下面的升级文档)!如果您在部署时遇到任何问题，请随时打开问题。

## ⭐特点

  - 开源、易于部署(10分钟内完成，无需本地工具)且免费
  - 监控能力
  - 每隔1分钟进行多达50次检查
  - 来自Over的特定地理位置检查 [310 cities](https://www.cloudflare.com/network/) 世界范围
  - 支持HTTP/https/tcp端口监控
  - 长达90天的正常运行时间历史记录和正常运行时间百分比跟踪
  - 可定制的HTTP(s)请求方法、头和正文
  - 自定义状态码和关键字检查HTTP(s)
  - 停机通知支持 [100+ notification channels](https://github.com/caronc/apprise/wiki)
  - 可自定义Webhook
  - 多语言支持(英文/中文)
  - “状态”页
  - 所有类型监控器的交互式ping(响应时间)图表
  - “计划维护警报和突发事件历史记录”页
  - 适应系统主题的响应式用户界面
  - “可自定义状态”页
  - 使用您自己的域名和CNAME
  - 可选密码身份验证(“私人状态”页)
  - 用于获取实时状态数据的JSON API

## 👀演示

我的状态页面(在线演示): https://uptimeflare.pages.dev/

一些截图:

![桌面，轻主题](docs/desktop.png)

## ⚡快速入门 / 📄文件

请参考 [维基](https://github.com/allovend/UptimeFlare/wiki)

## 🚀升级现有部署

使用立即获取最新功能[升级过程简单](https://github.com/allovend/UptimeFlare/wiki/Synchronize-updates-from-upstream)

## ⚙️面向开发人员的文档

若要进一步提供新功能或定制部署，请参阅[此处](https://github.com/allovend/UptimeFlare/wiki/How-to-develop).

## 新功能(全部)

- [x] 指定监控器的区域
- [x] TCP `已开通` 承诺
- [x] 使用Apprise支持各种通知渠道
- [x] ~~电报示例~~
- [x] ~~[树皮](https://bark.day.app) 示例~~
- [x] ~~通过Cloudflare电子邮件工作人员发送电子邮件通知~~
- [x] 通过提供简单的示例来改进文档
- [x] 通知宽限期
- [ ] SSL证书检查
- [x] ~~自主机Dockerfile~~
- [x] 事件历史记录
- [x] 改进 `检查位置工作者路线` 并有可能修复 `代理失败`
- [x] 群组
- [x] 删除旧的事件
- [x] ~~已知问题~~: `获取` 不支持非标准端口（在CF更新后已解决）
- [x] 兼容性日期更新
- [x] 定期维护
- [x] 为开发者添加文档
- [x] 迁移到 Terraform Cloudflare 提供商版本 5.x
- [x] Cloudflare D1 数据库
- [x] 定期维护（通过 IIFE）
- [x] 更简洁的配置示例
- [x] 即将进行的维护
- [x] 通用 Webhook 升级
- [x] 国际化...?（可能）
- [ ] 通过代理的 ICMP？
- [x] 添加默认 UA
- [x] 可自定义的页脚
- [x] 新的头部 logo
- [x] 改进 CPU 时间使用
- [x] 本地部署（文档 WIP）
