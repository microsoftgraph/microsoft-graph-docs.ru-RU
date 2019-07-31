---
author: JeremyKelley
description: Ресурс remoteItem указывает, что элемент driveItem ссылается на элемент, находящийся на другом диске.
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 05da43fb3d7b1e2adec01f707eeed61df4623f04
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008707"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="d1658-103">Тип ресурса RemoteItem</span><span class="sxs-lookup"><span data-stu-id="d1658-103">RemoteItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1658-104">Ресурс **remoteItem** указывает, что элемент [**driveItem**](driveitem.md) ссылается на элемент, находящийся на другом диске.</span><span class="sxs-lookup"><span data-stu-id="d1658-104">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="d1658-105">Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="d1658-105">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="d1658-106">Элементы [**DriveItem**](driveitem.md) с аспектом **remoteItem**, не равным null, — это ресурсы, к которым предоставлен общий доступ, ресурсы, добавленные в хранилище OneDrive пользователя, или ресурсы в элементах, возвращенных из коллекций разнородных элементов (например, результатов поиска).</span><span class="sxs-lookup"><span data-stu-id="d1658-106">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="d1658-107">**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.</span><span class="sxs-lookup"><span data-stu-id="d1658-107">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1658-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1658-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d1658-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1658-109">Properties</span></span>

| <span data-ttu-id="d1658-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d1658-110">Property name</span></span>        | <span data-ttu-id="d1658-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d1658-111">Type</span></span>                                | <span data-ttu-id="d1658-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d1658-112">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d1658-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="d1658-113">createdBy</span></span>            | [<span data-ttu-id="d1658-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d1658-114">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="d1658-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="d1658-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1658-117">createdDateTime</span></span>      | <span data-ttu-id="d1658-118">Timestamp</span><span class="sxs-lookup"><span data-stu-id="d1658-118">Timestamp</span></span>                           | <span data-ttu-id="d1658-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="d1658-121">file</span><span class="sxs-lookup"><span data-stu-id="d1658-121">file</span></span>                 | [<span data-ttu-id="d1658-122">File</span><span class="sxs-lookup"><span data-stu-id="d1658-122">File</span></span>](file.md)                     | <span data-ttu-id="d1658-p104">Указывает, что удаленный элемент является файлом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="d1658-125">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="d1658-125">fileSystemInfo</span></span>       | [<span data-ttu-id="d1658-126">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="d1658-126">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="d1658-p105">Сведения об удаленном элементе из локальной файловой системы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="d1658-129">folder</span><span class="sxs-lookup"><span data-stu-id="d1658-129">folder</span></span>               | [<span data-ttu-id="d1658-130">Folder</span><span class="sxs-lookup"><span data-stu-id="d1658-130">Folder</span></span>](folder.md)                 | <span data-ttu-id="d1658-p106">Указывает, что удаленный элемент является папкой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="d1658-133">id</span><span class="sxs-lookup"><span data-stu-id="d1658-133">id</span></span>                   | <span data-ttu-id="d1658-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d1658-134">String</span></span>                              | <span data-ttu-id="d1658-p107">Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="d1658-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d1658-137">lastModifiedBy</span></span>       | [<span data-ttu-id="d1658-138">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d1658-138">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="d1658-p108">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="d1658-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1658-141">lastModifiedDateTime</span></span> | <span data-ttu-id="d1658-142">Timestamp</span><span class="sxs-lookup"><span data-stu-id="d1658-142">Timestamp</span></span>                           | <span data-ttu-id="d1658-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="d1658-145">name</span><span class="sxs-lookup"><span data-stu-id="d1658-145">name</span></span>                 | <span data-ttu-id="d1658-146">String</span><span class="sxs-lookup"><span data-stu-id="d1658-146">String</span></span>                              | <span data-ttu-id="d1658-p110">Необязательное свойство. Имя файла удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="d1658-150">пакет</span><span class="sxs-lookup"><span data-stu-id="d1658-150">package</span></span>              | [<span data-ttu-id="d1658-151">Package</span><span class="sxs-lookup"><span data-stu-id="d1658-151">Package</span></span>](package.md)               | <span data-ttu-id="d1658-p111">В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="d1658-155">parentReference</span><span class="sxs-lookup"><span data-stu-id="d1658-155">parentReference</span></span>      | [<span data-ttu-id="d1658-156">ItemReference</span><span class="sxs-lookup"><span data-stu-id="d1658-156">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="d1658-p112">Свойства родительского элемента удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="d1658-159">общие</span><span class="sxs-lookup"><span data-stu-id="d1658-159">shared</span></span>               | [<span data-ttu-id="d1658-160">shared</span><span class="sxs-lookup"><span data-stu-id="d1658-160">shared</span></span>](shared.md)                 | <span data-ttu-id="d1658-p113">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="d1658-163">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="d1658-163">sharepointIds</span></span>        | [<span data-ttu-id="d1658-164">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="d1658-164">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="d1658-p114">Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="d1658-167">size</span><span class="sxs-lookup"><span data-stu-id="d1658-167">size</span></span>                 | <span data-ttu-id="d1658-168">Int64</span><span class="sxs-lookup"><span data-stu-id="d1658-168">Int64</span></span>                               | <span data-ttu-id="d1658-p115">Размер удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="d1658-171">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="d1658-171">webDavUrl</span></span>            | <span data-ttu-id="d1658-172">Url</span><span class="sxs-lookup"><span data-stu-id="d1658-172">Url</span></span>                                 | <span data-ttu-id="d1658-173">URL-адрес, совместимый с протоколом DAV, для элемента.</span><span class="sxs-lookup"><span data-stu-id="d1658-173">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="d1658-174">webUrl</span><span class="sxs-lookup"><span data-stu-id="d1658-174">webUrl</span></span>               | <span data-ttu-id="d1658-175">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="d1658-175">Url</span></span>                                 | <span data-ttu-id="d1658-p116">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1658-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="d1658-178">Заметки</span><span class="sxs-lookup"><span data-stu-id="d1658-178">Remarks</span></span>

<span data-ttu-id="d1658-179">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d1658-179">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": []
}
-->
