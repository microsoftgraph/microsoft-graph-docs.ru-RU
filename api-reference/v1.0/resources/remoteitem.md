---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: remoteItem
ms.openlocfilehash: 549b0804a1d6449a71d2cc870836c0d044099a38
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264275"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="ab50d-102">Тип ресурса remoteItem</span><span class="sxs-lookup"><span data-stu-id="ab50d-102">RemoteItem resource type</span></span>

<span data-ttu-id="ab50d-p101">Ресурс **remoteItem** указывает, что элемент [**driveItem**](driveitem.md) ссылается на элемент, находящийся на другом диске. Этот ресурс предоставляет уникальные идентификаторы исходного диска и целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p101">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="ab50d-105">Элементы [**DriveItem**](driveitem.md) с аспектом **remoteItem**, не равным null, — это ресурсы, к которым предоставлен общий доступ, ресурсы, добавленные в хранилище OneDrive пользователя, или ресурсы в элементах, возвращенных из коллекций разнородных элементов (например, результатов поиска).</span><span class="sxs-lookup"><span data-stu-id="ab50d-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="ab50d-106">**Примечание.** В отличие от папок, расположенных на одном и том же диске, у элемента **driveItem**, перемещенного в удаленный элемент, может измениться значение `id`.</span><span class="sxs-lookup"><span data-stu-id="ab50d-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab50d-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab50d-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ab50d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab50d-108">Properties</span></span>

| <span data-ttu-id="ab50d-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ab50d-109">Property name</span></span>        | <span data-ttu-id="ab50d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ab50d-110">Type</span></span>                                | <span data-ttu-id="ab50d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab50d-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ab50d-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="ab50d-112">createdBy</span></span>            | [<span data-ttu-id="ab50d-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ab50d-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="ab50d-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="ab50d-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab50d-116">createdDateTime</span></span>      | <span data-ttu-id="ab50d-117">Timestamp</span><span class="sxs-lookup"><span data-stu-id="ab50d-117">Timestamp</span></span>                           | <span data-ttu-id="ab50d-p103">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="ab50d-120">file</span><span class="sxs-lookup"><span data-stu-id="ab50d-120">file</span></span>                 | [<span data-ttu-id="ab50d-121">Файл</span><span class="sxs-lookup"><span data-stu-id="ab50d-121">File</span></span>](file.md)                     | <span data-ttu-id="ab50d-p104">Указывает, что удаленный элемент является файлом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="ab50d-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="ab50d-124">fileSystemInfo</span></span>       | [<span data-ttu-id="ab50d-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="ab50d-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="ab50d-p105">Сведения об удаленном элементе из локальной файловой системы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="ab50d-128">folder</span><span class="sxs-lookup"><span data-stu-id="ab50d-128">folder</span></span>               | [<span data-ttu-id="ab50d-129">Папка</span><span class="sxs-lookup"><span data-stu-id="ab50d-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="ab50d-p106">Указывает, что удаленный элемент является папкой. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="ab50d-132">id</span><span class="sxs-lookup"><span data-stu-id="ab50d-132">id</span></span>                   | <span data-ttu-id="ab50d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ab50d-133">String</span></span>                              | <span data-ttu-id="ab50d-p107">Уникальный идентификатор для удаленного элемента на его диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="ab50d-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ab50d-136">lastModifiedBy</span></span>       | [<span data-ttu-id="ab50d-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ab50d-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="ab50d-p108">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="ab50d-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab50d-140">lastModifiedDateTime</span></span> | <span data-ttu-id="ab50d-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="ab50d-141">Timestamp</span></span>                           | <span data-ttu-id="ab50d-p109">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="ab50d-144">name</span><span class="sxs-lookup"><span data-stu-id="ab50d-144">name</span></span>                 | <span data-ttu-id="ab50d-145">Строка</span><span class="sxs-lookup"><span data-stu-id="ab50d-145">String</span></span>                              | <span data-ttu-id="ab50d-p110">Необязательное свойство. Имя файла удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="ab50d-149">package</span><span class="sxs-lookup"><span data-stu-id="ab50d-149">package</span></span>              | [<span data-ttu-id="ab50d-150">Пакет</span><span class="sxs-lookup"><span data-stu-id="ab50d-150">Package</span></span>](package.md)               | <span data-ttu-id="ab50d-p111">При наличии этого свойства оно указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="ab50d-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="ab50d-154">parentReference</span></span>      | [<span data-ttu-id="ab50d-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="ab50d-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="ab50d-p112">Свойства родительского элемента удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="ab50d-158">shared</span><span class="sxs-lookup"><span data-stu-id="ab50d-158">shared</span></span>               | [<span data-ttu-id="ab50d-159">shared</span><span class="sxs-lookup"><span data-stu-id="ab50d-159">shared</span></span>](shared.md)                 | <span data-ttu-id="ab50d-p113">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="ab50d-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ab50d-162">sharepointIds</span></span>        | [<span data-ttu-id="ab50d-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="ab50d-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="ab50d-p114">Обеспечивает взаимодействие между элементами в OneDrive для бизнеса и SharePoint с использованием полного набора идентификаторов элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="ab50d-166">size</span><span class="sxs-lookup"><span data-stu-id="ab50d-166">size</span></span>                 | <span data-ttu-id="ab50d-167">Int64</span><span class="sxs-lookup"><span data-stu-id="ab50d-167">Int64</span></span>                               | <span data-ttu-id="ab50d-p115">Размер удаленного элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="ab50d-170">specialFolder</span><span class="sxs-lookup"><span data-stu-id="ab50d-170">specialFolder</span></span>        | <span data-ttu-id="ab50d-171">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="ab50d-171">[specialFolder][]</span></span>                   | <span data-ttu-id="ab50d-p116">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p116">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>                                                                     |
| <span data-ttu-id="ab50d-174">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="ab50d-174">webDavUrl</span></span>            | <span data-ttu-id="ab50d-175">Url</span><span class="sxs-lookup"><span data-stu-id="ab50d-175">Url</span></span>                                 | <span data-ttu-id="ab50d-176">URL-адрес, совместимый с протоколом DAV, для элемента.</span><span class="sxs-lookup"><span data-stu-id="ab50d-176">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="ab50d-177">webUrl</span><span class="sxs-lookup"><span data-stu-id="ab50d-177">webUrl</span></span>               | <span data-ttu-id="ab50d-178">Url</span><span class="sxs-lookup"><span data-stu-id="ab50d-178">Url</span></span>                                 | <span data-ttu-id="ab50d-p117">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab50d-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

[specialFolder]: specialFolder.md

## <a name="remarks"></a><span data-ttu-id="ab50d-182">Примечания</span><span class="sxs-lookup"><span data-stu-id="ab50d-182">Remarks</span></span>

<span data-ttu-id="ab50d-183">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ab50d-183">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->