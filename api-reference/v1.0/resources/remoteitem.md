---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: ceb66fdacd4a108318c84fd9297aca8b2332c3f3
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481127"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="87490-102">Тип ресурса RemoteItem</span><span class="sxs-lookup"><span data-stu-id="87490-102">RemoteItem resource type</span></span>

<span data-ttu-id="87490-103">Ресурс **remoteItem** указывает, что элемент [**driveItem**](driveitem.md) ссылается на элемент, находящийся на другом диске.</span><span class="sxs-lookup"><span data-stu-id="87490-103">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="87490-104">Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="87490-104">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="87490-105">Элементы [**DriveItem**](driveitem.md) с аспектом **remoteItem**, не равным null, — это ресурсы, к которым предоставлен общий доступ, ресурсы, добавленные в хранилище OneDrive пользователя, или ресурсы в элементах, возвращенных из коллекций разнородных элементов (например, результатов поиска).</span><span class="sxs-lookup"><span data-stu-id="87490-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="87490-106">**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.</span><span class="sxs-lookup"><span data-stu-id="87490-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87490-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87490-107">JSON representation</span></span>

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
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="87490-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="87490-108">Properties</span></span>

| <span data-ttu-id="87490-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="87490-109">Property name</span></span>        | <span data-ttu-id="87490-110">Тип</span><span class="sxs-lookup"><span data-stu-id="87490-110">Type</span></span>                                | <span data-ttu-id="87490-111">Описание</span><span class="sxs-lookup"><span data-stu-id="87490-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="87490-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="87490-112">createdBy</span></span>            | [<span data-ttu-id="87490-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="87490-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="87490-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="87490-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87490-116">createdDateTime</span></span>      | <span data-ttu-id="87490-117">Timestamp</span><span class="sxs-lookup"><span data-stu-id="87490-117">Timestamp</span></span>                           | <span data-ttu-id="87490-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="87490-120">file</span><span class="sxs-lookup"><span data-stu-id="87490-120">file</span></span>                 | [<span data-ttu-id="87490-121">File</span><span class="sxs-lookup"><span data-stu-id="87490-121">File</span></span>](file.md)                     | <span data-ttu-id="87490-p104">Указывает, что удаленный элемент является файлом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="87490-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="87490-124">fileSystemInfo</span></span>       | [<span data-ttu-id="87490-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="87490-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="87490-p105">Сведения об удаленном элементе из локальной файловой системы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="87490-128">folder</span><span class="sxs-lookup"><span data-stu-id="87490-128">folder</span></span>               | [<span data-ttu-id="87490-129">Folder</span><span class="sxs-lookup"><span data-stu-id="87490-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="87490-p106">Указывает, что удаленный элемент является папкой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="87490-132">id</span><span class="sxs-lookup"><span data-stu-id="87490-132">id</span></span>                   | <span data-ttu-id="87490-133">String</span><span class="sxs-lookup"><span data-stu-id="87490-133">String</span></span>                              | <span data-ttu-id="87490-p107">Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="87490-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="87490-136">lastModifiedBy</span></span>       | [<span data-ttu-id="87490-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="87490-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="87490-p108">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="87490-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87490-140">lastModifiedDateTime</span></span> | <span data-ttu-id="87490-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="87490-141">Timestamp</span></span>                           | <span data-ttu-id="87490-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="87490-144">name</span><span class="sxs-lookup"><span data-stu-id="87490-144">name</span></span>                 | <span data-ttu-id="87490-145">String</span><span class="sxs-lookup"><span data-stu-id="87490-145">String</span></span>                              | <span data-ttu-id="87490-p110">Необязательное свойство. Имя файла удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="87490-149">пакет</span><span class="sxs-lookup"><span data-stu-id="87490-149">package</span></span>              | [<span data-ttu-id="87490-150">Package</span><span class="sxs-lookup"><span data-stu-id="87490-150">Package</span></span>](package.md)               | <span data-ttu-id="87490-p111">При наличии этого свойства оно указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="87490-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="87490-154">parentReference</span></span>      | [<span data-ttu-id="87490-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="87490-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="87490-p112">Свойства родительского элемента удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="87490-158">shared</span><span class="sxs-lookup"><span data-stu-id="87490-158">shared</span></span>               | [<span data-ttu-id="87490-159">shared</span><span class="sxs-lookup"><span data-stu-id="87490-159">shared</span></span>](shared.md)                 | <span data-ttu-id="87490-p113">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="87490-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="87490-162">sharepointIds</span></span>        | [<span data-ttu-id="87490-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="87490-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="87490-p114">Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="87490-166">size</span><span class="sxs-lookup"><span data-stu-id="87490-166">size</span></span>                 | <span data-ttu-id="87490-167">Int64</span><span class="sxs-lookup"><span data-stu-id="87490-167">Int64</span></span>                               | <span data-ttu-id="87490-p115">Размер удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="87490-170">specialFolder</span><span class="sxs-lookup"><span data-stu-id="87490-170">specialFolder</span></span>        | <span data-ttu-id="87490-171">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="87490-171">[specialFolder][]</span></span>                   | <span data-ttu-id="87490-p116">Если текущий элемент также доступен в качестве специальной папки, то будет возвращен этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p116">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>                                                                     |
| <span data-ttu-id="87490-174">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="87490-174">webDavUrl</span></span>            | <span data-ttu-id="87490-175">Url</span><span class="sxs-lookup"><span data-stu-id="87490-175">Url</span></span>                                 | <span data-ttu-id="87490-176">URL-адрес, совместимый с протоколом DAV, для элемента.</span><span class="sxs-lookup"><span data-stu-id="87490-176">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="87490-177">webUrl</span><span class="sxs-lookup"><span data-stu-id="87490-177">webUrl</span></span>               | <span data-ttu-id="87490-178">Url</span><span class="sxs-lookup"><span data-stu-id="87490-178">Url</span></span>                                 | <span data-ttu-id="87490-p117">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87490-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a><span data-ttu-id="87490-182">Заметки</span><span class="sxs-lookup"><span data-stu-id="87490-182">Remarks</span></span>

<span data-ttu-id="87490-183">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="87490-183">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
