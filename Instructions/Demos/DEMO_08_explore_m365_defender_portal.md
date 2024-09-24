<!---
---
演示：标题：“Microsoft Defender 门户”模块：“学习路径：介绍 Microsoft 安全解决方案的功能；模块 4：介绍 Microsoft 365 的威胁防护功能；单元 7：介绍 Microsoft Defender 门户”
---
--->

# 演示 ：Microsoft Defender 门户

此演示与下列 Learn 内容保持一致：

- 学习路径：描述 Microsoft 安全解决方案的功能
- 模块：描述 Microsoft 365 的威胁防护功能
- 单元：介绍 Microsoft Defender 门户

## 演示方案

在此演示中，你将通过登陆页面上显示的内容来展示 Microsoft Defender 门户。 你还将演练导航面板上的选项，这些选项提供对 Microsoft 扩展检测和响应 (XDR) 解决方案一部分功能的快速访问：Microsoft Defender for Endpoint 和 Microsoft Defender for Office 365（电子邮件和协作）。  最后，你还将了解 Microsoft 安全功能分数如何帮助组织改善其安全状况。

### 演示第 1 部分

浏览 Microsoft Defender 登陆页面。

1. 打开 Microsoft 365 安全性主页的浏览器选项卡。  如果之前关闭了浏览器，请打开 Microsoft Edge。 在地址栏中，输入 **https://admin.microsoft.com** 并使用授权实验室主机托管服务提供商 (ALH) 提供的 Microsoft 365 租户管理员凭据登录并访问 Microsoft 365 管理中心。 从 Microsoft 365 管理中心的左侧导航窗格，选择“**全部显示**”，然后选择“**安全性**”。  打开一个新的浏览器页，进入 Microsoft Defender 门户的欢迎页。  

1. Microsoft Defender 门户的主页显示安全团队所需的许多常见卡片。 卡片和数据的组成取决于用户的角色。 滚动页面，查看您作为全局管理员角色的默认卡片集。

1. 显示的卡片可根据您的偏好进行自定义。  选择 **+ 添加卡片**。 此时会打开一个窗口，显示可添加到主页的卡片。  你可能已显示所有卡片，在这种情况下，会显示提示“主页上已显示所有卡片。” 选择窗口右上角的 **X** 关闭窗口。

1. 选择任何卡片右上角的省略号将提供从登陆页面删除卡片的选项。  

1. 您还可以移动卡片。 将鼠标光标悬停在任意卡片的标题栏上，出现一个十字形光标时，选择该卡片并将其移动到所需位置。  

1. 某些卡片的底部有可选择的按钮。 某些卡片的标题用作该主题页面的链接。  例如，如果选择“Microsoft 安全功能分数卡”标题，则会将你带到“Microsoft 安全功能分数”页。  在本演示的后续部分中，你将详细了解 Microsoft 安全功能分数。

1. 保持浏览器窗口打开。

### 演示第 2 部分

在这部分演示中，你将了解 Defender 门户左侧导航面板中提供的一些选项。  通过 Microsoft Defender 门户，Microsoft 兑现了提供统一安全运营平台的承诺。 Microsoft Defender 门户在一个中心位置整合了防范、检测、调查和响应整个组织及其所有组件面临的威胁的功能。 它包括快速访问 Microsoft Defender XDR 解决方案（Microsoft Defender for Endpoint、Defender for Office for 365、Microsoft Defender for Cloud Apps 等）。  选择其中一些链接，探索这些选项。   要返回 Microsoft Defender 门户的主页，请选择左侧导航面板上的“**主页**”。

**备注：目的是演示导航面板上的一些选项，而不是对所有选项进行全面演示**。

1. **风险管理** - 列出的选项提供跨公司资产和工作负载的安全状况的统一视图。
    1. **攻击面** - 可以查看组织的攻击面地图。 攻击路径：根据跨资产和工作负载收集的数据自动生成攻击路径。 它模拟攻击方案，并识别攻击者可能利用的漏洞和弱点。
    1. **安全性见解** - Microsoft 安全风险管理中的风险见解将跨负载和资源的安全状况数据和见解持续聚合到单个管道中。
    1. **安全功能分数** - 安全功能分数提供分数明细、可提高组织分数的改进操作，以及该组织与其他类似组织的安全功能分数比较结果。
    1. **数据连接器** - 此处可连接数据源，以获得更丰富、更集中的风险管理体验。
1. **调查和响应** - 将在此处看到几个选项：
    1. **事件和警报** - 在此处查看来自不同 Defender XDR 解决方案（Defender for Identity、Defender for Cloud Apps、Defender for Office 365 和 Defender for Identity）和其他 Microsoft 解决方案（Microsoft Sentinel、Microsoft Defender for Cloud、Microsoft Entra 和 Microsoft Purview）的事件或单个警报。
    1. **搜寻** - 可在此处生成自定义检测规则，并搜寻环境中的特定威胁。
    1. **操作和提交** - 统一操作中心汇集了整个 Microsoft Defender for Endpoint 和 Microsoft Defender for Office 365 中的修正操作。 它在一个位置列出了针对设备、电子邮件和协作内容以及标识的待处理和已完成修正操作。 在拥有 Exchange Online 邮箱的 Microsoft 365 组织中，管理员可以使用 Microsoft Defender 门户中的“提交”页，将电子邮件、URL 和附件提交到 Microsoft 进行分析。
    1. **合作伙伴目录** - 合作伙伴目录列出了支持的技术合作伙伴和专业服务，可以帮助组织增强平台的检测、调查和威胁智能功能。
