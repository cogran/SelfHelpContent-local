<properties
    pageTitle="I can't delete my classic storage account"
    description="无法删除经典存储帐户"
    service="microsoft.classicstorage"
    resource="storageaccounts"
    authors="passaree"
    displayOrder="1"
    selfHelpType="resource"
    supportTopicIds="32551644,32551656,32551657,32551665"
    resourceTags=""
    productPesIds="15629"
    cloudEnvironments="public"
/>


# <a name="i-cant-delete-my-classic-storage-account"></a>无法删除经典存储帐户

## <a name="recommended-steps"></a>**建议的步骤**
当你尝试在 Azure 门户或 Azure 经典门户中删除 Azure 存储帐户、容器或 VHD 时，可能会收到错误。 这些问题可能是由以下情况造成的：<br>

- 当你删除 VM 时，磁盘和 VHD 未自动删除。 这可能是存储帐户删除失败的原因。 我们不会删除磁盘，以便你可以使用该磁盘装入另一个 VM。<br>
- 磁盘或者与磁盘关联的 Blob 上仍有租约。<br>

如果存储帐户使用经典部署模型，你可以通过执行以下步骤来删除虚拟机磁盘：

1. 导航到 [Azure 经典门户](https://manage.windowsazure.com/)
2. 选择“虚拟机”>“磁盘”。
3. 找到与你想要删除的存储帐户、容器或 VHD 关联的磁盘。 通过检查磁盘的位置，你将会找到关联的存储帐户、容器或 VHD。
4. 选择你的数据磁盘，然后单击“删除磁盘”。
5. 若要删除磁盘映像，请导航到“映像”选项卡，然后删除存储在帐户中的任何映像。

## <a name="recommended-documents"></a>**建议的文档**
[删除经典存储帐户时出现问题](http://go.microsoft.com/fwlink/?LinkId=785085)



<!--HONumber=Nov16_HO4-->


