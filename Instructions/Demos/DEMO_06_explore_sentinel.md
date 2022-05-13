---
Demo:
  title: Microsoft Sentinel
  module: 'Module 3 Lesson 3: Describe the capabilities of Microsoft security solutions: Describe security capabilities of Microsoft Sentinel'
ms.openlocfilehash: 242d971510a428170a0d531b1ddcdf422ed4f9c9
ms.sourcegitcommit: 25998048c2e354ea23d6f497205e8a062d34ac80
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2022
ms.locfileid: "144557322"
---
# <a name="demo-microsoft-sentinel"></a>演示：Microsoft Sentinel

## <a name="demo-scenario"></a>演示方案

在本演示中，你将演练创建 Microsoft Sentinel 实例的过程。  你还将设置权限，以确保可访问将为支持 Microsoft Sentinel 而部署的资源。  完成此基本设置后，你将逐步完成将 Microsoft Sentinel 连接到数据源并创建工作簿以监视和可视化数据的步骤。  最后，你将显示可用的一些其他选项，包括在发生任何可疑情况时获得通知的内置分析、自动化功能等等。

### <a name="pre-demo-setup--create-an-microsoft-sentinel-instance"></a>预演示设置：创建 Microsoft Sentinel 实例

1. 打开浏览器选项卡“主页 - Microsoft Azure”。  如果之前关闭了该选项卡，请打开浏览器页面，在地址栏中输入 portal.azure.com，然后重新登录。

1. 在页面顶部显示 Microsoft Azure 旁边蓝色栏的搜索框中，输入“Microsoft Sentinel”，然后在搜索结果中选择“Microsoft Sentinel”。 

1. 在“Microsoft Sentinel”页中，选择“创建 Microsoft Sentinel”。

1. 在“将 Microsoft Sentinel 添加到工作区”页中，选择“创建新工作区”。

1. 在“创建 Log Analytics”工作区的“基本”选项卡中，输入以下内容：
    1. 订阅：Azure Pass - 赞助
    1. 资源组：选择“新建”，输入名称“SC900-Sentinel-RG”，然后选择“确定”  。
    1. 名称：SC900-LogAnalytics-workspace。
    1. 区域：美国东部（可能会根据你的位置选择不同的默认区域）
    1. 选择“下一页:标记 >”

1. 对于标记，可将其留空，然后选择“查看 + 创建”。

1. 验证输入的信息，然后选择“创建”。

1. 可能需要一两分钟才会列出新工作区，如果仍未看到它，请选择“刷新”，然后选择“添加” 。

1. 添加新工作区后，将显示“Microsoft Sentinel | 新闻和指南”页。  请注意，“入门”页面列出了三个步骤。

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

    1. 选择窗口右上角的“X”关闭此窗口。

1. 在访问控制页面中，选择窗口右上角的“X”关闭此窗口。

### <a name="demo-part-3"></a>演示第 3 部分

在演示的本部分中，你需完成将 Microsoft Sentinel 连接到数据源以开始收集数据的过程。

1. 在页面顶部显示 Microsoft Azure 旁边蓝色栏的搜索框中，输入“Microsoft Sentinel”，然后在搜索结果中选择“Microsoft Sentinel”。 

1. 在“Microsoft Sentinel”页中，选择使用 Microsoft Sentinel 实例创建的工作区：SC900-LogAnalytics-workspace。

1. 可使用 Microsoft Sentinel 完成的第一步是收集数据。 在左侧导航面板中选择配置下方列出的“数据连接器”。

1. 在“数据连接器”页面中，向下滚动主窗口，以查看可用连接器的详细列表。 在“数据连接器”页面的“搜索”框中，输入“Office 365”，然后从列表中选择“Office 365”。

1. 此时会打开“Office 365 连接器”窗口。  选择“打开连接器页”。

1. 在“Office 365 连接器”页面中，查看窗口左侧的“说明”。

1. 主窗口中的“说明”选项卡提供 Microsoft Sentinel 与 Office 365 集成的先决条件，这些都应显示绿色复选标记。   在配置下，选择“Exchange”和“SharePoint”，然后选择“应用更改”。  几乎立即会看到窗口左侧的连接状态。

1. 通过选择窗口右上角的“X”关闭该窗口以返回到“数据连接器”页面。

1. “数据连接器”页面顶部应显示已连接 1 个连接器，以反映现已连接到 Office 365。 如果未看到此连接器，请选择“刷新”。 可能需要几分钟时间才能更新此页面。

1. 请将此页面保持打开状态，因为在下一个任务中将用到它。

### <a name="demo-part-4"></a>演示第 4 部分

在演示的此部分中，你将逐步完成为 Office 365 设置工作簿的过程，以可视化和监视数据。

1. 从左侧导航面板中，选择“工作簿”。