1. **威胁智能** - 在“威胁智能”选项卡中，用户可访问 Microsoft Defender 威胁智能和功能支持，包括威胁分析、Intel 配置文件、Intel 资源管理器和 Intel 项目。
1. **资产** - 在“资产”选项卡中，可以查看和管理组织的受保护和已发现资产（设备和标识）的清单。
1. **Microsoft Sentinel** - Defender 门户的 Microsoft Sentinel 部分中提供了一些 Microsoft Sentinel 功能。  这需要通过“设置”页面设置集成。
1. **标识** - 标识节点映射到与 Microsoft Defender for Identity 关联的功能。 仪表板提供有关标识威胁检测和响应 (ITDR) 的关键见解和实时数据。 “运行状况问题”页列出 Defender for Identity 部署和传感器的任何当前运行状况问题，提醒你在 Defender for Identity 部署中出现的任何问题。 “工具”页列出有助于管理 Microsoft Defender for Identity 环境的其他信息。
1. **终结点** - Microsoft Defender 门户左侧导航面板上的“终结点”节点映射到与 Microsoft Defender for Endpoints 关联的功能。
    1. 漏洞管理 - 管理设备上的漏洞和其他风险源。 从此处可以访问漏洞管理仪表板、建议、修正措施、弱点等。
    1. 合作伙伴和 API - 此处可以选择“已连接的应用程序”和 “API 资源管理器”。
    1. 配置管理 - 此处可查看设备配置管理仪表板。  还可以定义终结点策略并跟踪部署。
1. **电子邮件和协作** - 可在其中找到 Microsoft Defender for Office 365 功能，可用于跟踪和调查用户电子邮件面临的威胁、跟踪活动等。
1. **云应用** - 可在其中找到 Microsoft Defender for Cloud Apps 功能。 有关详细信息，请参阅“Microsoft Defender for Cloud Apps 演示”。
1. **SOC 优化** - SOC 优化提供了优化安全控制的方法，随着时间的推移，可从 Microsoft 安全服务中获得更多价值。
1. **报告** - 报告在 Microsoft Defender 门户中进行了统一。 管理员可从常规安全报告开始，然后深入到有关终结点、电子邮件和协作、云应用、基础结构和标识的特定分支报告。 此处的链接是根据工作负载配置动态生成的。
1. **学习中心** - 学习中心与 Microsoft Learn 相链接，可以在 Microsoft Learn 中访问培训课程、教程、文档和其他相关材料。
1. **系统** - 这包括用于配置权限、查看服务运行状况和常规设置的选项。
    1. 权限 - 可在此处为不同的 Microsoft Defender XDR 解决方案分配角色权限。
    1. 设置 - 此处为 Defender 门户、Defender XDR、属于 Microsoft Defender XDR 的解决方案和 Microsoft Sentinel 配置设置。  可以随时浏览此页面。
1. **自定义导航** - 此处可以选择显示或隐藏导航窗格中的项目。 其他管理员不会看到你的更改。

1. 左侧导航面板提供了指向 Microsoft 的扩展检测和响应（XDR 解决方案）一部分信息的链接以及对其的访问，其中包括事件和警报、搜寻、操作中心、威胁分析、安全分数等等。  它还提供了对 Microsoft Defender for Endpoint（在“终结点”下列出的链接）、Defender for Office 365（在“电子邮件和协作”下列出的链接）和 Microsoft Defender for Cloud Apps（云应用下的链接）等的快速访问。  选择其中一些链接，探索这些选项。   要返回 Microsoft Defender 门户的主页，请选择左侧导航面板上的“**主页**”。

### 演示第 3 部分

在这一部分的演示中，你将了解 Microsoft 安全功能分数如何帮助组织改善其安全状况。

1. 在左侧导航面板中，选择“**Microsoft 安全功能分数**”。

1. 这会打开“Microsoft 安全功能分数”页面，显示“概述”选项卡。Microsoft 安全功能分数是针对组织安全状况的一种衡量标准。 组织的安全功能分数以百分比形式显示，同时显示在可能的总分中已取得的分数，并按类别进行细分。 选择“你的安全功能分数”旁边的“**包含**”。 可以选择在你的分数视图中包含可达到分数、计划分数和当前许可证分数。

1. “概述”页还包括建议的操作、对比分数、历史记录和其他资源。

1. 选择页面顶部的“**改进操作**”。  注意表格中每个项目的可用信息。  

1. 从列表中选择前几项，然后查看可查看的信息。 请在打开的窗口中观察可用的状态选项。 选择要查看的“**实现**”选项卡，查看与实现相关的信息。 单击右上角的“**X**”以关闭此窗口。

1. 从页面顶部选择**历史记录**选项卡。  对于列出的每个活动，都有一句介绍上下文的简短说明。  在历史记录表中选择一个项。  在详细信息页面右上方的历史记录下，选择** X 事件**（其中 X 为数字）。  这会打开“操作历史记录”窗口，并提供详细信息。  选择页面底部的**关闭**，然后选择详细信息页面右上角的 **X** 返回历史记录页面。

1. 从页面顶部选择**指标和趋势**。  注意可用信息。  从页面右上角选择**日历图标**。  您可以将视图缩小到自定义日期范围。  通过选择**筛选图标**，可按标识、设备和/或应用筛选视图中的内容。  关闭窗口。

1. 在左侧导航面板中，选择“**主页**”，进入 Microsoft Defender 主页。

1. 如果打算继续进行下一个演示，请保持浏览器选项卡打开。

### 审阅

在此演示中，你通过演示登陆页面上显示的内容浏览了 Microsoft Defender 门户，也浏览了导航面板上的选项，这些选项可快速访问 Microsoft 的扩展检测和响应 (XDR) 解决方案、Microsoft Defender for Endpoints 和 Microsoft Defender for Office 365（电子邮件和协作）中的部分功能。  最后，您展示了 Microsoft Secure Score 如何帮助组织改善其安全态势。
