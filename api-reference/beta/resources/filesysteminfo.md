---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
ms.openlocfilehash: e2dfac79f5c7d511cab11c076d697940a01f4c7c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524697"
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="bbee8-102">Аспект FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="bbee8-102">FileSystemInfo facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbee8-p101">Ресурс FileSystemInfo содержит свойства, которые отображаются в локальной файловой системе устройства для локальной версии элемента. Этот аспект можно использовать, чтобы указать последнюю дату изменения или создания элемента, какой она была на локальном устройстве.</span><span class="sxs-lookup"><span data-stu-id="bbee8-p101">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="bbee8-105">Он доступен в свойстве fileSystemInfo ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="bbee8-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbee8-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbee8-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a><span data-ttu-id="bbee8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbee8-107">Properties</span></span>

| <span data-ttu-id="bbee8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbee8-108">Property</span></span>                 | <span data-ttu-id="bbee8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bbee8-109">Type</span></span>           | <span data-ttu-id="bbee8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bbee8-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bbee8-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="bbee8-111">**createdDateTime**</span></span>      | <span data-ttu-id="bbee8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbee8-112">DateTimeOffset</span></span> | <span data-ttu-id="bbee8-113">Дата и время создания файла в клиентском устройстве в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bbee8-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="bbee8-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="bbee8-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="bbee8-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbee8-115">DateTimeOffset</span></span> | <span data-ttu-id="bbee8-p102">Дата и время последнего использования файла в формате UTC. Доступно только для списка последних файлов.</span><span class="sxs-lookup"><span data-stu-id="bbee8-p102">The UTC date and time the file was last accessed. Available for the [recent file list](../api/drive-recent.md) only.</span></span> |
| <span data-ttu-id="bbee8-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="bbee8-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="bbee8-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbee8-119">DateTimeOffset</span></span> | <span data-ttu-id="bbee8-120">Дата и время последнего изменения файла в клиентском устройстве в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bbee8-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="bbee8-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="bbee8-121">Notes</span></span>

<span data-ttu-id="bbee8-p103">Значения свойств createdDateTime и lastModifiedDateTime отличаются от этих же свойств ресурса DriveItem. В качестве значений для ресурса DriveItem выступают созданные или измененные дата и время, которые можно увидеть в службе. Значения, хранящиеся в ресурсе FileSystemInfo, предоставляются клиентом.</span><span class="sxs-lookup"><span data-stu-id="bbee8-p103">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource. The values on the DriveItem resource are the created and modified date and time as seen from the service. The values stored in the **FileSystemInfo** resource are provided by the client.</span></span>

<span data-ttu-id="bbee8-p104">Например, если файл был создан на устройстве в понедельник, но не загружен в службу до вторника, клиент, загружающий файл, должен прописать аспект `fileSystemInfo`включить дату создания в понедельник. При получении метаданных элемента в качестве даты его создания указывается вторник, но в аспекте `fileSystemInfo` отображается исходная дата создания — понедельник.</span><span class="sxs-lookup"><span data-stu-id="bbee8-p104">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="bbee8-p105">Эти свойства доступны для чтения и записи. Если вы загружаете файл и вам известны локальные клиентские значения для этих полей, их необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="bbee8-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="bbee8-129">Если содержимое файла обновлено и эти свойства не предоставлены, **lastModifiedDateTime** автоматически сбрасывает текущее время.</span><span class="sxs-lookup"><span data-stu-id="bbee8-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="bbee8-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="bbee8-130">Remarks</span></span>

* <span data-ttu-id="bbee8-131">Свойство **lastAccessedDateTime** недоступно для элементов в SharePoint Online или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="bbee8-131">**lastAccessedDateTime** is not available for items in SharePoint online or OneDrive for Business.</span></span>

<span data-ttu-id="bbee8-132">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bbee8-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/filesysteminfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
