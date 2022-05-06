---
Demo:
  title: Azure Active Directory 自助式密码重置
  module: 'Module 2 Lesson 2: Describe the capabilities of Microsoft Identity and access management solutions: Describe the different authentication methods of Azure AD'
ms.openlocfilehash: 819439157f86ba4a28255cf876e239f3960df8f4
ms.sourcegitcommit: 25998048c2e354ea23d6f497205e8a062d34ac80
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2022
ms.locfileid: "144557214"
---
# <a name="demo-azure-active-directory-self-service-password-reset-sspr"></a>演示：Azure Active Directory 自助式密码重置 (SSPR)

## <a name="demo-scenario"></a>演示方案

在本演示中，你将演练与启用自助式密码重置相关的各种设置。

1. 转到浏览器中打开的“Contoso - Microsoft Azure”选项卡。 如果之前关闭了该选项卡，请打开浏览器页面，在地址栏中输入 portal.azure.com，然后选择“Azure Active Directory”。 你应在 Azure 门户中以管理员身份登录；如果没有，请重新登录。

1. 从左侧导航窗格中，选择“密码重置”。

1. “属性”选项卡突出显示。  请注意，在“属性”窗口中，SSPR 可以为“无”、“选定”或“全部”。
    1. 将光标置于显示“自助式密码重置已启用”旁边的信息图标上，指出你可选中“选定”，仅允许一组有限的用户重置密码，而不是选择“无”或“全部”。
    1. 将光标置于显示“选择组”旁边的信息图标上，指出在这里确定允许哪些用户重置其自己的密码。   必须将用户包含在组中，不能单独选择用户。  此外，如果更改组，则你选择的组将替换当前列出的组。  因此，建议只将用户添加到 SSPR 组中。
    1. 请注意浅蓝色的信息框，并将其告知学员 - 这些设置仅适用于组织中的最终用户。 始终为管理员启用自助式密码重置，且管理员需要使用两种身份验证方法来重置其密码。

1. 从“密码重置”的左侧导航面板中，选择“身份验证方法”。
    1. 将光标置于显示“重置所需的方法数”旁边的信息图标上。  指出这将设置此目录中的用户重置其密码所必需的备用标识方法数目。   请勿更改设置。
    1. 指出不同的“用户可用方法”，包括 SSPR 支持安全问题这一点。 选择“安全问题”，显示使用安全问题的选项。 说明这些选项后，返回并选择“安全问题”来删除复选标记。

1. 从“密码重置”的左侧导航面板中，选择“注册”。
    1. 将鼠标悬停在显示“要求用户在登录时注册”旁边的信息图标上。   将这一点告知用户。  
    1. 将鼠标悬停在显示“要求用户重新确认其身份验证信息之前的天数”旁边的信息图标上。   将这一点告知用户。  

1. 从“密码重置”的左侧导航面板中，选择“通知”。  说明两个设置 - 将鼠标悬停在描述的信息图标上。

1. 请注意“密码重置”导航窗格如何另外显示用于查看审核日志和“使用情况和见解”的选项。

1. 选择页面右上角的“X”。 这会回到 Contoso 租户的主页。

1. 将此浏览器页面保持在打开状态，进行下一演示。

### <a name="review"></a>审阅

在本演示中，你演示了与自助式密码重置相关的设置。
