---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
description: Ресурс remoteItem указывает, что элемент driveItem ссылается на элемент, находящийся на другом диске.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0d19034475f72984f023cef368e1fec5f75fe456
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034729"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="1d57c-103">Тип ресурса RemoteItem</span><span class="sxs-lookup"><span data-stu-id="1d57c-103">RemoteItem resource type</span></span>

<span data-ttu-id="1d57c-104">Ресурс **remoteItem** указывает, что элемент [**driveItem**](driveitem.md) ссылается на элемент, находящийся на другом диске.</span><span class="sxs-lookup"><span data-stu-id="1d57c-104">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="1d57c-105">Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="1d57c-105">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="1d57c-106">Элементы [**DriveItem**](driveitem.md) с аспектом **remoteItem**, не равным null, — это ресурсы, к которым предоставлен общий доступ, ресурсы, добавленные в хранилище OneDrive пользователя, или ресурсы в элементах, возвращенных из коллекций разнородных элементов (например, результатов поиска).</span><span class="sxs-lookup"><span data-stu-id="1d57c-106">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="1d57c-107">**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.</span><span class="sxs-lookup"><span data-stu-id="1d57c-107">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d57c-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d57c-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1d57c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d57c-109">Properties</span></span>

| <span data-ttu-id="1d57c-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1d57c-110">Property name</span></span>        | <span data-ttu-id="1d57c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1d57c-111">Type</span></span>                                | <span data-ttu-id="1d57c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1d57c-112">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1d57c-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="1d57c-113">createdBy</span></span>            | [<span data-ttu-id="1d57c-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="1d57c-114">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="1d57c-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="1d57c-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d57c-117">createdDateTime</span></span>      | <span data-ttu-id="1d57c-118">Timestamp</span><span class="sxs-lookup"><span data-stu-id="1d57c-118">Timestamp</span></span>                           | <span data-ttu-id="1d57c-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="1d57c-121">file</span><span class="sxs-lookup"><span data-stu-id="1d57c-121">file</span></span>                 | [<span data-ttu-id="1d57c-122">File</span><span class="sxs-lookup"><span data-stu-id="1d57c-122">File</span></span>](file.md)                     | <span data-ttu-id="1d57c-p104">Указывает, что удаленный элемент является файлом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="1d57c-125">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="1d57c-125">fileSystemInfo</span></span>       | [<span data-ttu-id="1d57c-126">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="1d57c-126">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="1d57c-p105">Сведения об удаленном элементе из локальной файловой системы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="1d57c-129">folder</span><span class="sxs-lookup"><span data-stu-id="1d57c-129">folder</span></span>               | [<span data-ttu-id="1d57c-130">Folder</span><span class="sxs-lookup"><span data-stu-id="1d57c-130">Folder</span></span>](folder.md)                 | <span data-ttu-id="1d57c-p106">Указывает, что удаленный элемент является папкой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="1d57c-133">id</span><span class="sxs-lookup"><span data-stu-id="1d57c-133">id</span></span>                   | <span data-ttu-id="1d57c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1d57c-134">String</span></span>                              | <span data-ttu-id="1d57c-p107">Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="1d57c-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1d57c-137">lastModifiedBy</span></span>       | [<span data-ttu-id="1d57c-138">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="1d57c-138">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="1d57c-p108">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="1d57c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d57c-141">lastModifiedDateTime</span></span> | <span data-ttu-id="1d57c-142">Timestamp</span><span class="sxs-lookup"><span data-stu-id="1d57c-142">Timestamp</span></span>                           | <span data-ttu-id="1d57c-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="1d57c-145">name</span><span class="sxs-lookup"><span data-stu-id="1d57c-145">name</span></span>                 | <span data-ttu-id="1d57c-146">String</span><span class="sxs-lookup"><span data-stu-id="1d57c-146">String</span></span>                              | <span data-ttu-id="1d57c-p110">Необязательное свойство. Имя файла удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="1d57c-150">пакет</span><span class="sxs-lookup"><span data-stu-id="1d57c-150">package</span></span>              | [<span data-ttu-id="1d57c-151">Package</span><span class="sxs-lookup"><span data-stu-id="1d57c-151">Package</span></span>](package.md)               | <span data-ttu-id="1d57c-p111">В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="1d57c-155">parentReference</span><span class="sxs-lookup"><span data-stu-id="1d57c-155">parentReference</span></span>      | [<span data-ttu-id="1d57c-156">ItemReference</span><span class="sxs-lookup"><span data-stu-id="1d57c-156">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="1d57c-p112">Свойства родительского элемента удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="1d57c-159">общие</span><span class="sxs-lookup"><span data-stu-id="1d57c-159">shared</span></span>               | [<span data-ttu-id="1d57c-160">shared</span><span class="sxs-lookup"><span data-stu-id="1d57c-160">shared</span></span>](shared.md)                 | <span data-ttu-id="1d57c-p113">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="1d57c-163">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="1d57c-163">sharepointIds</span></span>        | [<span data-ttu-id="1d57c-164">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="1d57c-164">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="1d57c-p114">Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="1d57c-167">size</span><span class="sxs-lookup"><span data-stu-id="1d57c-167">size</span></span>                 | <span data-ttu-id="1d57c-168">Int64</span><span class="sxs-lookup"><span data-stu-id="1d57c-168">Int64</span></span>                               | <span data-ttu-id="1d57c-p115">Размер удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="1d57c-171">specialFolder</span><span class="sxs-lookup"><span data-stu-id="1d57c-171">specialFolder</span></span>        | <span data-ttu-id="1d57c-172">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="1d57c-172">[specialFolder][]</span></span>                   | <span data-ttu-id="1d57c-p116">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p116">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>                                                                     |
| <span data-ttu-id="1d57c-175">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="1d57c-175">webDavUrl</span></span>            | <span data-ttu-id="1d57c-176">Url</span><span class="sxs-lookup"><span data-stu-id="1d57c-176">Url</span></span>                                 | <span data-ttu-id="1d57c-177">URL-адрес, совместимый с протоколом DAV, для элемента.</span><span class="sxs-lookup"><span data-stu-id="1d57c-177">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="1d57c-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="1d57c-178">webUrl</span></span>               | <span data-ttu-id="1d57c-179">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="1d57c-179">Url</span></span>                                 | <span data-ttu-id="1d57c-p117">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d57c-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a><span data-ttu-id="1d57c-183">Заметки</span><span class="sxs-lookup"><span data-stu-id="1d57c-183">Remarks</span></span>

<span data-ttu-id="1d57c-184">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1d57c-184">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
