📌 Shadowrocket 配置仓库

本仓库用于存放 Shadowrocket 使用的自定义 规则文件（configs） 与 模块文件（modules）。
你可以在 Shadowrocket 中通过 远程订阅链接 自动更新这些文件，方便日后维护。

⸻

📁 仓库结构

Shadowrocket
├─ configs/               # 规则文件（.list）
│  ├─ main.list           # 主规则（推荐作为主要订阅）
│  ├─ adblock.list        # 去广告规则（可选）
│  └─ custom.list         # 自定义规则
│
├─ modules/               # 模块文件（.sgmodule）
│  ├─ main.sgmodule       # 主模块：MITM、分流、策略等
│  └─ mitm.sgmodule       # 独立 MITM 模块（可按需使用）
│
└─ README.md


⸻

📥 Shadowrocket 订阅方式

你可以将 GitHub 中规则或模块文件的 RAW 链接 复制到 Shadowrocket 中作为远程订阅。

添加规则（.list）

Shadowrocket →
配置 → 右上角 + →
下载配置
输入 RAW 链接即可。

添加模块（.sgmodule）

Shadowrocket →
模块 → 右上角 + →
输入 RAW 链接即可安装。

⸻

✏️ 文件说明（建议用途）

configs/main.list

主规则文件，通常包含：
	•	国内直连
	•	国外代理
	•	常用服务分流
	•	自定义例外

configs/adblock.list

可选的去广告规则
（如不需要可删除）

configs/custom.list

你个人追加规则的保存位置。

⸻

modules/main.sgmodule

建议将你的：
	•	MITM 证书设置
	•	分流策略组
	•	DNS 配置
	•	节点组结构

都写在这个模块里。

modules/mitm.sgmodule

如果你想把 MITM 单独维护，可以放这里。

⸻

🧩 如何更新？

对任意文件修改 → GitHub 自动保存 RAW 链接不变 →
Shadowrocket 会自动同步更新（开启自动更新即可）。

⸻

🛠 推荐工作流程
	1.	在本地编辑 .list 或 .sgmodule 文件
	2.	提交更新到 GitHub
	3.	Shadowrocket 自动载入最新版本
	4.	如需添加新规则 → 只改 custom.list
	5.	大改策略 → 修改 main.sgmodule

⸻

📝 许可说明

本仓库仅作为个人 Shadowrocket 配置用途。
如需引用他人规则，请遵守原作者授权要求。