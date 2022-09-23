---
ms.openlocfilehash: eeee584ece9bb3ec4edcba5fa2e76a13dd9459c4
ms.sourcegitcommit: 15658ca1c7bae8a4dbaa33ab6f897070bde521b9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2022
ms.locfileid: "147892601"
---
<a name="---"></a><!---
---
Lab: Title: '探索 Microsoft Defender for Cloud' Learning Path/Module/Unit: '学习路径：描述 Microsoft 安全解决方案的功能；模块 2：描述 Azure 的安全管理功能；第 3 单元：描述 Microsoft Defender for Cloud'
---
--->

# <a name="lab-explore-microsoft-defender-for-cloud"></a>实验室：探索 Microsoft Defender for Cloud

此实验室与下列 Learn 内容保持一致：

- 学习路径：描述 Microsoft 安全解决方案的功能
- 模块：描述 Azure 的安全管理功能
- 单元：描述 Microsoft Defender for Cloud

## <a name="lab-scenario"></a>实验室场景

在本实验中，你将探索 Microsoft Defender for Cloud，并了解如何使用 Azure 安全功能分数来改善组织的安全态势。  注意：此演示演练假定演示者通过 Azure Pass 对 Azure 订阅具有管理员级权限。  由授权实验室主机托管服务提供商管理的 Azure 订阅（如 Cloudslice 订阅）会限制访问和功能，因此下面的一些步骤可能不可用或不显示任何信息。

预计用时：30 分钟

### <a name="setup"></a>设置

在此任务中，你将对 Microsoft Defender for Cloud 进行一些基本设置，以使订阅准备就绪，并启用和分配默认策略。

1. 打开 Microsoft Edge。 在地址栏中，输入“portal.azure.com”。

1. 使用管理员凭据登录。
    1. 在“登录”窗口中，输入 admin@WWLxZZZZZZ.onmicrosoft.com（其中 ZZZZZZ 是实验室托管提供商提供的唯一租户 ID），然后选择“下一步” 。
    1. 输入管理员密码，该密码应由实验室托管提供商提供。 选择“登录”。
    1. 在提示保持登录状态时，选择“是”。

1. 在屏幕左上角的“Microsoft Azure”旁边，选择“显示门户菜单”图标（三条横线，也称为汉堡图标），然后在左侧导航面板的“收藏夹”下选择“Microsoft Defender for Cloud”。  如果它未在收藏夹下列出，请在搜索框中输入“Microsoft Defender for Cloud”，然后从结果列表中选择“Microsoft Defender for Cloud”。

1. 如果这是你首次使用订阅进入 Microsoft Defender for Cloud，可能会登陆到“入门”页面，系统还可能提示进行升级。  滚动到页面底部，然后选择“跳过”。  此时会转到“概述”页。
    1. 在页面顶部，你将看到一个浅蓝色的信息框，指示“正在为订阅做好准备。 这可能需要几分钟的时间...”
    1. 订阅准备就绪后，可能会出现一个新的信息框，显示“一个订阅未分配有默认策略。 若要查看订阅列表，请打开‘安全策略’页。”  选择句子末尾的右箭头，或从左侧导航窗格中选择“环境设置”。
        1. 现在你位于“环境设置”页。 选择“Azure Pass - 赞助”。  注意：如果 Azure 环境基于由授权实验室主机托管服务提供商管理的 Azure 订阅，而不是 Azure Pass，则会看到它被引用。 通过选择大于符号来展开选项，直到无法再展开选项并看到订阅。
        1. 从左侧导航窗格中，选择“安全策略”。
        1. 从主页的“默认计划”下，选择“分配策略”。
        1. 从页面底部，选择“查看 + 创建”。
        1. 从页面底部，选择“创建”。  这会将 Azure 安全基准指定为默认策略计划。  刷新屏幕（可能需要几分钟才能生效）。
        1. 通过选择页面上的“X”退出环境设置页。  
        1. 从 Azure 服务页中选择“Microsoft Defender for Cloud”以返回到概述页。

### <a name="task-1"></a>任务 1

在此任务中，你将大致演练 Microsoft Defender for Cloud 的一些功能

1. 在 Microsoft Defender for Cloud 的“概述”页中，请注意页面上提供的信息。  页面顶部的信息包括 Azure 订阅数、评估资源数、可用建议数和任何安全警报。  在页面的正文中，有表示安全功能分数、法规合规性、见解等内容的卡片。

1. 在页面顶部选择“已评估的资源”。  （请注意，这相当于在 Microsoft Defender for Cloud 主页的左侧导航面板中选择“清单”）。
    1. 随后会转到“清单”页面，其中显示 Azure Pass 订阅。  选择“Azure Pass - 赞助”。
    1. “资源运行状况”页面提供建议列表。  在可用列表中，选择“应向订阅分配多个所有者”。
    1. 选择“修正”步骤旁的向下箭头。 注意详细的修正步骤是如何与执行操作的选项一起提供的。  
    1. 从屏幕左上角选择“Microsoft Defender for Cloud”以返回到 Microsoft Defender for Cloud 概述页面。

1. 在页面顶部选择“可用建议”。  （请注意，这相当于在 Microsoft Defender for Cloud 主页的左侧导航面板中选择“建议”）。
    1. “建议”页面显示了安全功能分数仪表板。
    1. 安全功能分数仪表板下方有控制措施列表。 每项安全控制措施都表示一项应该缓解的安全风险，其中还有与该控制措施相关的最高分数、当前分数、潜在分数增加和资源运行状况状态的信息。  
    1. 选择其中一项控制措施，例如“实现安全最佳做法”。  选择其中一个子项，例如“应为订阅分配多个所有者”。  在打开的页面中，你将看到一段描述、修正步骤和受影响的资源。 选择屏幕右上角的“X”退出此页面。
    1. 选择屏幕右上角的“X”退出“建议”页面，返回到概述页面。

1. 在主页中选择“法规合规性”。 “法规合规性”页面上提供了合规性控制措施列表。  每项控制措施下都有一组基于 Azure 安全基准的评估；该基准针对如何保护 Azure 上的云解决方案提供相关建议。
    1. 选择“IM.标识管理”，然后选择“IM-6 使用强身份验证控件”。  列表显示了可用于改进合规性态势的客户责任操作。
    1. 选择屏幕右上角的“X”关闭页面，返回到 Microsoft Defender for Cloud 概述页面。
    1. 使 Microsoft Defender for Cloud 概述页面保持打开状态，你将在下一个任务中使用它。

### <a name="task-2"></a>任务 2

还记得吗，Microsoft Defender for Cloud 有两种模式：没有增强的安全功能（免费）以及具有通过 Microsoft Defender for Cloud 计划提供的增强安全功能。 在此任务中，你将了解如何启用/禁用各种 Microsoft Defender for Cloud 计划。

1. 在 Microsoft Defender for Cloud 概述页面中，从左侧导航面板中选择“环境设置”。
1. 选择“租户根组”旁边的大于号 > 以将其展开（不要直接选择“租户根组”，因为这样会引导你访问其他页面），然后选择“Azure Pass - 赞助”
1. 在“Defender 计划”页上，注意如何选择“全部启用”或选择单个 Defender 计划。 在将所有计划设置为关闭的情况下将设置保留原样。
1. 关闭所有打开的浏览器选项卡。

### <a name="review"></a>审阅

在本实验中，你探索了 Microsoft Defender for Cloud，并了解了如何使用 Azure 安全功能分数来改善组织的安全态势。
