---
author: JeremyKelley
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
description: Ресурс remoteItem указывает, что элемент driveItem ссылается на элемент, находящийся на другом диске.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d913645b0563834f0493243aa006c34058991f7c
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240376"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="8f94a-103">Тип ресурса RemoteItem</span><span class="sxs-lookup"><span data-stu-id="8f94a-103">RemoteItem resource type</span></span>

<span data-ttu-id="8f94a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f94a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f94a-105">Ресурс **remoteItem** указывает, что элемент [**driveItem**](driveitem.md) ссылается на элемент, находящийся на другом диске.</span><span class="sxs-lookup"><span data-stu-id="8f94a-105">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="8f94a-106">Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="8f94a-106">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="8f94a-107">Элементы [**DriveItem**](driveitem.md) с аспектом **remoteItem**, не равным null, — это ресурсы, к которым предоставлен общий доступ, ресурсы, добавленные в хранилище OneDrive пользователя, или ресурсы в элементах, возвращенных из коллекций разнородных элементов (например, результатов поиска).</span><span class="sxs-lookup"><span data-stu-id="8f94a-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="8f94a-108">**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.</span><span class="sxs-lookup"><span data-stu-id="8f94a-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f94a-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f94a-109">JSON representation</span></span>

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
  "image" : { "@odata.type": "microsoft.graph.image" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="8f94a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f94a-110">Properties</span></span>

| <span data-ttu-id="8f94a-111">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8f94a-111">Property name</span></span>        | <span data-ttu-id="8f94a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8f94a-112">Type</span></span>                                | <span data-ttu-id="8f94a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8f94a-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8f94a-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="8f94a-114">createdBy</span></span>            | [<span data-ttu-id="8f94a-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8f94a-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="8f94a-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="8f94a-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f94a-118">createdDateTime</span></span>      | <span data-ttu-id="8f94a-119">Timestamp</span><span class="sxs-lookup"><span data-stu-id="8f94a-119">Timestamp</span></span>                           | <span data-ttu-id="8f94a-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="8f94a-122">file</span><span class="sxs-lookup"><span data-stu-id="8f94a-122">file</span></span>                 | [<span data-ttu-id="8f94a-123">File</span><span class="sxs-lookup"><span data-stu-id="8f94a-123">File</span></span>](file.md)                     | <span data-ttu-id="8f94a-p104">Указывает, что удаленный элемент является файлом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="8f94a-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="8f94a-126">fileSystemInfo</span></span>       | [<span data-ttu-id="8f94a-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="8f94a-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="8f94a-p105">Сведения об удаленном элементе из локальной файловой системы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="8f94a-130">folder</span><span class="sxs-lookup"><span data-stu-id="8f94a-130">folder</span></span>               | [<span data-ttu-id="8f94a-131">Folder</span><span class="sxs-lookup"><span data-stu-id="8f94a-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="8f94a-p106">Указывает, что удаленный элемент является папкой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="8f94a-134">id</span><span class="sxs-lookup"><span data-stu-id="8f94a-134">id</span></span>                   | <span data-ttu-id="8f94a-135">String</span><span class="sxs-lookup"><span data-stu-id="8f94a-135">String</span></span>                              | <span data-ttu-id="8f94a-p107">Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="8f94a-138">image</span><span class="sxs-lookup"><span data-stu-id="8f94a-138">image</span></span>                | [<span data-ttu-id="8f94a-139">Image</span><span class="sxs-lookup"><span data-stu-id="8f94a-139">Image</span></span>](image.md)                   | <span data-ttu-id="8f94a-p108">Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p108">Image metadata, if the item is an image. Read-only.</span></span>                                                                                               |
| <span data-ttu-id="8f94a-142">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8f94a-142">lastModifiedBy</span></span>       | [<span data-ttu-id="8f94a-143">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8f94a-143">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="8f94a-p109">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p109">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="8f94a-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f94a-146">lastModifiedDateTime</span></span> | <span data-ttu-id="8f94a-147">Timestamp</span><span class="sxs-lookup"><span data-stu-id="8f94a-147">Timestamp</span></span>                           | <span data-ttu-id="8f94a-p110">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p110">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="8f94a-150">name</span><span class="sxs-lookup"><span data-stu-id="8f94a-150">name</span></span>                 | <span data-ttu-id="8f94a-151">String</span><span class="sxs-lookup"><span data-stu-id="8f94a-151">String</span></span>                              | <span data-ttu-id="8f94a-p111">Необязательное свойство. Имя файла удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p111">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="8f94a-155">пакет</span><span class="sxs-lookup"><span data-stu-id="8f94a-155">package</span></span>              | [<span data-ttu-id="8f94a-156">Package</span><span class="sxs-lookup"><span data-stu-id="8f94a-156">Package</span></span>](package.md)               | <span data-ttu-id="8f94a-p112">В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p112">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="8f94a-160">parentReference</span><span class="sxs-lookup"><span data-stu-id="8f94a-160">parentReference</span></span>      | [<span data-ttu-id="8f94a-161">ItemReference</span><span class="sxs-lookup"><span data-stu-id="8f94a-161">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="8f94a-p113">Свойства родительского элемента удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p113">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="8f94a-164">общие</span><span class="sxs-lookup"><span data-stu-id="8f94a-164">shared</span></span>               | [<span data-ttu-id="8f94a-165">shared</span><span class="sxs-lookup"><span data-stu-id="8f94a-165">shared</span></span>](shared.md)                 | <span data-ttu-id="8f94a-p114">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p114">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="8f94a-168">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8f94a-168">sharepointIds</span></span>        | [<span data-ttu-id="8f94a-169">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="8f94a-169">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="8f94a-p115">Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p115">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="8f94a-172">size</span><span class="sxs-lookup"><span data-stu-id="8f94a-172">size</span></span>                 | <span data-ttu-id="8f94a-173">Int64</span><span class="sxs-lookup"><span data-stu-id="8f94a-173">Int64</span></span>                               | <span data-ttu-id="8f94a-p116">Размер удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p116">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="8f94a-176">specialFolder</span><span class="sxs-lookup"><span data-stu-id="8f94a-176">specialFolder</span></span>        | <span data-ttu-id="8f94a-177">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="8f94a-177">[specialFolder][]</span></span>                   | <span data-ttu-id="8f94a-p117">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p117">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>                                                                     |
| <span data-ttu-id="8f94a-180">video</span><span class="sxs-lookup"><span data-stu-id="8f94a-180">video</span></span>                | [<span data-ttu-id="8f94a-181">Video</span><span class="sxs-lookup"><span data-stu-id="8f94a-181">Video</span></span>](video.md)                   | <span data-ttu-id="8f94a-p118">Метаданные видео, если в роли элемента выступает видео. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p118">Video metadata, if the item is a video. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="8f94a-184">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="8f94a-184">webDavUrl</span></span>            | <span data-ttu-id="8f94a-185">Url</span><span class="sxs-lookup"><span data-stu-id="8f94a-185">Url</span></span>                                 | <span data-ttu-id="8f94a-186">URL-адрес, совместимый с протоколом DAV, для элемента.</span><span class="sxs-lookup"><span data-stu-id="8f94a-186">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="8f94a-187">webUrl</span><span class="sxs-lookup"><span data-stu-id="8f94a-187">webUrl</span></span>               | <span data-ttu-id="8f94a-188">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="8f94a-188">Url</span></span>                                 | <span data-ttu-id="8f94a-p119">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f94a-p119">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a><span data-ttu-id="8f94a-192">Заметки</span><span class="sxs-lookup"><span data-stu-id="8f94a-192">Remarks</span></span>

<span data-ttu-id="8f94a-193">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8f94a-193">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->

