# 本地生活服务图片工厂

Windows 独立运行版本 **1.4.1**：[下载安装包](https://github.com/eish1997/local-service-factory-releases/releases/download/v1.4.1/LocalServiceFactory-1.4.1-setup.exe) · [版本说明](https://github.com/eish1997/local-service-factory-releases/releases/tag/v1.4.1)。内置 Python 和运行依赖，无需开发环境。

新增同级「批次 / 提示词 / 后处理」页面，包含 18 个结构模板和 4 个兼容预设。支持原图对照、模板内随机变化、单图导入导出和应用预览。汽车救援与货车救援的新共享批次自动轮换模板：电话大字居中，副词可独立配色、分组、加粗描边、局部底板及轻微旋转。全部操作在本地渲染，保留原照片；后处理不调用生图 API。

旧批次继续冻结规则，已有图片不自动重做。右键组或图片可重新后处理并追加历史，打包使用当前显示的版本。其他类别保持原后处理范围。

软件启动时检查更新，此后每六小时检查。校验 Ed25519 发布签名和文件摘要、备份原程序后，在正常退出且无后台任务时安装。[规则数据](https://github.com/eish1997/local-service-factory-rules)独立更新；本次配套规则最低需要软件 1.4.1。

安装包 SHA256：`f3ba07bcda1b1261e534d8441a0384010e1a8bc44f9912521c66f000cabc794b`。

本版完成公开下载和签名核验、独立引擎八业务组装、汽车/货车各五张隔离本地渲染，以及打包界面三个页面和窄窗口验证。运行时与安装更新链路没有修改，沿用 1.3.1 的真实 NSIS 安装与更新模块验收证据；本版没有重复进行实际旧版整机迁移、全新 Windows 虚拟机或付费生图测试。安装包无 Windows Authenticode 发布者证书。

用户 API 密钥、客户电话、图片、任务和个人配置保留在本地，不进入分发仓库。维护者明确要求发布后，通过 `python factory.py updates` 发布软件、`python factory.py rules` 发布规则；日常本地编辑不自动上传。
