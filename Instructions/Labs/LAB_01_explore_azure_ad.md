<a name="---"></a><!---
---
Lab: Title: '探索 Azure Active Directory' Learning Path/Module/Unit: '学习路径：描述 Azure Active Directory (Azure AD) 的功能（Microsoft Entra 的一部分）；模块 1：描述 Azure AD 的基本服务和标识类型；第 4 单元：描述 Azure AD 标识类型'
---
--->

# <a name="lab-explore-azure-active-directory"></a>实验室：探索 Azure Active Directory

此实验室与下列 Learn 内容保持一致：

- 学习路径：描述 Active Directory (Azure AD) 的功能（Microsoft Entra 的一部分）
- 模块：描述 Azure AD 的基本服务和标识类型
- 单元：描述 Azure AD 标识类型

## <a name="lab-scenario"></a>实验室场景

在此实验室中，你将访问 Azure Active Directory。  此外，你还将创建一个用户并配置不同设置，包括添加许可证。  

预计用时：10-15 分钟

### <a name="task-1"></a>任务 1

作为 Microsoft 365 的订阅者，你已在使用 Azure AD。  在本任务中，你将演练如何通过 Microsoft 365 管理门户和 Azure 门户访问 Azure AD。

1. 在 Microsoft Edge 浏览器中，选择标记为“主页 - Microsoft 365 管理员中心”的选项卡。

1. 如果之前关闭了该浏览器选项卡，请执行以下步骤：
    1. 在地址栏中输入 admin.microsoft.com 并使用管理员凭据登录，如下所示：
    1. 在“登录”窗口中，输入 admin@WWLxZZZZZZ.onmicrosoft.com（其中 ZZZZZZ 是实验室托管提供商提供的唯一租户 ID），然后选择“下一步” 。
    1. 输入管理员密码，该密码应由实验室托管提供商提供。 选择“登录”。
    1. 在提示保持登录状态时，选择“是”。
    1. 从 Microsoft 365 管理中心的左侧导航窗格中，选择“全部显示”。

1. 在“管理中心”下，选择“Azure Active Directory”（可能需要向下滚动）。  这会打开一个新的浏览器页面，显示 Azure Active Directory 管理中心的“我的仪表板”页。 在仪表板的主窗口中，你将看到一些磁贴，包括组织的标识磁贴（Contoso、租户和 Azure AD 版本）、用户和组的磁贴等。

1. 在左侧导航窗格的“收藏夹”下，选择“Azure Active Directory”。  在主窗口中，你将看到另一个导航面板，其中列出了 Azure AD 中提供的所有服务。 在右侧，你将看到有关 Contoso 租户的信息以及指向可以创建的标识类型和特色服务的链接。  

1. 现在，打开一个新的浏览器窗口，在地址栏中输入 portal.azure.com。  由于你已经以 admin@WWLxZZZZZZ.onmicrosoft.com 身份登录，并且最初使用这些相同凭据兑换了 Azure Pass，因此在访问 Azure 门户时应登录为管理员。  可以通过检查页面右上角的电子邮件并将鼠标悬停在用户图标上来验证这一点。

1. Azure 门户的登陆页面显示了包括 Azure Active Directory、VM、存储帐户、数据库等在内的 Azure 服务。  选择“更多服务”，然后选择“Azure Active Directory” 。 如果没有立即看到它，可以在蓝色搜索栏上输入 Azure Active Directory，并从搜索结果中选择它。  

1. 现在看到的是 Microsoft 365 Contoso 租户的 Azure Active Directory。    无论使用哪种方式来访问 Azure Active Directory 服务（Microsoft 365 管理门户或 Azure 门户），最终都会停留在同一位置 - 可在其中管理所有 Azure AD 服务的 Contoso Azure Active Directory。

1. 将此浏览器页面保持在打开状态，进行下一任务。

### <a name="task-2"></a>任务 2

在本任务中，你将了解如何在 Azure Active Directory 中创建新用户，并探索一些可在用户级别进行管理的服务。

1. 转到浏览器中打开的“Contoso - Microsoft Azure”选项卡。 如果之前关闭了该选项卡，请打开浏览器页面，在地址栏中输入 portal.azure.com，然后选择“Azure Active Directory”。  你应在 Azure 门户中以管理员身份登录；如果没有，请重新登录。

1. 从左侧导航窗格中，选择“用户”。  注意租户已配置了用户。

1. 在页面顶部，选择“+ 新建用户”，然后从下拉框中选择“创建新用户” 。

