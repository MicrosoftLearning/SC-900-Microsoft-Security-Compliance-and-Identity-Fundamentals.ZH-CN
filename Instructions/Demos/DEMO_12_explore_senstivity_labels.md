<!---
---
Demo: Title: 'Sensitivity labels in Microsoft Purview' Learning Path/Module/Unit: '学习路径：描述 Microsoft 合规性功能；模块 3：描述 Microsoft Purview 中的信息保护、数据生命周期管理和数据治理功能；第 4 单元：描述敏感度标签'
---
--->

# 演示：Microsoft Purview 中的灵敏度标签

此演示与下列 Learn 内容保持一致：

- 学习路径：描述 Microsoft 合规性功能
- 模块：介绍 Microsoft Purview 中的信息保护、数据生命周期管理和数据治理功能
- 单元：描述敏感度标签

## 演示方案

在本演示中，你将展示敏感度标签的功能。  你将完成已创建的现有敏感度标签以及发布标签的相应策略的设置。   然后，你将从用户的角度了解如何应用标签以及标签的作用。  **注意**：第一次使用 Microsoft 365 租户在线 Word 时，敏感性选项可能需要 15 分钟才能出现在功能区中。  演示者应在课前运行演示第 2 部分，以确保有足够的时间显示选项。

### 演示第 1 部分

在本演示中，你将展示现有敏感度标签以及发布标签的相应策略的设置。

1. 打开 Microsoft Purview 主页的浏览器选项卡。  如果你之前关闭了它，请打开一个浏览器选项卡，然后输入**https://admin.microsoft.com**。 使用授权实验室托管者 (ALH) 提供的 Microsoft 365 租户的管理员凭据登录。 从 Microsoft 365 管理中心的左侧导航窗格，选择“**全部显示**”，然后选择“**合规性**”。  这会打开一个新的浏览器页面，显示 Microsoft Purview 合规性门户的欢迎页。  

1. 在左侧导航面板的“解决方案”下，展开“**信息保护**”，然后选择“**概述**”。  在概述页面中，可查看应用于内容的热门敏感度标签、检测到的热门活动、应用敏感度标签的位置等信息。  
    1. 在概述页面中，你会看到黄色的信息框，它表示你的组织尚未开启处理 Office 在线文件（已应用加密的敏感度标签且存储在 OneDrive 和 SharePoint 中）中的内容的功能。  选择“**立即开启**”。  执行此操作后，设置在系统中传播可能存在延迟。

1. 在左侧导航面板中，选择“**标签**”。

1. 为了方便起见，某些标签已在你的 Microsoft 365 实验室租户中预配置。 选择名为**机密-财务**的标签。  此时会打开一个窗口，其中提供关于此标签的信息。  注意该标签的设置。  选择页面顶部的“编辑”标签（也可能显示为铅笔图标）以查看一些基本配置设置。**** 如果未看到此选项，请选择省略号。
    1. 配置的第一步是为标签提供一个名称和描述。  请勿更改任何内容。  选择页面底部的“**下一步**”。
    1. 查看此标签的范围。 请勿更改任何内容。  选择页面底部的“**下一步**”。
    1. 在下一个屏幕中，你可以为标记的项选择保护设置。 此标签已配置为支持内容标记。 请勿更改任何内容。  选择页面底部的“**下一步**”。
        1. 在“内容标记”页面中，记下页面顶部的信息框中的内容。  请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 现在您正处于“文件和电子邮件自动标记”窗口。  阅读页面顶部的自动加标签的描述及其下方的信息框。  另请记住，此标签设置为在特定条件下自动加标签。 请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 此窗口为应用此标签的团队、组和站点定义保护设置。 这处于未启用状态，选择页面底部的“**下一步**”。
    1. 此窗口是一项预览功能，它能够自动将此标签应用到 Microsoft Purview 数据映射中包含你所选敏感信息类型的架构化数据资产（例如 SQL、Synapse 等）。  此功能未启用。 选择页面底部的“**取消**”以退出标签配置向导，并返回“信息保护”页面。

1. 在左侧导航面板中，选择“**标签策略**”。  需通过标签策略发布敏感度标签。  为方便起见，Microsoft 365 租户已配置了一些标签策略。

1. 选择**机密-财务**策略。  此时会打开一个窗口，其中提供关于此策略的信息。 选择窗口顶部的“**编辑策略**”。  在此，您无需更改任何设置。
    1. 查看“选择要发布的敏感度标签”的说明。  请注意已列出的标签。  请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 查看“分配管理单元”的说明。 管理单元设置为完整目录，不要更改任何设置。 选择**下一步**。  
    1. 查看“发布到用户和组”的说明。  请注意，此标签适用于所有用户。  请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 查看策略设置。 请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 查看“将默认标签应用于文档”的说明。 请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 查看“将默认标签应用于电子邮件”和“从附件继承标签”的说明。 请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 查看“将默认标签应用于会议和日历事件”的说明。 请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 查看“将默认标签应用于 Power BI 内容”的说明。 请勿更改任何设置。  选择页面底部的“**下一步**”。
    1. 最后一个配置选项是为策略命名。  因为正在编辑策略，所以名称字段处于灰显状态。选择页面底部的“**下一步**”。
    1. 查看策略设置。 选择“**取消**”以放弃任何更改并返回到“标签策略”页。

1. 在左侧导航面板中的信息保护下，选择“自动标记”。 查看说明。 请注意，你要创建自动标记策略以自动将敏感度标签应用于包含敏感信息的电子邮件或 OneDrive 和 SharePoint 文件。 如果配置了自动标记策略，请选择一个策略，并在详细信息窗格中查看策略信息。  如果未列出任何策略，可以选择演练创建策略的步骤（如果时间允许）。

1. 从左侧导航面板选择“主页”以返回 Microsoft Purview 合规性门户。

1. 将此浏览器选项卡保持打开状态。

### 演示第 2 部分

在此步骤中，你将演示从用户角度应用标签的过程（在本例中，用户是管理员）。  为了查看应用标签的影响，你将选择“机密 - 财务”标签，因为此标签应用了水印。

1. 从 Microsoft Purview 合规性门户主页中，选择“Contoso Electronics”旁边的“**应用启动器**”图标。 选择 **Word 图标**。  

1. 选择“**空白文档**”，然后在页面中输入一些文本。  在页面顶部的蓝色栏上，选择“文档 - 已保存”旁边的向下箭头，然后用键盘在“文件名”框中输入“**Test-label**”、按下“**Enter**”键。

1. 顶部菜单栏最右侧（也称为功能区）有一个向下箭头，选择它，然后选择“经典功能区”。****  这样可以更便捷地标识敏感度图标。 选择麦克风图标旁边的“敏感度”。**** 从下拉菜单选择“机密 - 财务”****。  

1. 从顶部菜单栏选项“**查看**”，然后选择“**阅读视图**”。

1. 请注意文档包含水印的方式。  

1. 关闭浏览器中打开的 Microsoft Word 选项卡以退出 Word。

1. 使 Microsoft Purview 浏览器选项卡保持打开状态，以供下一个演示使用。

### 审阅

在此演示中，你演示了可为敏感度标签配置的设置，以及发布敏感度标签的策略的设置。 您还将看到如何应用标签。
