---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: remoteItem
localization_priority: Normal
ms.openlocfilehash: 122e13513db1a59e23a41cadd16e61996e6a6c04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843192"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="ff0d2-102">Тип ресурса RemoteItem</span><span class="sxs-lookup"><span data-stu-id="ff0d2-102">RemoteItem resource type</span></span>

> <span data-ttu-id="ff0d2-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff0d2-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff0d2-p102">Ресурс **remoteItem** указывает, что элемент [**driveItem**](driveitem.md) ссылается на элемент, находящийся на другом диске. Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p102">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="ff0d2-107">Элементы [**DriveItem**](driveitem.md) с аспектом **remoteItem**, не равным null, — это ресурсы, к которым предоставлен общий доступ, ресурсы, добавленные в хранилище OneDrive пользователя, или ресурсы в элементах, возвращенных из коллекций разнородных элементов (например, результатов поиска).</span><span class="sxs-lookup"><span data-stu-id="ff0d2-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="ff0d2-108">**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff0d2-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff0d2-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ff0d2-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff0d2-110">Properties</span></span>

| <span data-ttu-id="ff0d2-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ff0d2-111">Property name</span></span>        | <span data-ttu-id="ff0d2-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ff0d2-112">Type</span></span>                                | <span data-ttu-id="ff0d2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ff0d2-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ff0d2-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="ff0d2-114">createdBy</span></span>            | [<span data-ttu-id="ff0d2-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ff0d2-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="ff0d2-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="ff0d2-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0d2-118">createdDateTime</span></span>      | <span data-ttu-id="ff0d2-119">Timestamp</span><span class="sxs-lookup"><span data-stu-id="ff0d2-119">Timestamp</span></span>                           | <span data-ttu-id="ff0d2-p104">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="ff0d2-122">file</span><span class="sxs-lookup"><span data-stu-id="ff0d2-122">file</span></span>                 | [<span data-ttu-id="ff0d2-123">File</span><span class="sxs-lookup"><span data-stu-id="ff0d2-123">File</span></span>](file.md)                     | <span data-ttu-id="ff0d2-p105">Указывает, что удаленный элемент является файлом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p105">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="ff0d2-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="ff0d2-126">fileSystemInfo</span></span>       | [<span data-ttu-id="ff0d2-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="ff0d2-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="ff0d2-p106">Сведения об удаленном элементе из локальной файловой системы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p106">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="ff0d2-130">folder</span><span class="sxs-lookup"><span data-stu-id="ff0d2-130">folder</span></span>               | [<span data-ttu-id="ff0d2-131">Folder</span><span class="sxs-lookup"><span data-stu-id="ff0d2-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="ff0d2-p107">Указывает, что удаленный элемент является папкой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p107">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="ff0d2-134">id</span><span class="sxs-lookup"><span data-stu-id="ff0d2-134">id</span></span>                   | <span data-ttu-id="ff0d2-135">Строка</span><span class="sxs-lookup"><span data-stu-id="ff0d2-135">String</span></span>                              | <span data-ttu-id="ff0d2-p108">Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p108">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="ff0d2-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ff0d2-138">lastModifiedBy</span></span>       | [<span data-ttu-id="ff0d2-139">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ff0d2-139">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="ff0d2-p109">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p109">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="ff0d2-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0d2-142">lastModifiedDateTime</span></span> | <span data-ttu-id="ff0d2-143">Timestamp</span><span class="sxs-lookup"><span data-stu-id="ff0d2-143">Timestamp</span></span>                           | <span data-ttu-id="ff0d2-p110">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p110">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="ff0d2-146">name</span><span class="sxs-lookup"><span data-stu-id="ff0d2-146">name</span></span>                 | <span data-ttu-id="ff0d2-147">Строка</span><span class="sxs-lookup"><span data-stu-id="ff0d2-147">String</span></span>                              | <span data-ttu-id="ff0d2-p111">Необязательное свойство. Имя файла удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p111">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="ff0d2-151">пакет</span><span class="sxs-lookup"><span data-stu-id="ff0d2-151">package</span></span>              | [<span data-ttu-id="ff0d2-152">Package</span><span class="sxs-lookup"><span data-stu-id="ff0d2-152">Package</span></span>](package.md)               | <span data-ttu-id="ff0d2-p112">При наличии этого свойства оно указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p112">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="ff0d2-156">parentReference</span><span class="sxs-lookup"><span data-stu-id="ff0d2-156">parentReference</span></span>      | [<span data-ttu-id="ff0d2-157">ItemReference</span><span class="sxs-lookup"><span data-stu-id="ff0d2-157">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="ff0d2-p113">Свойства родительского элемента удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p113">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="ff0d2-160">shared</span><span class="sxs-lookup"><span data-stu-id="ff0d2-160">shared</span></span>               | [<span data-ttu-id="ff0d2-161">shared</span><span class="sxs-lookup"><span data-stu-id="ff0d2-161">shared</span></span>](shared.md)                 | <span data-ttu-id="ff0d2-p114">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p114">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="ff0d2-164">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ff0d2-164">sharepointIds</span></span>        | [<span data-ttu-id="ff0d2-165">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="ff0d2-165">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="ff0d2-p115">Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p115">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="ff0d2-168">size</span><span class="sxs-lookup"><span data-stu-id="ff0d2-168">size</span></span>                 | <span data-ttu-id="ff0d2-169">Int64</span><span class="sxs-lookup"><span data-stu-id="ff0d2-169">Int64</span></span>                               | <span data-ttu-id="ff0d2-p116">Размер удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p116">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="ff0d2-172">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="ff0d2-172">webDavUrl</span></span>            | <span data-ttu-id="ff0d2-173">Url</span><span class="sxs-lookup"><span data-stu-id="ff0d2-173">Url</span></span>                                 | <span data-ttu-id="ff0d2-174">URL-адрес, совместимый с протоколом DAV, для элемента.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-174">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="ff0d2-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="ff0d2-175">webUrl</span></span>               | <span data-ttu-id="ff0d2-176">Url</span><span class="sxs-lookup"><span data-stu-id="ff0d2-176">Url</span></span>                                 | <span data-ttu-id="ff0d2-p117">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff0d2-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="ff0d2-179">Заметки</span><span class="sxs-lookup"><span data-stu-id="ff0d2-179">Remarks</span></span>

<span data-ttu-id="ff0d2-180">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ff0d2-180">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
