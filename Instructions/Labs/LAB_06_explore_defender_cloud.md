---
lab:
    title: '实验室：探索 Microsoft Defender for Cloud'    
    module: '模块 2：描述 Azure 的安全管理功能'
---


# <a name="lab-explore-microsoft-defender-for-cloud"></a>实验室：探索 Microsoft Defender for Cloud

此实验室与下列 Learn 内容保持一致：

- 学习路径：描述 Microsoft 安全解决方案的功能
- 模块：描述 Azure 的安全管理功能
- 单元：描述 Microsoft Defender for Cloud

## <a name="lab-scenario"></a>实验室场景

在此实验室中，你将探索 Microsoft Defender for Cloud。  注意：由授权实验室托管商 (AH) 提供的 Azure 订阅会限制访问，并且可能会遇到比正常情况更长的延迟。

预计用时：30 分钟

### <a name="task-1"></a>任务 1

在此任务中，你将大致演练 Microsoft Defender for Cloud 的一些功能

1. 打开 Microsoft Edge。 在地址栏中，输入“portal.azure.com”。
1. 使用管理员凭据登录。
    1. 在“登录”窗口中，输入实验室托管提供商提供的用户名，然后选择“下一步”。
    1. 输入管理员密码，该密码应由实验室托管提供商提供。 选择“登录”。
    1. 在提示保持登录状态时，选择“是”。

1. 在蓝色搜索栏中输入“Microsoft Defender for Cloud”，然后从结果列表中选择“Microsoft Defender for Cloud” 。

1. 如果这是你首次使用订阅进入 Microsoft Defender for Cloud，可能会登陆到“入门”页面，系统还可能提示进行升级。  滚动到页面底部，然后选择“稍后提醒我”（或“跳过”） 。  此时会转到“概述”页。

1. 在 Microsoft Defender for Cloud 的概述页面中，请注意该页上可用的信息（如果没有看到任何评估的资源和活动建议，请刷新浏览器页面，这可能需要几分钟时间）。  页面顶部的信息包括 Azure 订阅数、评估资源数、可用建议数和任何安全警报。  在页面的正文中，有表示安全态势、法规合规性、见解等内容的卡片。  注意：Microsoft Defender for Cloud 默认策略计划（通常必须由管理员分配）已作为 Azure 订阅设置的一部分进行分配。 但是，安全功能分数将显示为 0%，因为 Azure 可能会延迟 24 小时才能反映初始分数。

1. 在页面顶部选择“已评估的资源”。  （请注意，这相当于在 Microsoft Defender for Cloud 主页的左侧导航面板中选择“清单”）。
    1. 随后会转到“清单”页，其中列出了当前资源。 选择虚拟机资源“sc900-winwm”。 此资源与在上一实验室中使用的虚拟机相关联。
    1. VM 的“资源运行状况”页面提供有建议列表。  从可用列表中，选择显示“运行不正常”状态的任何项。
    1. 请注意详细说明。  选择“修正”步骤旁的向下箭头。 请注意如何提供修正说明（或指向说明的链接）以及执行操作的选项。  退出窗口，不执行任何操作。
    1. 返回到 Microsoft Defender for Cloud 概述页面，方法是从页面顶部显示“资源运行状况”的位置上方选择“Microsoft Defender for Cloud | 概述”。

1. 从左侧导航面板中，选择“建议”。  （请注意，这相当于从 Microsoft Defender for Cloud 概述页面的顶部选择“可用建议”）。
    1. 验证是否已选中“所有建议”选项卡（带下划线）。  请注意，仪表板视图按严重性、资源运行状况等显示活动建议。
    1. 请注意，某些项显示为运行不正常的资源，如行项右侧的红色条所示。  从列表中选择任何运行不正常的资源。  在打开的页面中，你将看到一段描述、修正步骤和受影响的资源。 选择屏幕右上角的“X”退出此页面。
    1. 选择屏幕右上角的“X”退出“建议”页面，返回到概述页面。

1. 在左侧主导航面板中，选择“法规合规性”。 法规合规性页面提供基于 Microsoft 云安全基准的合规性控制列表（验证是否已选中 Microsoft 云安全基准选项卡 [带下划线]）。 每个控制域下是控制的一个子集，每个控制都有一个或多个评估。 每个评估都提供信息，包括说明、修正和受影响的资源。
    1. 让我们来探索一个控制域区域。 选择（展开）“NS. 网络安全性”。 将显示与网络安全相关的控制列表。
    1. 选择“应启用 NS-10. Microsoft Defender for DNS”。 请注意自动评估列表（包括 AWS 的自动评估）以及每个评估行项如何提供信息，包括资源类型、失败的资源和合规性工作站。 选择列出的评估。  此处显示的信息包括说明、修正步骤和受影响的资源。
    1. 选择屏幕右上角的“X”关闭页面。
    1. 从左侧导航面板中选择“概述”，返回到 Microsoft Defender for Cloud 概述页。
    1. 使 Microsoft Defender for Cloud 概述页面保持打开状态，你在下一个任务中会用到它。

### <a name="task-2"></a>任务 2

还记得吗，Microsoft Defender for Cloud 有两种模式：没有增强的安全功能（免费）以及具有通过 Microsoft Defender for Cloud 计划提供的增强安全功能。 在此任务中，你将了解如何启用/禁用各种 Microsoft Defender for Cloud 计划。

1. 在 Microsoft Defender for Cloud 概述页面中，从左侧导航面板中选择“环境设置”。
1. 选择“全部展开”框，然后选择黄色键图标旁边列出的“MOC 订阅--lodXXXXXXXX”订阅 。
1. 在“Defender 计划”页上，注意如何选择“全部启用”或选择单个 Defender 计划。 
    1. 验证 CSPM 状态是否设置为“开”，如果没有，请立即设置。  
    1. 为服务器启用计划。  对于“服务器”行项，选择“开”，然后从页面顶部选择“保存” 。
1. 关闭所有打开的浏览器选项卡。

### <a name="review"></a>审阅

在此实验室中，你探索了 Microsoft Defender for Cloud。
