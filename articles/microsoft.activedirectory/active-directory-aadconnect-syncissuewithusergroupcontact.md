<properties
    pageTitle="Synchronization issue with specific user, group or contact object"
    description="与特定用户、组或联系人对象同步的问题"
    service="microsoft.activedirectory"
    resource="activedirectory"
    authors="cychua"
    displayOrder=""
    selfHelpType="generic"
    supportTopicIds="32570979"
    resourceTags=""
    productPesIds="14785"
    cloudEnvironments="public"
/>


# <a name="synchronization-issue-with-specific-user-group-or-contact-object"></a>与特定用户、组或联系人对象同步的问题

## <a name="recommended-steps"></a>建议的步骤

**同步特定用户、组或联系人对象的问题**

如果同步特定的对象时遇到问题：

  * 检查对应于此对象的任何同步错误。 有关常见同步错误的详细信息，请参阅[排查同步过程中发生的错误](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-troubleshoot-sync-errors)一文。 将通过以下方式向客户显示同步错误：
  
    * 通过 Azure AD Connect Health 的[对象级同步错误报告](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-sync)。 目前只会向选定的客户显示这些错误。
    
    * 标识同步错误报告 - 每当 Azure AD Connect 完成同步周期但出错时，就会向租户的技术通知联系人发送此电子邮件通知。
    
    * 通过[同步服务管理器的“操作”选项卡](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-service-manager-ui-operations)。
    
  * 在 [重复属性复原](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-duplicate-attribute-resiliency) 功能下检查重复属性错误。

  * 如果未发现此对象的任何错误，请遵循[排查对象无法同步到 Azure AD 的问题](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-object-not-syncing)一文中所述的故障排除步骤。

