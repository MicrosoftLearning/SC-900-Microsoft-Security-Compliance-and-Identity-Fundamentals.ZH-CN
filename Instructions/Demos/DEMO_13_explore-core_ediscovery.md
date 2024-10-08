<!---
---
演示：标题：“探索电子数据展示”学习路径/模块/单元：“学习路径：介绍 Microsoft Priva 和 Microsoft Purview 的功能；模块 3：介绍 Microsoft Purview 的数据合规性解决方案；单元 2：介绍电子数据展示”
---
--->

# 演示：探索电子数据展示（标准版）

此演示与下列 Learn 内容保持一致：

- 学习路径：介绍 Microsoft Priva 和 Microsoft Purview 的功能
- 模块：介绍 Microsoft Purview 的数据合规性解决方案
- 单元：介绍电子数据展示

## 演示方案

在本演示中，你将演示设置电子数据展示所需的步骤，包括设置角色权限、创建电子数据展示案例、创建电子数据展示保留和创建搜索查询。  备注：在 Microsoft Purview 门户中，对用户界面的更新正在逐步推出。 某些实验室/演示租户可能尚未显示最新的 UI，因此所有实验室步骤均使用经典电子数据展示 UI 来展示。

### 演示第 1 部分

如果某个用户想要访问电子数据展示（标准版）或者想要成为电子数据展示案件的成员，则必须获得相应的权限。 在演示的此部分，你作为全局管理员将逐步完成将特定用户添加为电子数据展示管理器角色组成员的过程。

1. 打开 **Microsoft Purview** 的浏览器选项卡。 如果之前已关闭，请打开浏览器选项卡，并在地址栏中输入 **https://purview.microsoft.com**。 若要访问新的 Microsoft Purview 门户，请选择“**我同意数据流披露条款和隐私声明**”旁边的框，然后选择“**开始**”。  
1. 从左侧导航面板中，选择“**设置**”。
1. 在打开的导航面板中，选择“**角色和范围**”以展开选项，然后选择“**角色组**”。
1. 在屏幕右侧的搜索框中，搜索术语“**电子数据展示**”。  选择“**电子数据展示管理器**”。
    1. 选择“编辑”  。
    1. 选择“**选择用户**”。
    1. 搜索 MOD 管理员，选择“**MOD 管理员**”旁边的框，然后选择页面底部的“**选择**”按钮。
    1. 选择“**下一步**”，然后选择“**保存**”，最后选择“**完成**”。

1. 将此浏览器选项卡保持打开状态。

### 演示第 2 部分

在本部分中，你将创建一个案例以开始使用电子数据展示（标准版）。

1. 在左侧导航面板中，选择“**解决方案**”，选择“**电子数据展示**”，然后选择“**标准案例**”。

1. 从“电子数据展示(标准版)”页面的顶部，选择“**+ 创建案件**”。

1. 在新建案例窗口中，输入案例名称 **SC900 测试案例**，然后选择页面底部的**保存**。

1. 现在，该案例应出现在列表中。

1. 作为该案例的创建者，由于您拥有电子数据展示管理员权限，因此可以开始使用该案例。  

1. 将此浏览器选项卡保持打开状态。

### 演示第 3 部分

现在你已创建电子数据展示（标准版）案例，可以开始处理该案例。  在此部分中，你将为创建的案例创建电子数据展示保留。  具体来说，你将为属于 Adele Vance 的 Exchange 邮箱创建保留。

1. 从“电子数据展示(标准版)”页面，选择在前一个选项卡中创建的案例 -“**SC900 测试案例**”。

1. 在案例的主页上，选择**保持**选项卡，然后选择 **+创建**。

1. 在“名称”字段中，输入“**测试保留**”，然后选择“**下一步**”。

1. 在“选择位置”页面中，选择“**Exchange 邮箱**”旁边的切换开关以将状态设置为“**开启**”。  

1. 现在选择“**选择用户、组或团队**”。  在搜索框中输入 **Adele**，然后按键盘上的回车键。 从搜索结果中选择“**Adele Vance**”，然后选择“**完成**”。

1. 在选择位置页面，选择**下一步**。  为了演示的方便，此保留中不包含其他位置。

1. 通过“查询条件”页面，可以根据满足需求的特定关键字或条件创建保留，选择“**+ 添加条件**”以查看可用选项。  选择**下一步**。 在不附加任何条件的情况下，保留将保留指定位置的所有内容。

1. 查看设置并选择**提交**，可能需要一分钟，然后选择**完成**。  测试保留应出现在列表中。  如果没有立即看到，请选择**刷新**。

1. 将此浏览器选项卡保持打开状态。

### 演示第 4 部分

设置好保留后，你将创建一个搜索查询。  电子数据展示在搜索完成后执行相关操作，例如导出和下载结果以供将来调查。   注意：与电子数据展示（标准）案件相关的搜索不会在 Microsoft Purview 合规性门户网站的内容搜索页面上列出。 这些搜索仅列在相关电子数据展示（标准版）案件的“搜索”页上。

1. 在“SC900 测试案例”页中，选择“**搜索**”。

1. 从搜索页面，选择 **+ 新建搜索**。

1. 在名称字段中，输入**测试保留 - 销售搜索**，然后从页面底部选择**下一步**。

1. 在“选择位置”页面，选择“**保留的位置**”，取消选择“**为本地用户添加应用内容**”（因为实验室环境没有本地用户），然后选择“**下一步**”。

1. 查询条件页面使您能够根据特定的关键字或满足的条件创建搜索，在关键字字段中输入**销售**，选择**下一步**。

1. 查看设置并选择**提交**，可能需要一分钟，然后选择**完成**。  搜索结果应出现在列表中。  如果没有立即看到，请选择**刷新**。

1. 从“搜索”窗口中，选择创建的搜索“**测试保留 - 销售搜索**”。  打开一个窗口，选择摘要选项卡。  搜索完成后，状态将指示搜索已完成。  你将看到“搜索统计信息”选项卡（如果没有看到“搜索统计信息”选项卡，则搜索可能仍在运行，并且可能需要几分钟才能完成）。  选择“**搜索统计信息**”选项卡，然后选择搜索内容旁边的向下箭头。  您还可以查看状况报告和热门位置的更多信息。  

1. 从页面底部选择**操作**。  请注意包含导出选项的可用选项。 选择**关闭**。

1. 关闭所有打开的浏览器选项卡。

### 审阅

在本演示中，你完成了开始使用电子数据展示（标准版）所需的步骤，包括设置电子数据展示的角色权限和创建电子数据展示案例。  通过处理创建的案例，你演练了电子数据展示（标准版）工作流中的环节（创建电子数据展示保留以及创建搜索查询）。
