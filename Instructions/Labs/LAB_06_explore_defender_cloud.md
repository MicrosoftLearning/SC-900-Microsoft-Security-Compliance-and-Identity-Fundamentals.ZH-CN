---
lab:
  title: 探索 Microsoft Defender for Cloud
  module: 'Module 3 Lesson 2: Describe the capabilities of Microsoft security solutions: Describe security management capabilities of Azure'
ms.openlocfilehash: 580e84e726a6ba9c7d9109881710e08f059d0818
ms.sourcegitcommit: 25998048c2e354ea23d6f497205e8a062d34ac80
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2022
ms.locfileid: "144557564"
---
# <a name="lab-explore-microsoft-defender-for-cloud"></a>实验室：探索 Microsoft Defender for Cloud

## <a name="lab-scenario"></a>实验室场景

在本实验中，你将探索 Microsoft Defender for Cloud，并了解如何使用 Azure 安全功能分数来改善组织的安全态势。

预计用时：30 分钟

### <a name="task-1"></a>任务 1

在此任务中，你将简单地浏览 Microsoft Defender for Cloud。

1. 打开 Microsoft Edge。 在地址栏中，输入“portal.azure.com”。

1. 使用管理员凭据登录。
    1. 在“登录”窗口中，输入 admin@WWLxZZZZZZ.onmicrosoft.com（其中 ZZZZZZ 是实验室托管提供商提供的唯一租户 ID），然后选择“下一步” 。
    1. 输入管理员密码，该密码应由实验室托管提供商提供。 选择“登录”。
    1. 在提示保持登录状态时，选择“是”。

1. 在屏幕左上角的“Microsoft Azure”旁边，选择“显示门户菜单”图标（三条横线，也称为汉堡图标），然后在左侧导航面板的“收藏夹”下选择“Microsoft Defender for Cloud”。  如果它未在收藏夹下列出，请在搜索框中输入“Microsoft Defender for Cloud”，然后从结果列表中选择“Microsoft Defender for Cloud”。

1. 请注意 Microsoft Defender for Cloud 概述页面上提供的信息。  

1. 可能会在页面顶部看到一个蓝色信息框，这表示你可能在查看限制性信息。  选择“单击此处”。
    1. 为了确保获得租户范围的可见性，请向自己分配必要的角色。  选择“安全管理员”，然后选择页面底部的“获取访问权限” 。
    1. 可能会看到消息“根管理组不存在”。  根据描述，系统将为你创建组。  最多可能需要 15 分钟才能完成（但通常会更快）。  授予访问权限后，选择页面左上角的“Microsoft Defender for Cloud”，其上方显示“获取权限”，然后刷新 Microsoft Defender for Cloud 概述页面。

1. 页面顶部的信息包括 Azure 订阅数、评估资源数、可用建议数和任何安全警报。  在页面的正文中，有表示安全功能分数、法规合规性、见解等内容的卡片。  

1. 在页面顶部选择“已评估的资源”。  （请注意，这相当于在 Microsoft Defender for Cloud 主页的左侧导航面板中选择“清单”）。
    1. 随后会转到“清单”页面，其中显示 Azure Pass 订阅。  选择“Azure Pass - 赞助”。
    1. “资源运行状况”页面提供建议列表。  在可用列表中，选择“应向订阅分配多个所有者”。
    1. 选择“修正”步骤旁的向下箭头。 注意详细的修正步骤是如何与执行操作的选项一起提供的。  
    1. 从屏幕左上角选择“Microsoft Defender for Cloud”以返回到 Microsoft Defender for Cloud 概述页面。

