📌 Shadowrocket 配置仓库

本仓库用于存放 Shadowrocket 使用的自定义 规则文件（configs） 与 模块文件（modules）。
你可以在 Shadowrocket 中通过 远程订阅链接 自动更新这些文件，方便日后维护。

📥 Shadowrocket 订阅方式

你可以将 GitHub 中规则或模块文件的 RAW 链接 复制到 Shadowrocket 中作为远程订阅。

✏️  文件说明（建议用途）

configs/rules.list

规则文件，通常包含：

	•	国内直连
	•	国外代理
	•	常用服务分流
	•	自定义例外

modules/module.sgmodule

模块文件，通常包含：

	•	MITM 证书设置
	•	分流策略组
	•	DNS 配置
	•	节点组结构

🧩 如何更新？

对任意文件修改 → GitHub 自动保存 RAW 链接不变 →
Shadowrocket 会自动同步更新（开启自动更新即可）。

📝 许可说明

本仓库仅作为个人 Shadowrocket 配置用途。
如需引用他人规则，请遵守原作者授权要求。