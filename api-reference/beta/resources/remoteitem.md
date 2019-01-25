---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: remoteItem
localization_priority: Normal
ms.openlocfilehash: 13eb7ff286467a7acfef85f58ea59763a13d9801
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514336"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="8e5c7-102">Тип ресурса RemoteItem</span><span class="sxs-lookup"><span data-stu-id="8e5c7-102">RemoteItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e5c7-p101">Ресурс remoteItem указывает, что элемент driveItem ссылается на элемент, находящийся на другом диске. Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p101">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="8e5c7-105">Элементы [**DriveItem**](driveitem.md) с аспектом **remoteItem**, не равным null, — это ресурсы, к которым предоставлен общий доступ, ресурсы, добавленные в хранилище OneDrive пользователя, или ресурсы в элементах, возвращенных из коллекций разнородных элементов (например, результатов поиска).</span><span class="sxs-lookup"><span data-stu-id="8e5c7-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="8e5c7-106">**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e5c7-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e5c7-107">JSON representation</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="8e5c7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e5c7-108">Properties</span></span>

| <span data-ttu-id="8e5c7-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8e5c7-109">Property name</span></span>        | <span data-ttu-id="8e5c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8e5c7-110">Type</span></span>                                | <span data-ttu-id="8e5c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e5c7-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8e5c7-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="8e5c7-112">createdBy</span></span>            | [<span data-ttu-id="8e5c7-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8e5c7-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="8e5c7-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="8e5c7-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e5c7-116">createdDateTime</span></span>      | <span data-ttu-id="8e5c7-117">Timestamp</span><span class="sxs-lookup"><span data-stu-id="8e5c7-117">Timestamp</span></span>                           | <span data-ttu-id="8e5c7-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="8e5c7-120">file</span><span class="sxs-lookup"><span data-stu-id="8e5c7-120">file</span></span>                 | [<span data-ttu-id="8e5c7-121">File</span><span class="sxs-lookup"><span data-stu-id="8e5c7-121">File</span></span>](file.md)                     | <span data-ttu-id="8e5c7-p104">Указывает, что удаленный элемент является файлом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="8e5c7-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="8e5c7-124">fileSystemInfo</span></span>       | [<span data-ttu-id="8e5c7-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="8e5c7-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="8e5c7-p105">Сведения об удаленном элементе из локальной файловой системы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="8e5c7-128">folder</span><span class="sxs-lookup"><span data-stu-id="8e5c7-128">folder</span></span>               | [<span data-ttu-id="8e5c7-129">Folder</span><span class="sxs-lookup"><span data-stu-id="8e5c7-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="8e5c7-p106">Указывает, что удаленный элемент является папкой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="8e5c7-132">id</span><span class="sxs-lookup"><span data-stu-id="8e5c7-132">id</span></span>                   | <span data-ttu-id="8e5c7-133">String</span><span class="sxs-lookup"><span data-stu-id="8e5c7-133">String</span></span>                              | <span data-ttu-id="8e5c7-p107">Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="8e5c7-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8e5c7-136">lastModifiedBy</span></span>       | [<span data-ttu-id="8e5c7-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8e5c7-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="8e5c7-p108">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="8e5c7-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e5c7-140">lastModifiedDateTime</span></span> | <span data-ttu-id="8e5c7-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="8e5c7-141">Timestamp</span></span>                           | <span data-ttu-id="8e5c7-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="8e5c7-144">имя</span><span class="sxs-lookup"><span data-stu-id="8e5c7-144">name</span></span>                 | <span data-ttu-id="8e5c7-145">String</span><span class="sxs-lookup"><span data-stu-id="8e5c7-145">String</span></span>                              | <span data-ttu-id="8e5c7-p110">Необязательное свойство. Имя файла удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="8e5c7-149">пакет</span><span class="sxs-lookup"><span data-stu-id="8e5c7-149">package</span></span>              | [<span data-ttu-id="8e5c7-150">Package</span><span class="sxs-lookup"><span data-stu-id="8e5c7-150">Package</span></span>](package.md)               | <span data-ttu-id="8e5c7-p111">При наличии этого свойства оно указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="8e5c7-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="8e5c7-154">parentReference</span></span>      | [<span data-ttu-id="8e5c7-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="8e5c7-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="8e5c7-p112">Свойства родительского элемента удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="8e5c7-158">shared</span><span class="sxs-lookup"><span data-stu-id="8e5c7-158">shared</span></span>               | [<span data-ttu-id="8e5c7-159">shared</span><span class="sxs-lookup"><span data-stu-id="8e5c7-159">shared</span></span>](shared.md)                 | <span data-ttu-id="8e5c7-p113">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="8e5c7-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8e5c7-162">sharepointIds</span></span>        | [<span data-ttu-id="8e5c7-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="8e5c7-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="8e5c7-p114">Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="8e5c7-166">size</span><span class="sxs-lookup"><span data-stu-id="8e5c7-166">size</span></span>                 | <span data-ttu-id="8e5c7-167">Int64</span><span class="sxs-lookup"><span data-stu-id="8e5c7-167">Int64</span></span>                               | <span data-ttu-id="8e5c7-p115">Размер удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="8e5c7-170">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="8e5c7-170">webDavUrl</span></span>            | <span data-ttu-id="8e5c7-171">Url</span><span class="sxs-lookup"><span data-stu-id="8e5c7-171">Url</span></span>                                 | <span data-ttu-id="8e5c7-172">URL-адрес, совместимый с протоколом DAV, для элемента.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-172">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="8e5c7-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="8e5c7-173">webUrl</span></span>               | <span data-ttu-id="8e5c7-174">Url</span><span class="sxs-lookup"><span data-stu-id="8e5c7-174">Url</span></span>                                 | <span data-ttu-id="8e5c7-p116">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e5c7-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="8e5c7-177">Заметки</span><span class="sxs-lookup"><span data-stu-id="8e5c7-177">Remarks</span></span>

<span data-ttu-id="8e5c7-178">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8e5c7-178">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/remoteitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
