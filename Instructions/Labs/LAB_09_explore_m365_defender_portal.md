---
lab:
  title: 探索 Microsoft Defender 门户
  module: Describe the threat protection capabilities of Microsoft XDR
---

# 实验室：探索 Microsoft Defender 门户

此实验室与下列 Learn 内容保持一致：

- 学习路径：描述 Microsoft 安全解决方案的功能
- 模块：介绍 Microsoft Defender XDR 的威胁防护功能
- 单元：介绍 Microsoft Defender 门户

## 实验室方案

在本实验室中，你将通过演练登陆页面上显示的内容来探索 Microsoft Defender 门户。 你还将探索导航面板上的选项，这些选项提供对 Microsoft 扩展检测和响应 (XDR) 解决方案一部分功能的快速访问：Microsoft Defender for Endpoint 和 Microsoft Defender for Office 365（电子邮件和协作）。  最后，你还将探索 Microsoft 安全功能分数如何帮助组织提高其安全状况。

**预计用时**：30 分钟

### 任务 1

浏览 Microsoft Defender 登陆页面。

1. 打开 Microsoft Edge。 在地址栏中，输入“**admin.microsoft.com**”。

1. 使用管理员凭据登录。
    1. 在“登录”窗口中，输入 **admin@WWLxZZZZZZ.onmicrosoft.com**（其中 ZZZZZZ 是实验室托管提供商提供的唯一租户 ID），然后选择“**下一步**”。
    1. 输入管理员密码，该密码由实验室托管提供商提供。 选择“**登录**”。
    1. 如果你是首次登录到租户，系统可能会提示你完成 MFA 注册流程，具体取决于实验室主机托管服务提供商。 如果出现提示，则按照屏幕上的提示设置 MFA。
    1. 登录后，你将进入 Microsoft 365 管理中心页。

1. 从 Microsoft 365 管理中心的左侧导航窗格中，在“管理中心”下选择“**安全性**”。  如果未列出“安全性”，请选择“**全部显示**”，然后选择“**安全性**”。  打开一个新的浏览器页，进入 Microsoft Defender 门户的欢迎页。  

1. 如果你是第一次访问 Microsoft 365 Defender 门户，可能会出现一个弹出窗口，帮助你快速浏览。  你可以选择快速浏览或关闭窗口。

1. Microsoft Defender 门户的主页显示安全团队所需的许多常见卡片。 卡片和数据的组成取决于用户的角色。 滚动页面，查看您作为全局管理员角色的默认卡片集。

1. 显示的卡片可根据您的偏好进行自定义。  选择 **+ 添加卡片**。 此时会打开一个窗口，显示可添加到主页的卡片。  你可能已显示所有卡片，在这种情况下，会显示提示“主页上已显示所有卡片。” 选择窗口右上角的 **X** 关闭窗口。

1. 选择任何卡片右上角的省略号将提供从登陆页面删除卡片的选项。  

1. 您还可以移动卡片。 将鼠标光标悬停在任意卡片的标题栏上，出现一个十字形光标时，选择该卡片并将其移动到所需位置。  

1. 某些卡片的底部有可选择的按钮。 某些卡片的标题用作该主题页面的链接。  例如，如果选择“Microsoft 安全功能分数卡”标题，则会将你带到“Microsoft 安全功能分数”页。  在本演示的后续部分中，你将详细了解 Microsoft 安全功能分数。

1. 保持浏览器窗口打开。

### 任务 2

在实验室的这部分，你将了解 Defender 门户左侧导航面板中提供的一些选项。  通过 Microsoft Defender 门户，Microsoft 兑现了提供统一安全运营平台的承诺。 Microsoft Defender 门户在一个中心位置整合了防范、检测、调查和响应整个组织及其所有组件面临的威胁的功能。  

1. 随时浏览左侧导航面板。

1. 要返回 Microsoft Defender 门户的主页，请选择左侧导航面板上的“**主页**”。

### 任务 3

在此任务中，你将探索 Microsoft 安全功能分数如何帮助组织提高其安全状况。

1. 你应仍在 Microsoft Defender 门户中。 从左侧导航面板中展开“**风险管理**”，然后选择“**安全功能分数**”。  如果租户中未显示“风险管理”，则从 Microsoft Defender 门户的“欢迎”页向下滚动，直到看到“**Microsoft 安全功能分数**”卡。 选择卡的标题（将鼠标光标悬停在卡标题上时，文本将变为蓝色）。

1. 这会打开“Microsoft 安全功能分数”页面，显示“概述”选项卡。Microsoft 安全功能分数是针对组织安全状况的一种衡量标准。 组织的安全功能分数以百分比形式显示，同时显示在可能的总分中已取得的分数，并按类别进行细分。 选择“你的安全功能分数”旁边的“**包含**”。  将打开一个小窗口，用于将可实现的分数、计划内分数和当前许可证分数包括在组织安全分数的明细中。  再次选择“**包含**”以关闭窗口。

1. 概览页面还包括顶级改进操作、比较得分、历史记录和其他资源。

1. 选择页面顶部的“**改进操作**”。  请注意表中提供的信息。  

1. 选择列表中的第一项，然后查看可查看的信息。 请在打开的窗口中观察可用的状态选项。 选择要查看的“**实现**”选项卡，查看与实现相关的信息。 单击右上角的“**X**”以关闭此窗口。

1. 从页面顶部选择**历史记录**选项卡。  对于列出的每个活动，都有一句介绍上下文的简短说明。  在历史记录表中选择一个项。  在详细信息页面右上方的历史记录下，选择** X 事件**（其中 X 为数字）。  这会打开“操作历史记录”窗口，并提供详细信息。  选择页面底部的**关闭**，然后选择详细信息页面右上角的 **X** 返回历史记录页面。

1. 从页面顶部选择**指标和趋势**。  注意可用信息。  从页面右上角选择**日历图标**。  您可以将视图缩小到自定义日期范围。  通过选择**筛选图标**可按标识和/或应用筛选视图中的内容。  关闭窗口，从左侧导航面板选择“**主页**”，返回 Microsoft Defender 主页。

1. 关闭所有打开的浏览器选项卡。

### 审阅

在本实验室中，你通过演练登陆页面上显示的内容探索了 Microsoft Defender 门户，也探索了导航面板上的选项，这些选项可用于快速访问 Microsoft 的扩展检测和响应 (XDR) 解决方案、Microsoft Defender for Endpoints 和 Microsoft Defender for Office 365（电子邮件和协作）中的部分功能。  最后，您将了解 Microsoft Secure Score 如何帮助组织改善其安全状况。
