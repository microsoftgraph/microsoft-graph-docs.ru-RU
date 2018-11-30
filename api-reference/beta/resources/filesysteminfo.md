---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
ms.openlocfilehash: 08a79a265e8d4dbda3017a1ff8a32c5e4cab51ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075520"
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="aca32-102">Аспект FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="aca32-102">FileSystemInfo facet</span></span>

> <span data-ttu-id="aca32-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aca32-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aca32-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aca32-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aca32-p102">Ресурс **FileSystemInfo** содержит свойства, которые отображаются в локальной файловой системе устройства для локальной версии элемента. Этот аспект можно использовать, чтобы указать последнюю дату изменения или создания элемента, какой она была на локальном устройстве.</span><span class="sxs-lookup"><span data-stu-id="aca32-p102">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="aca32-107">Он доступен в свойстве fileSystemInfo ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="aca32-107">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aca32-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aca32-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="aca32-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="aca32-109">Properties</span></span>

| <span data-ttu-id="aca32-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="aca32-110">Property</span></span>                 | <span data-ttu-id="aca32-111">Тип</span><span class="sxs-lookup"><span data-stu-id="aca32-111">Type</span></span>           | <span data-ttu-id="aca32-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aca32-112">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="aca32-113">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="aca32-113">**createdDateTime**</span></span>      | <span data-ttu-id="aca32-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aca32-114">DateTimeOffset</span></span> | <span data-ttu-id="aca32-115">Дата и время создания файла в клиентском устройстве в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="aca32-115">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="aca32-116">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="aca32-116">**lastAccessedDateTime**</span></span> | <span data-ttu-id="aca32-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aca32-117">DateTimeOffset</span></span> | <span data-ttu-id="aca32-p103">Дата и время последнего использования файла в формате UTC. Доступно только для [списка последних файлов](../api/drive-recent.md).</span><span class="sxs-lookup"><span data-stu-id="aca32-p103">The UTC date and time the file was last accessed. Available for the [recent file list](../api/drive-recent.md) only.</span></span> |
| <span data-ttu-id="aca32-120">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="aca32-120">**lastModifiedDateTime**</span></span> | <span data-ttu-id="aca32-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aca32-121">DateTimeOffset</span></span> | <span data-ttu-id="aca32-122">Дата и время последнего изменения файла в клиентском устройстве в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="aca32-122">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="aca32-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="aca32-123">Notes</span></span>

<span data-ttu-id="aca32-p104">Значения свойств **createdDateTime** и **lastModifiedDateTime** отличаются от этих же свойств ресурса [DriveItem](driveitem.md). В качестве значений для ресурса DriveItem выступают созданные или измененные дата и время, которые можно увидеть в службе. Значения, хранящиеся в ресурсе **FileSystemInfo**, предоставляются клиентом.</span><span class="sxs-lookup"><span data-stu-id="aca32-p104">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource. The values on the DriveItem resource are the created and modified date and time as seen from the service. The values stored in the **FileSystemInfo** resource are provided by the client.</span></span>

<span data-ttu-id="aca32-p105">Например, если файл был создан на устройстве в понедельник, но не загружен в службу до вторника, клиент, загружающий файл, должен прописать аспект `fileSystemInfo`включить дату создания в понедельник. При получении метаданных элемента в качестве даты его создания указывается вторник, но в аспекте `fileSystemInfo` отображается исходная дата создания — понедельник.</span><span class="sxs-lookup"><span data-stu-id="aca32-p105">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="aca32-p106">Эти свойства доступны для чтения и записи. Если вы загружаете файл и вам известны локальные клиентские значения для этих полей, их необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="aca32-p106">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="aca32-131">Если содержимое файла обновлено и эти свойства не предоставлены, **lastModifiedDateTime** автоматически сбрасывает текущее время.</span><span class="sxs-lookup"><span data-stu-id="aca32-131">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="aca32-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="aca32-132">Remarks</span></span>

* <span data-ttu-id="aca32-133">Свойство **lastAccessedDateTime** недоступно для элементов в SharePoint Online или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="aca32-133">**lastAccessedDateTime** is not available for items in SharePoint online or OneDrive for Business.</span></span>

<span data-ttu-id="aca32-134">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="aca32-134">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
