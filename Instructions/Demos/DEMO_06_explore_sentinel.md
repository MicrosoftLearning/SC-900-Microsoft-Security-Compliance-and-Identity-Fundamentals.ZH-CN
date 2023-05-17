---
demo:
    title: '演示：Microsoft Sentinel'    
    module: '模块 3：描述 Microsoft Sentinel 的安全功能'
---


# <a name="demo-microsoft-sentinel"></a>演示：Microsoft Sentinel

此演示与下列 Learn 内容保持一致：

- 学习路径：描述 Microsoft 安全解决方案的功能
- 模块：描述 Microsoft Sentinel 的安全功能
- 单元：描述 Microsoft Sentinel 如何提供集成威胁管理

## <a name="demo-scenario"></a>演示方案

在本演示中，你将演练创建 Microsoft Sentinel 实例的过程。  你还将设置权限，以确保可访问将为支持 Microsoft Sentinel 而部署的资源。  完成此基本设置后，你将逐步完成将 Microsoft Sentinel 连接到数据源并选择工作簿以监视和可视化数据的步骤。  最后，你将显示可用的一些其他选项，包括在发生任何可疑情况时获得通知的内置分析、自动化功能等等。

### <a name="pre-demo-setup--create-a-microsoft-sentinel-instance"></a>预演示设置：创建 Microsoft Sentinel 实例

1. 打开浏览器选项卡“主页 - Microsoft Azure”。  如果之前关闭了该选项卡，请打开浏览器页面，在地址栏中输入 portal.azure.com，然后重新登录。

1. 在页面顶部显示 Microsoft Azure 旁边蓝色栏的搜索框中，输入“Microsoft Sentinel”，然后在搜索结果中选择“Microsoft Sentinel”。 

1. 在“Microsoft Sentinel”页中，选择“创建 Microsoft Sentinel”。

1. 在“将 Microsoft Sentinel 添加到工作区”页中，选择“创建新工作区”。

1. 在“创建 Log Analytics”工作区的“基本”选项卡中，输入以下内容：
    1. 订阅：保留默认值。
    1. 资源组：选择“新建”，输入名称“SC900-Sentinel-RG”，然后选择“确定”  。
    1. 名称：SC900-LogAnalytics-workspace。
    1. 区域：美国东部（可能会根据你的位置选择不同的默认区域）
    1. 选择“查看 + 创建”（不会配置任何标记）。
    1. 验证输入的信息，然后选择“创建”。
    1. 可能需要一两分钟才会列出新工作区，如果仍未看到它，请选择“刷新”，然后选择“添加” 。

1. 添加新工作区后，将显示“Microsoft Sentinel | 资讯与指南”页面，指示已激活 Microsoft Sentinel 免费试用版。  选择“确定”。  请注意，“入门”页面列出了三个步骤。

1. 请将此页面保持打开状态，因为在下一个任务中将用到它。

### <a name="demo-part-2"></a>演示第 2 部分

创建 Microsoft Sentinel 实例后，你需要确保具有对为支持 Microsoft Sentinel 而部署的资源的必要访问权限。  

1. 在页面顶部显示 Microsoft Azure 旁边蓝色栏的搜索框中，输入“资源组”，然后在搜索结果中选择“资源组” 。 在资源组级别分配角色可确保该角色会应用到为支持 Microsoft Sentinel 而部署的所有资源。

1. 从“资源组”页中选择使用 Microsoft Sentinel 创建的资源组“SC900-Sentinel-RG”。

1. 在 SC900-Sentinel-RG 页面中，从左侧导航面板中选择“访问控制(IAM)”。

1. 从“访问控制”页面中选择“查看我的访问权限”。  作为 MOD 管理员，当前角色是服务管理员。  这将授予你所需的权限，但出于演示目的，你可能需要显示 Sentinel 特定角色。  选择窗口右上角的“X”关闭 MOD 管理员分配窗口。

    1. 从“访问控制”页面中选择“+添加”，然后选择“添加角色分配” 。

    1. “添加角色分配”窗口随即打开。  在搜索框中，输入“Microsoft Sentinel”以查看与 Microsoft Sentinel 相关的 4 个角色。
    1. 从列出的任一角色中，选择“视图”以查看该角色的详细信息。  最佳做法是分配角色所需的最低特权。  

    1. 选择窗口右上角的“X”关闭窗口。

1. 在访问控制页面中，选择窗口右上角的“X”关闭此窗口。

### <a name="demo-part-3"></a>演示第 3 部分

在演示的这一部分中，你将展示连接到数据源的步骤。  具体而言，你将连接到 Microsoft Defender for Cloud 数据连接器。

1. 在页面顶部显示 Microsoft Azure 旁边蓝色栏的搜索框中，输入“Microsoft Sentinel”，然后在搜索结果中选择“Microsoft Sentinel”。 

1. 在“Microsoft Sentinel”页中，选择使用 Microsoft Sentinel 实例创建的工作区：SC900-LogAnalytics-workspace。

1. 可使用 Microsoft Sentinel 完成的第一步是收集数据。 在左侧导航面板中选择配置下方列出的“数据连接器”。

1. 在“数据连接器”页面中，向下滚动主窗口，以查看可用连接器的详细列表。 在“数据连接器”页的“搜索”框中，输入“Microsoft Defender for Cloud”，然后从列表中选择“Microsoft Defender for Cloud” 。

