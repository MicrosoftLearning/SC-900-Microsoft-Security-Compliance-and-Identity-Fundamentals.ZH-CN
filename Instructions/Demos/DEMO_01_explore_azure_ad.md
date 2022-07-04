---
Demo:
  title: Azure Active Directory 用户设置
  module: 'Module 2 Lesson 1: Describe the capabilities of Microsoft Identity and access management solutions: Explore the services and identity types of Azure AD'
ms.openlocfilehash: 061dfa556f7e4e00d63c938b52097e0b641fed4f
ms.sourcegitcommit: b8b861a8c884a56f094213e47a59be48ba898ca1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "146741887"
---
# <a name="demo-azure-active-directory-user-settings"></a>演示：Azure Active Directory 用户设置

## <a name="demo-scenario"></a>演示方案

在本演示中，你将访问 Azure Active Directory，并演练现有用户的各种设置。  演示者注意：此演示通过 Microsoft 365 租户访问 Azure AD。 向学员展示的另一种选择是通过 Azure 门户访问 Azure AD。 通过 Microsoft 365 门户的意图是显示 Microsoft 365 包括对 Azure AD 的访问权限。

1. 打开 Microsoft Edge。

1. 在地址栏中，输入“admin.microsoft.com”以访问 Microsoft 365 管理中心。

1. 使用管理员凭据登录。
    1. 在“登录”窗口中，输入 admin@WWLxZZZZZZ.onmicrosoft.com（其中 ZZZZZZ 是实验室托管提供商提供的唯一租户 ID），然后选择“下一步” 。
    1. 输入管理员密码，该密码应由实验室托管提供商提供。 选择“登录”。
    1. 在提示保持登录状态时，选择“是”。

1. 从 Microsoft 365 管理中心的左侧导航窗格中，选择“全部显示”。

1. 在“管理中心”下，选择“Azure Active Directory”（可能需要向下滚动）。  这会打开一个新的浏览器页面，显示 Azure Active Directory 管理中心的“我的仪表板”页。 在仪表板的主窗口中，你将看到一些磁贴，包括组织的标识磁贴（Contoso、租户和 Azure AD 版本）、用户和组的磁贴等。

1. 从左侧导航窗格中，选择“用户”。 注意租户已配置了用户。

1. 在用户列表中，选择“Adele Vance”。

1. 请注意在左侧导航面板中，已选中“个人资料”。  显示/说明在个人资料页上显示的信息。

1. 在左侧导航面板中，选择“已分配的角色”。  未向此用户分配任何管理角色。  在页面顶部选择“+添加分配”，显示可用的管理角色类型。  请不要添加任何项，只需选择页面右上角的“X”关闭页面即可。

1. 在左侧导航面板中，选择“组”。  指出此用户属于多个组。  在这里可说明组的类型。  若要将此用户添加到其他组，只需选择“+添加成员身份”即可。  请勿添加任何新组，只需说明很轻松就能将用户添加到现有组即可。 选择页面右上角的“X”关闭组窗口。

1. 在左侧导航面板中，选择“许可证”。 请注意已向此用户分配了 Microsoft 365 E5 许可证和 EMS 许可证。  若要添加许可证，请在主窗口顶部选择“+分配”。  显示此用户的许可证。 请勿更改任何内容。  选择页面右上角的“X”关闭此窗口。

1. 在左侧导航面板中，选择“设备”。  未显示任何内容，但你可指出如果向此用户分配了设备，设备会在此处显示。

1. 在左侧导航面板中，选择“Azure 角色分配”。  请注意：
    1. 这与上述“已分配的角色”选项卡不同，上述选项卡用于 Azure Active Directory 中基于角色的访问控制（强调 Active Directory）。
    1. 在此选项卡中，可查看针对 Azure 资源分配给用户的角色分配。 例如，如果要创建一个 Azure 资源组，并向 Adele 分配一个特定角色（比如资源组的所有者或参与者），那么此处会列出该角色。 这是 Azure 基于角色的访问控制 (Azure RBAC) 的一部分。 这种角色分配作为该特定资源的一部分进行管理。

1. 在左侧导航面板中，选择“身份验证方法”。  指出有描述显示“在这里，你可以设置用户用于执行多重身份验证和自助式密码重置的电话号码和电子邮件地址，并重置用户密码。” 如果用户配置有 SSPR 或需要使用 MFA，而你身为管理员填充了此信息，那么该用户已注册，无需再执行 SSPR 或 MFA 的注册步骤。  通常，用户会自行注册，而不是由管理员进行注册。

1. 在左侧导航面板中，选择“登录”。在这里，你能看到此用户的登录活动。  由于此用户尚未登录，因此你可能看不到其任何信息。

1. 选择页面右上角的“X”。 这会回到用户列表。  在关闭用户列表之前，可强调页面顶部显示了 MFA。  选择“多重身份验证”。  此时将打开一个新的浏览器窗口。  你可在这里为用户批量选择 MFA。  这是为用户启用 MFA 的一种方式。  实际上，我们将在条件访问的情况下更详细地介绍 MFA，条件访问可更精细地控制 MFA。  关闭多重身份验证的浏览器选项卡。

1. 选择页面右上角的“X”。 这会回到 Contoso 租户的主页。

### <a name="review"></a>审阅

在本演示中，你演练了现有用户的设置，其中包括可将该用户分配到的组、角色的可用性以及用户许可证的分配。
