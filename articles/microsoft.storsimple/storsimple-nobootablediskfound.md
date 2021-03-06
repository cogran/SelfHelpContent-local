<properties
    pageTitle="My virtual array doesn't boot up."
    description="虚拟阵列无法启动。"
    service="microsoft.storsimple"
    resource="managers"
    authors="anbacker"
    displayOrder="2"
    selfHelpType="resource"
    supportTopicIds=""
    resourceTags="9000Or1200Series"
    productPesIds=""
    cloudEnvironments="public"
/>


# <a name="my-virtual-array-doesnt-boot-up"></a>虚拟阵列无法启动。
如果无法启动预配的虚拟阵列，请检查所用的虚拟磁盘映像版本。 <br>
常见错误消息： <br>
    1. `Boot failure. Reboot and Select proper Boot device`。<br>
    2. `Insert Boot Media in selected Boot device`。

## <a name="recommended-steps"></a>**建议的步骤**
* 如果使用适用于 Windows Server 2008 R2 或更高版本的 VHD，则需要创建**第 1 代** VM。
* 如果使用适用于 Windows Server 2012 或更高版本的 VHDX，则需要创建**第 2 代** VM。


## <a name="recommended-documents"></a>**建议的文档**
[在 Hyper-V 中预配虚拟阵列。](https://aka.ms/storsimple-troubleshoot-provisionarray)<br>
[适用于 Hyper-V 2008 R2 和更高版本的 VHD](https://go.microsoft.com/fwLink/?LinkID=692085&clcid=0x409)<br>
[适用于 Hyper-V 2012 和更高版本的 VHDX](https://go.microsoft.com/fwLink/?LinkID=724278&clcid=0x409)<br>
[第 2 代虚拟机概述](https://technet.microsoft.com/library/dn282285.aspx)