1. 如果未选择该选项，应已选中“创建新用户”。

1. 按如下所示填写“标识”字段：

    1. 用户名：sara。

    1. 名称字段：Sara Perez。

    1. 名字：Sara。

    1. 姓氏：Perez。

1. 按如下所示填写“密码”字段：

    1. 选择“让我创建密码”。

    1. 初始密码：Naja8996。 当 Sara 首次登录时，系统将提示她更改密码。

1. 配置“组和角色”。

    1. 在“组”旁边，选择“已选择 0 个组”。  这将显示可用的组。  请注意可用组的列表。

    1. 选择“操作”，可能需要向下滚动，然后按“选择” 。 请注意“组”旁边的文本是如何更新以反映已选择的 1 个组的。  

    1. 在“角色”旁边，选择“用户”。 此时将显示目录角色列表。  向下滚动以查看各种内置角色、查看各种角色，但不要更改用户角色。  选择页面右上角的“X”关闭此窗口。

1. 配置**设置**

    1. 阻止登录：否（保留默认设置）。

    1. 使用位置：选择下拉列表，然后选择美国（向下滚动以查找此选项）或所在国家/地区。  分配许可证需要配置使用位置。

1. 在页面底部，选择“创建”按钮。

1. 验证用户是否显示在用户列表中（名称按字母顺序列出），可能需要刷新浏览器页面。

1. 从用户列表中选择刚刚创建的用户 Sara Perez。  此时将打开个人资料页。

1. 左侧导航面板显示可为用户配置的各种选项。  选择“组”。  可在此处看到有关该组的其他信息。  验证是否列出了“操作”组（可能需要几分钟时间才会显示组分配）。  注意：你还将看到 Contoso 组，尽管我们在创建用户时只分配了一个组，。  这由租户中的预配置策略所致，该策略自动将新用户分配给 Contoso 组。

1. 在左侧导航面板中，选择“许可证”。  请注意，找不到此用户的许可证分配。  

1. 若要添加许可证，请在主窗口顶部选择“+ 分配”。

1. 在“选择许可证”下，选择“Office 365 E3”和“Windows 10/11 Enterprise E3”，然后选择屏幕底部的“保存”按钮  。 屏幕右上角的通知应显示许可证分配成功。

1. 选择屏幕右上角的“X”关闭“许可证分配”窗口。

1. 选择页面顶部的“刷新”图标确认许可证分配。

1. 通过选择屏幕左上方（面包屑）的“Contoso”（其上显示“Sara Perez | 许可证”），返回 Contoso 概述 Azure Active Directory 页面。

1. 你已在 Azure Active Directory 中成功创建并配置用户。

1. 退出所有打开的浏览器选项卡。  在 Azure 门户中，通过选择屏幕右上角电子邮件地址旁边的用户图标，然后选择“退出”来退出。在 Microsoft 365 中，选择 Microsoft 365 窗口右上角的图标，该图标显示为包含字母 SP 的圆圈（在问号图标旁），然后选择“退出”。关闭所有浏览器窗口 。

### <a name="task-3"></a>任务 3

在本任务中，你将以 Sara Perez 的身份完成首次登录。

1. 打开 Microsoft Edge。

2. 在地址栏中，输入 login.microsoft.com。

3. 以 sara@WWLxZZZZZ.onmicrosoft.com 身份登录（其中 ZZZZZZ 是实验室托管提供商提供的唯一租户 ID）。

4. 输入临时密码 Naja8996。

5. 现在，系统会提示你更新密码。 在“当前密码”字段中，输入 Naja8996。

6. 在“新密码”字段中输入 SC900-Lab。  在“确认密码”字段中输入 SC900-Lab，然后选择“登录”。  注意：最佳做法是，应使用更安全的密码。 选择此密码是出于方便考虑，并且仅用于本实验室目的。

7. 现在你应成功登录 Microsoft 365。

8. 通过选择“Microsoft 365”窗口右上角的图标退出，该图标显示为包含字母 SP 的圆圈（在问号图标旁），然后选择“退出”并关闭浏览器。

### <a name="review"></a>审阅

在本实验室中，你开始了对 Azure AD 的初步探索。 由于 Microsoft 365 的订阅者自动使用 Azure AD，你发现你可以通过 Microsoft 365 管理门户或 Azure 门户访问 Azure AD 功能和服务。  无论使用哪种方法，都会到达相同的位置。  你还演练了创建新用户以及可以配置的不同设置的过程，包括可以将用户分配到的组、角色的可用性以及用户许可证的分配。