1. 在搜索框中输入“Office 365”，然后选择“Office 365”。

1. 在屏幕右侧打开的窗口中查看说明，然后从屏幕底部选择“保存”，然后选择“确定”将工作簿保存到默认位置。  现在选择“查看保存的工作簿”。

1. 此时会打开“Office 365 工作簿”页面。  选择“操作: 取消设置”旁边的下拉箭头，然后选择“全部”。  现在选择“用户: 查询挂起”旁边的下拉箭头，然后选择“全部”。  选择“保存(磁盘)”图标。 选择窗口右上角的“X”关闭此窗口。 数据可能需要几分钟时间才能开始显示在工作簿中，因此稍后将返回到工作簿。

1. 在“工作簿”页的左上角，选择“工作簿”上方的“Microsoft Sentinel”。 这会返回到“概述”页面。

### <a name="demo-part-5"></a>演示第 5 部分

在演示的此部分中，你将显示 Sentinel 中可用的一些选项。

1. 从左侧导航面板中，选择“搜寻”。  从已选中（带下划线）的“查询”选项卡中，从列表中选择任何查询。  选择查询后，请注意提供的有关该查询的信息，包括查询的代码，以及运行查询和查看结果的选项。  不要选择任何内容。

1. 从左侧导航面板中，选择“MITRE ATT&CK”。  MITRE ATT&CK 是攻击者常用的策略和技术的公开访问知识库。 通过 Microsoft Sentinel，可以根据 MITRE ATT&CK® 框架中的策略和技术，来查看工作区中已经处于活动状态的检测，以及可供配置的检测，从而了解组织的安全覆盖范围。  从矩阵中选择任何单元格，并记下屏幕右侧可用的信息。  

1. 从左侧导航面板中，选择“社区”。 Microsoft 安全分析师会不断创建和添加新的工作簿、playbook、搜寻式查询及其他资源，并将其发布到社区，供你在环境中使用。 可以从个人社区 GitHub 存储库下载示例内容，以创建适用于 Microsoft Sentinel 的自定义工作簿、搜寻式查询、Notebook 和 Playbook。  选择“加入社区内容”。  此时会打开 GitHub 存储库的新选项卡，可在其中下载内容以启用方案。  在浏览器中，返回到 Azure 选项卡。

1. 从左侧导航面板中，选择“分析”。  从“高级多阶段攻击检测”列表中选择第一项。  请注意详细信息。  Microsoft Sentinel 使用 Fusion（基于可缩放的机器学习算法的关联引擎）通过识别在不同杀伤链阶段观测到的异常行为与可疑活动的组合来自动检测多阶段攻击（也称为高级持久威胁）。 Microsoft Sentinel 根据这些发现结果生成事件，否则很难捕获这些事件。

1. 从左侧导航面板中，选择“自动化”。  在这里，可以创建简单的自动化规则、与现有 playbook 集成或创建新的 playbook。  选择“+ 创建”，然后选择“自动化规则”。  请注意在屏幕右侧打开的窗口以及可用于创建条件和操作的选项。  选择屏幕底部的“取消”。

1. 从左侧导航面板中，选择“工作簿”。 从“工作簿”页面中选择“我的工作簿”选项卡，其位于搜索框上方。  已列出先前保存的工作簿，并且该工作簿可用于查看和监视数据。  选择“Office 365”，然后在屏幕右侧打开的窗口中，选择“查看保存的工作簿”。  请注意与 Office 365 工作负载相关的可视化效果。  

1. 选择窗口右上角的“X”关闭此窗口。

1. 从窗口左上角的蓝色条下方，选择“主页”以返回到 Azure 门户的主页。

### <a name="task-6"></a>任务 6

授课后拆解。 我们将根据 Microsoft Sentinel 中为分析引入的数据量对 Microsoft Sentinel 进行计费。 尽管本演示中引入的数据量非常少，但也建议在完成探索 Microsoft Sentinel 的功能后删除 Microsoft Sentinel 资源组。

1. 在 Microsoft Sentinel 页的左上角，选择 Microsoft Sentinel 上方的“所有服务”。

2. 在“筛选服务”框中，输入资源组，然后从提供的列表中选择“资源组”。

3. 从“资源组”页面选择使用 Microsoft Sentinel 创建的资源组“SC900-ResourceGroup”。

4. 在页面顶部中心选择“删除资源组”。  查看警告。  输入资源组名称“SC900-ResourceGroup”，然后从页面底部选择“删除” 。  可能需要几分钟时间才可删除资源组。

5. 验证已删除资源组后，关闭浏览器页面。

### <a name="review"></a>审阅

在此演示中，你演练了将 Microsoft Sentinel 连接到数据源的步骤，你设置了工作簿，并演示了 Microsoft Sentinel 中提供的多个选项。
