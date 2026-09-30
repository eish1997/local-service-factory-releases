# 本地生活服务图片工厂

Windows 独立运行版本 **1.3.1** 已发布：[下载最新安装包](https://github.com/eish1997/local-service-factory-releases/releases/tag/v1.3.1)。首次安装请选择 1.3.1，内置 Python 和运行依赖，无需配置开发环境。1.3.1 修复更新前的 Electron ASAR 程序备份问题。

软件启动时检查更新，此后每六小时检查。校验发布签名和文件摘要、备份原程序后，在正常退出且无后台任务时安装。规则数据从 [规则仓库](https://github.com/eish1997/local-service-factory-rules) 独立更新，新批次使用最新规则，旧批次继续使用冻结规则。

已完成真实 GitHub 发布、NSIS 安装及独立运行验证；较低版本测试适配器驱动真实 electron-updater，验证签名、任务保护、备份和实际安装。全新 Windows 虚拟机未测试。当前安装包无 Windows Authenticode 发布者证书，应用独立使用 Ed25519 发布签名核验更新。

用户 API 密钥、客户电话、图片、任务和个人配置保留在本地，不进入分发仓库。维护者明确要求发布后，通过 `python factory.py updates` 发布软件、`python factory.py rules` 发布规则；日常本地编辑不自动上传。
