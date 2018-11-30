---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
ms.openlocfilehash: 9a5214f9c5e161de0be66ac634c7c5538b203772
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="7eef1-102">Аспект FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="7eef1-102">FileSystemInfo facet</span></span>

<span data-ttu-id="7eef1-103">Ресурс **FileSystemInfo** содержит свойства, которые отображаются в локальной файловой системе устройства для локальной версии элемента.</span><span class="sxs-lookup"><span data-stu-id="7eef1-103">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>
<span data-ttu-id="7eef1-104">Этот аспект можно использовать, чтобы указать дату создания или последнего изменения элемента, какой она была на локальном устройстве.</span><span class="sxs-lookup"><span data-stu-id="7eef1-104">The FileSystemInfo facet contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="7eef1-105">Он доступен в свойстве fileSystemInfo ресурсов [driveItem][item-resource].</span><span class="sxs-lookup"><span data-stu-id="7eef1-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7eef1-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7eef1-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7eef1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7eef1-107">Properties</span></span>

| <span data-ttu-id="7eef1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7eef1-108">Property</span></span>                 | <span data-ttu-id="7eef1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7eef1-109">Type</span></span>           | <span data-ttu-id="7eef1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7eef1-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7eef1-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="7eef1-111">**createdDateTime**</span></span>      | <span data-ttu-id="7eef1-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7eef1-112">DateTimeOffset</span></span> | <span data-ttu-id="7eef1-113">Дата и время создания файла в клиентском устройстве в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7eef1-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="7eef1-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="7eef1-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="7eef1-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7eef1-115">DateTimeOffset</span></span> | <span data-ttu-id="7eef1-116">Дата и время последнего использования файла в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7eef1-116">The UTC date and time the file was last accessed on a client.</span></span> <span data-ttu-id="7eef1-117">Доступно только для [списка последних файлов](../api/drive_recent.md).</span><span class="sxs-lookup"><span data-stu-id="7eef1-117">Available for the [recent file list](../api/drive_recent.md) only.</span></span> |
| <span data-ttu-id="7eef1-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="7eef1-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="7eef1-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7eef1-119">DateTimeOffset</span></span> | <span data-ttu-id="7eef1-120">Дата и время последнего изменения файла в клиентском устройстве в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7eef1-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="7eef1-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="7eef1-121">Notes</span></span>

<span data-ttu-id="7eef1-122">Значения свойств **createdDateTime** и **lastModifiedDateTime** отличаются от этих же свойств ресурса [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7eef1-122">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource.</span></span>
<span data-ttu-id="7eef1-123">В качестве значений для ресурса DriveItem выступают дата и время создания или изменения, которые зарегистрированы в службе.</span><span class="sxs-lookup"><span data-stu-id="7eef1-123">The properties on the driveItem resource are the created and modified date and time from the perspective of when the service saw the file.</span></span>
<span data-ttu-id="7eef1-124">Значения, хранящиеся в ресурсе **FileSystemInfo**, предоставляет клиент.</span><span class="sxs-lookup"><span data-stu-id="7eef1-124">The values stored in the **FileSystemInfo** facet are provided by the client are are the values displayed to the user if they exist.</span></span>

<span data-ttu-id="7eef1-125">Например, если файл был создан на устройстве в понедельник, но не отправлен в службу до вторника, клиент, отправляющий файл, должен записать дату создания, соответствующую понедельнику, в аспект `fileSystemInfo`.</span><span class="sxs-lookup"><span data-stu-id="7eef1-125">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the  facet will show the original created date on Monday.</span></span> <span data-ttu-id="7eef1-126">При получении метаданных элемента в качестве даты его создания будет указан вторник, но в аспекте `fileSystemInfo` будет отображаться исходная дата создания — понедельник.</span><span class="sxs-lookup"><span data-stu-id="7eef1-126">When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="7eef1-p105">Эти свойства доступны для чтения и записи. Если вы загружаете файл и вам известны локальные клиентские значения для этих полей, их необходимо включить в запрос.</span><span class="sxs-lookup"><span data-stu-id="7eef1-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="7eef1-129">Если содержимое файла обновлено и эти свойства не предоставлены, **lastModifiedDateTime** автоматически сбрасывает текущее время.</span><span class="sxs-lookup"><span data-stu-id="7eef1-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="7eef1-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="7eef1-130">Remarks</span></span>

* <span data-ttu-id="7eef1-131">Свойство **lastAccessedDateTime** недоступно для элементов в SharePoint Online или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7eef1-131">**lastAccessedDateTime** is not available for items in SharePoint online, OneDrive for Business, or SharePoint Server 2016.</span></span>

<span data-ttu-id="7eef1-132">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7eef1-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
