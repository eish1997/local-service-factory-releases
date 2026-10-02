# 本地生活服务图片工厂

当前软件版本：[1.4.4](https://github.com/eish1997/local-service-factory-releases/releases/tag/v1.4.4)

[下载 Windows 安装包](https://github.com/eish1997/local-service-factory-releases/releases/download/v1.4.4/LocalServiceFactory-1.4.4-setup.exe)

此版修复一张不可重试或结果不确定的图片拦住整批继续的问题。保留成功图、跳过待处理项，其余沿用原任务和预算继续；详情可展开查看原因。升级后点击“继续原任务”，无需重建同范围批次或预算。

安装包 SHA256：`c9d29710b75dd1f2570f28a6878297fd9b1f90bc765c4cdad35a502e3dccc461`。软件启动时及每六小时检查更新，下载并验证后在无后台任务的退出时安装。已有任务、图片和冻结规则保留；沿用规则1790789310472053700，本次未发布新规则。

Ed25519更新签名及公开下载摘要已验证；暂无Windows Authenticode发布者证书。未进行付费生图验收。

## 此前分发说明（历史记录）

# 本地生活服务图片工厂

Windows独立版 **1.4.3**：[下载安装包](https://github.com/eish1997/local-service-factory-releases/releases/download/v1.4.3/LocalServiceFactory-1.4.3-setup.exe) · [版本说明](https://github.com/eish1997/local-service-factory-releases/releases/tag/v1.4.3)。包含独立Python和依赖。

修复新版排版遗漏图片主题：详情保留本批次作业主题，三拼每格显示对应来源主题，首图不增加详情主题。使用最新18个结构模板及4个兼容预设，主题字体、颜色、描边、效果和局部底板跟随模板；电话大字居中且无底色，副服务词保留完整。当前八项目的新共享批次使用新预设；原本无副服务词表的家电和开锁只保留任务主题及电话。商务KTV的视觉生产门禁继续执行。

规则检查优先GitHub官方raw签名索引，传输失败备用官方API；签名、摘要、文件白名单及软件兼容校验相同，不需要用户配置发布凭证或专用网络设置。启动与新批次组装共用离线兼容检查：旧内置规则与新程序不兼容时切换当前随包规则，保留旧规则和历史；兼容的签名规则继续使用。

旧批次、原图和当前成品不自动重做。主动后处理/预览使用新设计及原任务确认文字，追加历史；打包读取当前版本。Windows后处理暂存路径已缩短。保留同级「批次 / 提示词 / 后处理」页面、预览随机、导入导出和历史切换。本地后处理不调用生图API。

软件启动及每六小时检查更新，验证Ed25519签名和摘要后，在后台任务结束、正常退出时安装。[配套规则](https://github.com/eish1997/local-service-factory-rules/releases/tag/rules-1790789310472053700)最低软件 **1.4.3**。

安装包132408388字节，SHA256：`2eb21e46c361ecbbdadf808f73bdf6b02c1f0456251fe5bde2f68ca32efbfed3`。

公开下载、签名和摘要验证通过；包内独立Python八项目本地渲染、旧批次预览/应用、旧内置规则数据副本的离线启动、820px界面和默认网络消费者updated→current通过。NSIS脚本、依赖及更新器备份链路未变，复用1.3.1实际NSIS证据；本版未执行旧程序整机迁移、全新Windows虚拟机或付费生图。暂无Windows Authenticode证书。

客户电话、图片、任务、预览、API密钥及机器配置不进入分发仓库。
