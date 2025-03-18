---
lab:
  title: 实验室设置
  module: Setup your Microsoft 365 lab tenant (not associated with a Learn module)
---

# 实验室：Microsoft 365 租户的设置

## WWL 租户 - 使用条款
如果在讲师引导式培训过程中向你提供租户，请注意，提供租户旨在支持讲师引导式培训中的动手实验室。

租户不应共享或用于动手实验室以外的用途。 本课程使用的租户为试用租户，课程结束后无法使用或访问，不符合扩展条件。

租户不得转换为付费订阅。 在本课程中获得的租户仍然是 Microsoft Corporation 的财产，我们保留随时获取访问权限和收回的权利。

## 实验室方案

此设置实验室包括在 Microsoft 365 租户中启用 Microsoft 审核日志和文件监视功能。

**预计用时**：5-10 分钟

### 设置 - 启用 Microsoft 365 审核日志和文件监视

在此设置任务中，你将在 Microsoft 365 中启用审核日志和文件监视功能。  

1. 打开 Microsoft Edge。 在地址栏中输入**`https://admin.microsoft.com`**。

1. 使用授权实验室托管者 (ALH) 提供的 Microsoft 365 租户的管理员凭据登录。

1. 从 Microsoft 365 管理中心的左侧导航窗格中，选择“**全部显示**”。

1. 在管理中心下，选择“**安全性**”。  打开一个新的浏览器页，进入 Microsoft Defender 的欢迎页。

1. 在左侧导航面板中，向下滚动并展开“**系统**”。  从展开的列表中，选择“**审核**”。  备注：还可通过 Microsoft Purview 门户访问审核功能。

1. 进入审核页面后，请等待 1-2 分钟。  如果未启用“审核”，你将在页面顶部看到一个显示“开始记录用户和管理员活动”的蓝条。  选择**开始记录用户和管理员活动**。  启用审计后，蓝色条将消失。  如果蓝条不存在，则表示已启用审核，无需采取进一步操作。  如果看到一条消息，“很抱歉，我们很难确定是否正在记录活动。 尝试刷新页面，“刷新页面后没有更改，需要通过 PowerShell 启用审核。
    1. 右键选择任务栏上的蓝色“Windows PowerShell”图标，然后选择“**以管理员身份运行**”。
    1. 要确认计算机上安装了 Exchange Online PowerShell 模块，请输入 **`Get-InstalledModule ExchangeOnlineManagement | Format-List Name,Version,InstalledLocation`**。  你将看到 Exchange OnlineManagement 的名称、版本和安装位置。
    1. 现在，通过输入 **`Import-Module ExchangeOnlineManagement`** 来加载模块。
    1. 要连接，请输入 **`Connect-ExchangeOnline -UserPrincipalName admin@WWLxZZZZZZ.onmicrosoft.com`**。  对于 UPN，请输入在实验室的资源选项卡中找到的管理员用户名。
    1. 将提示您登录。  输入在实验室的资源选项卡中找到的管理用户名和密码。
    1. 要打开审核功能，请输入 **`Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true`**。 将显示一条消息，指出更改可能需要长达 60 分钟才能生效。
    1. 尽管可能需要长达 60 分钟才能生效，但可以通过输入 **`Get-AdminAuditLogConfig | FL UnifiedAuditLogIngestionEnabled`** 来验证命令是否已收到。  如果启用了审核，则属性 UnifiedAuditLogIngestionEnabled 将显示 true 值。

1. 从左侧导航面板的“系统”下，选择“**设置**”。

1. 在“设置”页面中，选择“**云应用**”。   向下滚动，然后在“**信息保护**”下选择“**文件**”。

1. 如果尚未启用，请选择“**启用文件监视**”旁边的框，然后选择“**保存**”。  

1. Microsoft 365 租户上的实验室设置到此结束。

### 审阅

在此设置中，你在 Microsoft 365 中启用了审核日志和文件监视功能。
