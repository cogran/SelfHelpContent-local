<properties
    pageTitle="VMA RCA"
    description="RCA 节点重新启动 - bug 检查网络驱动程序 - 无服务修复"
    infoBubbleText="发现最近已重新启动。 请参阅右侧的详细信息。"
    service="microsoft.compute"
    resource="virtualmachines"
    authors="jozender"
    displayOrder=""
    articleId="UnexpectedVMReboot_CD44E20E-947F-4E01-B197-3907ABEA0974"
    diagnosticScenario="UnexpectedVMReboot"
    selfHelpType="rca"
    supportTopicIds="32411816"
    resourceTags="windows, linux"
    productPesIds="14749"
    cloudEnvironments="public"
/>

# <a name="we-ran-diagnostics-on-your-resource-and-found-an-issue"></a>我们对你的资源运行了诊断并发现了问题
 
<!--issueDescription-->
## <a name="vm-availability-incident-diagnostic-information-for---vmname--virtual-machine--vmname--"></a>**<!--$vmname-->虚拟机<!--/$vmname-->的 VM 可用性事件诊断信息：** ##

我们发现，你的 VM 在 **<!--$StartTime--> StartTime <!--/$StartTime--> (UTC)** 变得不可用，在 **<!--$EndTime--> EndTime <!--/$EndTime--> (UTC)** 恢复了可用性。 此意外事件是 **Azure 启动的主机节点重新启动操作**所致。
<!--/issueDescription-->

该主机节点重新启动操作由 Azure 监视系统触发，这些系统检测到托管虚拟机的物理节点上存在驱动程序故障情况。 这也导致了你的 VM 重新启动。 在此时间内，与 VM 的 RDP 连接或对该 VM 内运行的任何其他服务的请求可能已失败。 
 
我们的核心平台工程师已识别出该 Bug，并且当前正在致力于提供解决此问题的修补程序。 该解决方案在经过验证并完成测试后将会部署到所有受影响的节点。  

为了确保提高 Azure 中应用程序的保护和冗余级别，我们建议将两个或更多虚拟机组合到一个可用性集中。<br>
若要了解有关高可用性选项的详细信息，请参阅以下文章：<br>
* [管理虚拟机的可用性](https://azure.microsoft.com/documentation/articles/virtual-machines-manage-availability)<br>
* [配置虚拟机的可用性](https://azure.microsoft.com/documentation/articles/virtual-machines-how-to-configure-availability)<br>

Microsoft Azure 还可让你在 Azure 门户中访问资源运行状况和故障排除信息。<br>
若要了解有关 Azure 资源运行状况的详细信息，请参阅以下文章：<br>
* [了解资源运行状况中心并使用它来排查此方案将来出现的问题](https://docs.microsoft.com/azure/resource-health/resource-health-overview)

对于这可能给你带来的任何不便，我们深表歉意。 我们一直致力于改进该平台，以减少由于平台问题而导致的虚拟机可用性事件。

