<properties 
    pageTitle="I can't create a new DNS zone"
    description="无法在 Azure DNS 服务中创建新 DNS 区域。"
    service="microsoft.network"
    resource="dnszones"
    authors="jtuliani"
    displayOrder="1"
    selfHelpType="resource"
    supportTopicIds=""
    productPesIds=""
    resourceTags=""
    cloudEnvironments="public"
/>


# <a name="i-cant-create-a-new-dns-zone"></a>无法创建新的 DNS 区域

## <a name="recommended-steps"></a>**建议的步骤**

若要解决常见问题，请尝试下面的一个或多个步骤：

1.  查看[审核日志](data-blade:Microsoft_Azure_Insights.AzureDiagnosticsBladeWithParameter)以确定失败原因。
2.  每个 DNS 区域名称在其资源组中必须唯一。 即，一个资源组中不能具有名称相同的两个 DNS 区域。 请尝试使用不同的区域名称，或采用不同的资源组。
3.  如果出现错误：“已达到或超过订阅 {subscription id} 中最大区域数”，则请使用不同 Azure 订阅，删除一些区域，或联系 Azure 支持以提高订阅上限，然后重试。
4.  如果出现错误：“区域 '{zone name} 不可用”，则表示 Azure DNS 无法为此 DNS 区域分配名称服务器。 请尝试使用不同的区域名称。 或者，如果你是该域名的所有者，请联系 Azure 支持为你分配名称服务器。

如果上述步骤未解决该问题，请将此问题发布到 [MSDN 上的社区支持论坛](https://social.msdn.microsoft.com/Forums/en-US/home?forum=WAVirtualMachinesVirtualNetwork)或打开 Azure 支持票证。

## <a name="recommended-documents"></a>**建议的文档**

[DNS zones and records](https://docs.microsoft.com/azure/dns/dns-zones-records)
（DNS 区域和记录）<br>
[创建 DNS 区域](https://docs.microsoft.com/azure/dns/dns-getstarted-create-dnszone-portal)



<!--HONumber=Dec16_HO1-->

