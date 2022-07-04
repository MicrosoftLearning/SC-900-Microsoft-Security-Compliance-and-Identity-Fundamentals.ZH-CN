---
Demo:
  title: Microsoft Defender for Cloud
  module: 'Module 3 Lesson 2: Describe the capabilities of Microsoft security solutions: Describe security management capabilities of Azure'
ms.openlocfilehash: ff5145e967445c12dacd90ea50002fe0c3042efb
ms.sourcegitcommit: b8b861a8c884a56f094213e47a59be48ba898ca1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "146741899"
---
# <a name="demo-microsoft-defender-for-cloud"></a>演示：Microsoft Defender for Cloud

## <a name="demo-scenario"></a>演示方案

在本演示中，你将演练 Microsoft Defender for Cloud，并介绍如何利用 Azure 安全功能分数来改善组织的安全态势。  注意：此演示演练假定演示者通过 Azure Pass 对 Azure 订阅具有管理员级权限。  由授权实验室主机托管服务提供商管理的 Azure 订阅（如 Cloudslice 订阅）会限制访问和功能，因此下面的一些步骤可能不可用或不显示任何信息。

### <a name="demo-setup"></a>演示设置

在此设置任务中，你将对 Microsoft Defender for Cloud 进行一些基本设置，以使订阅准备就绪，并启用和分配默认策略。 请在课堂上演示之前执行此操作。 

1. 打开浏览器选项卡“主页 - Microsoft Azure”。  如果之前关闭了该选项卡，请打开浏览器页面，在地址栏中输入 portal.azure.com，然后重新登录。

1. 在搜索框中，在页面顶部显示 Microsoft Azure 的位置旁边的蓝色栏中，输入“Microsoft Defender for Cloud”，然后从搜索结果中选择“Microsoft Defender for Cloud” 。

1. 如果这是你首次使用订阅进入 Microsoft Defender for Cloud，可能会登陆到“入门”页面，系统还可能提示进行升级。  滚动到页面底部，然后选择“跳过”。  此时会转到“概述”页。
    1. 在页面顶部，你将看到一个浅蓝色的信息框，指示“正在为订阅做好准备。 这可能需要几分钟的时间...”
    1. 订阅准备就绪后，将出现一个新的信息框，显示“一个订阅未分配有默认策略。 若要查看订阅列表，请打开‘安全策略’页。”  选择句子末尾的右箭头。
        1. 现在你位于“环境设置”页。 选择“Azure Pass - 赞助”。 
        1. 从左侧导航窗格中，选择“安全策略”。
        1. 从主页的“默认计划”下，选择“分配策略”。
        1. 从页面底部，选择“查看 + 创建”。
        1. 从页面底部，选择“创建”。
        1. 从页面顶部的 Microsoft Azure 下方，从痕迹导航中选择“Microsoft Defender for Cloud”以返回到概述页面。

### <a name="demo-task"></a>演示任务

在此演示任务中，你将大致演练 Microsoft Defender for Cloud 的一些功能。

1. Microsoft Defender for Cloud 概述页面顶部的信息包括 Azure 订阅数、评估资源数、可用建议数和任何安全警报。  在页面的正文中，有表示安全功能分数、法规合规性、见解等内容的卡片。  

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

1. 你回到了 Microsoft Defender for Cloud 概述页面。  在主页中选择“法规合规性”。 （请注意，这相当于在 Microsoft Defender for Cloud 主页的左侧导航面板中选择“建议”）。
    1. “法规合规性”页面上提供了合规性控制措施列表。  每项控制措施下都有一组基于 Azure 安全基准的评估；该基准针对如何保护 Azure 上的云解决方案提供相关建议。
    1. 选择“IM.标识管理”，然后选择“IM-6 使用强身份验证控件”。  列表显示了可用于改进合规性态势的客户责任操作。
    1. 选择屏幕右上角的“X”关闭页面，返回到“法规合规性”页面。
    1. 选择屏幕右上角的“X”，返回到概述页面。

1. 还记得吗，Microsoft Defender for Cloud 有两种模式：没有增强的安全功能（免费）以及具有通过 Microsoft Defender for Cloud 计划提供的增强安全功能。 在这里，你将了解如何启用/禁用各种 Microsoft Defender for Cloud 计划。
    1. 在 Microsoft Defender for Cloud 概述页面中，从左侧导航面板中选择“环境设置”。
    1. 选择“租户根组”旁边的大于号 > 以将其展开（不要直接选择“租户根组”，因为这样会引导你访问其他页面），然后选择“Azure Pass - 赞助”
    1. 在“Defender 计划”页上，注意如何选择“全部启用”或选择单个 Defender 计划。 在将所有计划设置为关闭的情况下将设置保留原样。
    1. 选择屏幕右上角的“X”，返回到“环境设置”页。
    1. 选择屏幕右上角的“X”，返回到概述页面。

1. 选择页面左上角的“主页”，返回到 Azure 门户主页。  将此浏览器选项卡保持在可用状态，因为在稍后的演示中将回到此页面。

## <a name="review"></a>审阅

在本演示中，你演练了 Microsoft Defender for Cloud，并介绍了如何利用 Azure 安全功能分数来改善组织的安全态势。