1. “Microsoft Defender for Cloud 连接器”窗口随即打开。 查看说明，然后选择“打开连接器”页。

1. 在“Microsoft Defender for Cloud 连接器”页面中，查看窗口左侧的“说明”。

1. 主窗口中的“说明”选项卡给出了先决条件。  查看说明和配置信息。
    主窗口中的“说明”选项卡给出了先决条件。  查看说明和配置信息。
    1. 从配置部分中，选择列出的订阅“MOC 订阅--lodXXXXXXXXX”旁边的空框，这样蓝色框中就会出现一个复选标记，然后选择“连接”（连接选项显示在搜索框上方） 。  此时会显示“连接”窗口，选择“确定”。  在订阅旁边的状态列中，应会看到状态更新为“已连接”。  如果在页面左侧的窗口中看不到连接状态，请不要担心，不要刷新浏览器。
    1. 向下滚动页面并选择“启用”，从连接服务中生成的所有警报自动创建事件。
    1. 现在，选择页面顶部的“后续步骤”选项卡，查看此数据连接器的建议工作簿。  Microsoft Sentinel 附带内置的工作簿模板，支持在连接到数据源后快速了解数据。
    1. 选择“ASC 合规性和保护”（注意：ASC 或 Azure 安全中心现在称为 Microsoft Defender for Cloud）。  此操作将打开工作簿页面。  在屏幕右侧查看说明，然后从屏幕底部选择“保存”，然后选择“确定”将工作簿保存到默认位置。  现在选择“查看保存的工作簿”。  
    1. 在工作区字段中，选择“SC900-LogAnalytics-workspace”。
    1. 在工作簿页面顶部，选择“自动刷新: 关闭”，然后选择“5 分钟”并选择“应用”  。
    1. 在工作簿页面顶部，选择“保存”图标。
    1. 在“工作簿”页的左上角，选择“工作簿”上方的“Microsoft Sentinel”。 这会返回到“概述”页面。 现在，应会看到上方表示已连接的数字 1，以指示有一个活动连接器（可能需要选择刷新）。

1. 请将此页面保持打开状态，因为在下一个任务中将用到它。

### <a name="demo-part-4"></a>演示第 4 部分

在演示的此部分中，你将显示 Sentinel 中可用的一些选项。

1. 从左侧导航面板中，选择“搜寻”。  从已选中（带下划线）的“查询”选项卡中，从列表中选择任何查询。  选择查询后，请注意提供的有关该查询的信息，包括查询的代码，以及运行查询和查看结果的选项。  不要选择任何内容。

1. 从左侧导航面板中，选择“MITRE ATT&CK”。  MITRE ATT&CK 是攻击者常用的策略和技术的公开访问知识库。 通过 Microsoft Sentinel，可以根据 MITRE ATT&CK® 框架中的策略和技术，来查看工作区中已经处于活动状态的检测，以及可供配置的检测，从而了解组织的安全覆盖范围。  从矩阵中选择任何单元格，并记下屏幕右侧可用的信息。  

1. 从左侧导航面板中，选择“社区”。 Microsoft 安全分析师会不断创建和添加新的工作簿、playbook、搜寻式查询及其他资源，并将其发布到社区，供你在环境中使用。 可以从个人社区 GitHub 存储库下载示例内容，以创建适用于 Microsoft Sentinel 的自定义工作簿、搜寻式查询、Notebook 和 Playbook。  选择“加入社区内容”。  此时会打开 GitHub 存储库的新选项卡，可在其中下载内容以启用方案。  在浏览器中，返回到 Azure 选项卡。

1. 从左侧导航面板中，选择“分析”。  从“高级多阶段攻击检测”列表中选择第一项。  请注意详细信息。  Microsoft Sentinel 使用 Fusion（基于可缩放的机器学习算法的关联引擎）通过识别在不同杀伤链阶段观测到的异常行为与可疑活动的组合来自动检测多阶段攻击（也称为高级持久威胁）。 Microsoft Sentinel 根据这些发现结果生成事件，否则很难捕获这些事件。

1. 从左侧导航面板中，选择“自动化”。  在这里，可以创建简单的自动化规则、与现有 playbook 集成或创建新的 playbook。  选择“+ 创建”，然后选择“自动化规则”。  请注意在屏幕右侧打开的窗口以及可用于创建条件和操作的选项。  选择屏幕底部的“取消”。

1. 从左侧导航面板中，选择“工作簿”。 从“工作簿”页面中选择“我的工作簿”选项卡，其位于搜索框上方。  已列出先前保存的工作簿，并且该工作簿可用于查看和监视数据。   注意：Azure 订阅中没有任何实际活动要反映在工作簿中，Azure 实验室订阅在收集可在工作簿中可视化的数据时可能会遇到比正常情况更长的延迟。

1. 选择窗口右上角的“X”关闭窗口。

1. 从窗口左上角的蓝色条下方，选择“主页”以返回到 Azure 门户的主页。  

### <a name="review"></a>审阅

在此演示中，你逐步完成了将 Microsoft Sentinel 连接到数据源的步骤，设置了工作簿，并演示了 Microsoft Sentinel 中提供的多个选项。