1. 在页面顶部选择“可用建议”。  （请注意，这相当于在 Microsoft Defender for Cloud 主页的左侧导航面板中选择“建议”）。
    1. “建议”页面显示了安全功能分数仪表板。
    1. 安全功能分数仪表板下方有控制措施列表。 每项安全控制措施都表示一项应该缓解的安全风险，其中还有与该控制措施相关的最高分数、当前分数、潜在分数增加和资源运行状况状态的信息。  
    1. 选择其中一项控制措施，例如“启用 MFA”。  选择其中一个子项，例如“应在对订阅拥有所有者权限的帐户上启用 MFA”。  在打开的页面中，你将看到一段描述、修正步骤和受影响的资源。 选择屏幕右上角的“X”退出此页面。
    1. 选择屏幕右上角的“X”退出“建议”页面，返回到概述页面。

1. 在主页中选择“法规合规性”。 “法规合规性”页面上提供了合规性控制措施列表。  每项控制措施下都有一组基于 Azure 安全基准的评估；该基准针对如何保护 Azure 上的云解决方案提供相关建议。
    1. 选择“IM.标识管理”，然后选择“IM-6 使用强身份验证控件”。  列表显示了可用于改进合规性态势的客户责任操作。
    1. 选择屏幕右上角的“X”关闭页面，返回到 Microsoft Defender for Cloud 概述页面。
    1. 使 Microsoft Defender for Cloud 概述页面保持打开状态，你将在下一个任务中使用它。

### <a name="task-2"></a>任务 2

在本任务中，你将导航到 Azure 安全功能分数，并探索可提高安全功能分数的建议。

1. 在 Microsoft Defender for Cloud 概述页面中，选择“安全评分”卡片。
1. 选择“Azure Pass - 赞助”。  记下安全功能分数。
1. 在“建议”页中，选择“实现安全最佳做法”以展开列表。 请注意，其资源运行状况显示为红色。
1. 选择项“应向订阅分配多个所有者”，它将资源运行状况显示为红色。
1. 在“受影响的资源”下方，确保“不正常的资源”已选中/带下划线，然后选择列出的 Azure 订阅。
1. 从“访问控制(IAM)”页面的顶部选择“+ 添加”，然后从下拉列表中选择“添加角色分配” 。
    1. 在页面左侧，选择“所有者”（这应该是列出的第一项），以便该行以灰色突出显示，然后选择页面底部的“下一步”。
    1. 在“成员”旁边，选择“+ 选择成员”。
    1. 在屏幕右侧打开的“选择成员”窗口中，选择“Alex Wilber”，然后按页面底部的“选择”。  
    1. 在“添加角色分配”页中，验证 Alex Wilber 是否已列为成员，然后选择“下一步”，然后选择“查看 + 分配”。
    1. 可能需要长达 24 小时的时间才会更新状态，之后，在满足“管理访问和权限”组中的所有项时，安全功能分数也将更新。
    1. 在页面左上角的“Azure Pass”上方，选择“Microsoft Defender for Cloud”以返回 Microsoft Defender for Cloud 概述页面。
1. 将此页面保持在打开状态，以便执行后续任务。

### <a name="task-3"></a>任务 3

还记得吗，Microsoft Defender for Cloud 有两种模式：没有增强的安全功能（免费）以及具有通过 Microsoft Defender for Cloud 计划提供的增强安全功能。 在此任务中，你将了解如何启用/禁用各种 Microsoft Defender for Cloud 计划。

1. 在 Microsoft Defender for Cloud 概述页面中，从左侧导航面板中选择“环境设置”。
1. 选择“租户根组”旁边的大于号 > 以将其展开（不要直接选择“租户根组”，因为这样会引导你访问其他页面），然后选择“Azure Pass - 赞助”
1. 在“Defender 计划”页上，注意如何选择“全部启用”或选择单个 Defender 计划。 在将所有计划设置为关闭的情况下将设置保留原样。
1. 现在可以关闭浏览器选项卡以退出 Azure 门户。

### <a name="review"></a>审阅

在本实验中，你探索了 Microsoft Defender for Cloud，并了解了如何使用 Azure 安全功能分数来改善组织的安全态势。
