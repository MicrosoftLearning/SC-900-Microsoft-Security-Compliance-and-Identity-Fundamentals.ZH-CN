<a name="---"></a><!---
---
Lab: Title: '设置'
---
--->

# <a name="lab-setup"></a>实验室：设置

## <a name="lab-scenario"></a>实验室场景

此设置实验室包括启用 Microsoft 审核日志。

预计用时：5-10 分钟

### <a name="setup---enable-microsoft-365-audit-log"></a>设置 - 启用 Microsoft 365 审核日志

在此设置任务中，你将在 Microsoft 365 中启用审核日志功能。  虽然文档表明审核日志在默认情况下为打开状态，但大多数实验室租户未启用此功能，并且此功能可能需要几个小时才会生效。  启用此功能很有帮助，因为 Microsoft 365 使用审核日志来获取策略和分析见解中确定的用户见解和活动。

1. 打开 Microsoft Edge。 在地址栏中，输入“admin.microsoft.com”。

1. 使用管理员凭据登录。
    1. 在“登录”窗口中，输入 admin@WWLxZZZZZZ.onmicrosoft.com（其中 ZZZZZZ 是实验室托管提供商提供的唯一租户 ID），然后选择“下一步” 。
    1. 输入管理员密码，该密码应由实验室托管提供商提供。 选择“登录”。
    1. 在提示保持登录状态时，选择“是”。 这将使你进入 Microsoft 365 管理中心页面。

1. 从 Microsoft 365 管理中心的左侧导航窗格中，选择“全部显示”。

1. 在管理中心下，选择“合规性”。  这会打开一个新的浏览器页面，显示 Microsoft 365 合规中心的欢迎页。  

1. 在左侧导航面板的解决方案下，选择“审核”。  备注：还可以通过 Microsoft 365 Defender 主页（以前称为 Microsoft 365 安全中心）访问审核功能。

1. 确认已选中“搜索”选项卡（带下划线）。

1. 登陆“审核”页面后，请等待 2-3 分钟。  如果未启用“审核”，你将在页面顶部看到一个显示“开始记录用户和管理员活动”的蓝条。  选择“开始记录用户和管理员活动”。  如果系统提示你确认需更新组织设置，请选择“是”。 启用审核后，蓝条将消失。  如果蓝条不存在，则表示已启用审核，无需采取进一步操作。  检查是否启用了审核的另一种方法是通过 PowerShell 进行检查，但这不在本课程的范围之中。

1. 通过选择左侧导航面板中的“主页”，返回 Microsoft 365 合规中心的主页。

### <a name="review"></a>审阅

在此设置中，你还在 Microsoft 365 中启用了审核日志功能。