# 微信客户分析 Agent

一款面向 Apple Silicon Mac 的微信聊天分析工具。连接并同步微信后，你可以用自然语言筛选客户、了解人物与关系、梳理话题和待办，并在结果中查看对应的聊天证据。

## 下载安装

[下载最新版 v0.1.5-test（检查更新通道修复）](https://github.com/showyell-del/wechat-sales-agent-releases/releases/download/v0.1.5-test/WeChatSalesAgent-v0.1.5-test.dmg) · [查看发布页面](https://github.com/showyell-del/wechat-sales-agent-releases/releases/tag/v0.1.5-test)

历史版本：[v0.1.4-test](https://github.com/showyell-del/wechat-sales-agent-releases/releases/tag/v0.1.4-test)、[v0.1.3-test](https://github.com/showyell-del/wechat-sales-agent-releases/releases/tag/v0.1.3-test)、[v0.1.2-test](https://github.com/showyell-del/wechat-sales-agent-releases/releases/tag/v0.1.2-test)。

v0.1.5-test 修复了应用内「检查更新」：发布通道改为固定名称安装包 + 版本清单，客户端识别测试通道标签，清单改由 api.github.com 提供（国内网络下下载域名常不可达），并加入直连/代理交替重试。v0.1.4-test 已修复授权误报：把断网等瞬时失败与真正的到期区分开，加入 30 秒超时与重试、72 小时离线宽限、10 分钟轮询。当前版本为 ad-hoc 签名、未经 Apple 公证，且尚未在另一台 Mac 完成全新安装验证，仅供内测，详见发布页面。

## 功能

- **自然语言分析**：输入问题，查找相关对话，支持连续追问。
- **客户经营**：筛选客户、分析机会与风险、整理跟进建议。
- **人物与关系**：基于聊天记录归纳人物特点和互动情况。
- **话题与时间线**：整理群聊话题、事件和承诺事项。
- **证据追溯**：查看支持结论的原始消息及上下文。
- **保存与导出**：保存分析，按需导出报告。
- **检查更新**：在应用菜单中检查新版本并前往发布页下载。

## 使用条件

- Apple Silicon Mac，已安装并登录微信。
- 需要有效激活码和 DeepSeek API Key；模型调用可能产生费用。
- 当前测试版需要关闭 macOS 系统完整性保护（SIP），这会降低系统安全保护。
- 当前安装包采用临时签名，未经 Apple 公证；系统可能阻止直接打开。

## 使用步骤

1. 下载并打开安装映像，将应用拖入“应用程序”。
2. 启动应用，根据界面提示完成激活和环境配置。
3. 连接微信并同步聊天记录，配置 DeepSeek API Key。
4. 在智能分析中输入问题，核对结论及其证据，按需保存或导出。

聊天数据和分析状态保存在本机；主动发起分析时，相关候选聊天内容会发送至 DeepSeek。分析结果仅基于已同步的可用记录，请结合原始证据判断。

此版本为测试版。
