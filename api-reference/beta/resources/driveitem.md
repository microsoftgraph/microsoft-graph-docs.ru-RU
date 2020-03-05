---
author: JeremyKelley
description: Ресурс driveItem представляет файл, папку или другой элемент, хранящийся на диске.
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: fb6f3c92972255dc459263da1bb161de22e3f5b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505569"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="68c2c-103">Тип ресурса driveItem</span><span class="sxs-lookup"><span data-stu-id="68c2c-103">driveItem resource type</span></span>

<span data-ttu-id="68c2c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68c2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68c2c-p101">Ресурс **driveItem** представляет файл, папку или другой элемент, хранящийся на диске. Все объекты файловой системы в OneDrive и SharePoint возвращаются в виде ресурсов **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="68c2c-107">Обратиться к ресурсу **driveItem** можно двумя основными способами:</span><span class="sxs-lookup"><span data-stu-id="68c2c-107">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="68c2c-108">по уникальному идентификатору **driveItem** с помощью `drive/items/{item-id}`;</span><span class="sxs-lookup"><span data-stu-id="68c2c-108">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="68c2c-109">по пути файловой системы с помощью `/drive/root:/path/to/file`.</span><span class="sxs-lookup"><span data-stu-id="68c2c-109">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="68c2c-p102">У ресурсов **DriveItem** есть аспекты, смоделированные как свойства, которые предоставляют данные об идентификаторах и возможностях объекта driveItem. Пример:</span><span class="sxs-lookup"><span data-stu-id="68c2c-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="68c2c-112">У папок есть [**аспект folder**][folder].</span><span class="sxs-lookup"><span data-stu-id="68c2c-112">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="68c2c-113">У файлов есть [**аспект file**][file].</span><span class="sxs-lookup"><span data-stu-id="68c2c-113">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="68c2c-114">У изображений помимо аспекта file есть [**аспект image**][image].</span><span class="sxs-lookup"><span data-stu-id="68c2c-114">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="68c2c-115">У изображений, полученных с помощью камеры (фотографий), есть [**аспект photo**][photo], который определяет элемент как фотографию со свойствами времени съемки и устройства.</span><span class="sxs-lookup"><span data-stu-id="68c2c-115">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="68c2c-116">элементы с аспектом **folder** выполняют роль контейнеров элементов, поэтому у них есть ссылка `children`, указывающая на коллекцию объектов **driveItem** в папке.</span><span class="sxs-lookup"><span data-stu-id="68c2c-116">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68c2c-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="68c2c-117">JSON representation</span></span>

<span data-ttu-id="68c2c-118">Ниже представлено описание ресурса **driveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68c2c-118">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="68c2c-119">Ресурс **driveItem** является производным от ресурса [**baseItem**][baseItem] и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="68c2c-119">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{  
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "content": { "@odata.type": "Edm.Stream" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "pendingOperations": { "@odata.type": "microsoft.graph.pendingOperations" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "remoteItem": { "@odata.type": "microsoft.graph.remoteItem" },
  "root": { "@odata.type": "microsoft.graph.root" },
  "searchResult": { "@odata.type": "microsoft.graph.searchResult" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "string",

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "microsoft.graph.driveItemVersion"}],

  /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "eTag": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": {"@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "string",

  /* instance annotations */
  "@microsoft.graph.conflictBehavior": "string",
  "@microsoft.graph.downloadUrl": "url",
  "@microsoft.graph.sourceUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="68c2c-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="68c2c-120">Properties</span></span>

| <span data-ttu-id="68c2c-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="68c2c-121">Property</span></span>             | <span data-ttu-id="68c2c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="68c2c-122">Type</span></span>               | <span data-ttu-id="68c2c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="68c2c-123">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="68c2c-124">audio</span><span class="sxs-lookup"><span data-stu-id="68c2c-124">audio</span></span>                | <span data-ttu-id="68c2c-125">[audio][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-125">[audio][]</span></span>          | <span data-ttu-id="68c2c-p103">Метаданные звукового файла, если элемент — звуковой файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="68c2c-128">содержимое</span><span class="sxs-lookup"><span data-stu-id="68c2c-128">content</span></span>              | <span data-ttu-id="68c2c-129">Поток</span><span class="sxs-lookup"><span data-stu-id="68c2c-129">Stream</span></span>             | <span data-ttu-id="68c2c-130">Поток содержимого, если элемент представляет файл.</span><span class="sxs-lookup"><span data-stu-id="68c2c-130">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="68c2c-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="68c2c-131">createdBy</span></span>            | <span data-ttu-id="68c2c-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-132">[identitySet][]</span></span>    | <span data-ttu-id="68c2c-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="68c2c-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68c2c-135">createdDateTime</span></span>      | <span data-ttu-id="68c2c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68c2c-136">DateTimeOffset</span></span>     | <span data-ttu-id="68c2c-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="68c2c-139">cTag</span><span class="sxs-lookup"><span data-stu-id="68c2c-139">cTag</span></span>                 | <span data-ttu-id="68c2c-140">String</span><span class="sxs-lookup"><span data-stu-id="68c2c-140">String</span></span>             | <span data-ttu-id="68c2c-p106">ETag для содержимого элемента. Такой тег сущности не изменяется, если изменяются только метаданные. **Примечание.** Это свойство не возвращается, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="68c2c-145">deleted</span><span class="sxs-lookup"><span data-stu-id="68c2c-145">deleted</span></span>              | <span data-ttu-id="68c2c-146">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-146">[deleted][]</span></span>        | <span data-ttu-id="68c2c-p107">Сведения о состоянии удаления элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="68c2c-149">description</span><span class="sxs-lookup"><span data-stu-id="68c2c-149">description</span></span>          | <span data-ttu-id="68c2c-150">String</span><span class="sxs-lookup"><span data-stu-id="68c2c-150">String</span></span>             | <span data-ttu-id="68c2c-p108">Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive</span><span class="sxs-lookup"><span data-stu-id="68c2c-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="68c2c-154">eTag</span><span class="sxs-lookup"><span data-stu-id="68c2c-154">eTag</span></span>                 | <span data-ttu-id="68c2c-155">String</span><span class="sxs-lookup"><span data-stu-id="68c2c-155">String</span></span>             | <span data-ttu-id="68c2c-p109">Тег сущности для всего элемента (метаданные и содержимое). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="68c2c-158">file</span><span class="sxs-lookup"><span data-stu-id="68c2c-158">file</span></span>                 | <span data-ttu-id="68c2c-159">[file][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-159">[file][]</span></span>           | <span data-ttu-id="68c2c-p110">Файл метаданных, если в роли элемента выступает файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="68c2c-162">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="68c2c-162">fileSystemInfo</span></span>       | <span data-ttu-id="68c2c-163">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-163">[fileSystemInfo][]</span></span> | <span data-ttu-id="68c2c-p111">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="68c2c-166">folder</span><span class="sxs-lookup"><span data-stu-id="68c2c-166">folder</span></span>               | <span data-ttu-id="68c2c-167">[folder][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-167">[folder][]</span></span>         | <span data-ttu-id="68c2c-p112">Метаданные папки, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="68c2c-170">id</span><span class="sxs-lookup"><span data-stu-id="68c2c-170">id</span></span>                   | <span data-ttu-id="68c2c-171">Строка</span><span class="sxs-lookup"><span data-stu-id="68c2c-171">String</span></span>             | <span data-ttu-id="68c2c-p113">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="68c2c-174">изображение</span><span class="sxs-lookup"><span data-stu-id="68c2c-174">image</span></span>                | <span data-ttu-id="68c2c-175">[image][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-175">[image][]</span></span>          | <span data-ttu-id="68c2c-p114">Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="68c2c-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="68c2c-178">lastModifiedBy</span></span>       | <span data-ttu-id="68c2c-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-179">[identitySet][]</span></span>    | <span data-ttu-id="68c2c-p115">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="68c2c-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68c2c-182">lastModifiedDateTime</span></span> | <span data-ttu-id="68c2c-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68c2c-183">DateTimeOffset</span></span>     | <span data-ttu-id="68c2c-p116">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="68c2c-186">location</span><span class="sxs-lookup"><span data-stu-id="68c2c-186">location</span></span>             | <span data-ttu-id="68c2c-187">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-187">[geoCoordinates][]</span></span> | <span data-ttu-id="68c2c-p117">Метаданные местоположения, если в роли элемента выступают данные о местоположении. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="68c2c-190">name</span><span class="sxs-lookup"><span data-stu-id="68c2c-190">name</span></span>                 | <span data-ttu-id="68c2c-191">String</span><span class="sxs-lookup"><span data-stu-id="68c2c-191">String</span></span>             | <span data-ttu-id="68c2c-p118">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="68c2c-194">package</span><span class="sxs-lookup"><span data-stu-id="68c2c-194">package</span></span>              | <span data-ttu-id="68c2c-195">[package][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-195">[package][]</span></span>        | <span data-ttu-id="68c2c-p119">В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="68c2c-199">parentReference</span><span class="sxs-lookup"><span data-stu-id="68c2c-199">parentReference</span></span>      | <span data-ttu-id="68c2c-200">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-200">[itemReference][]</span></span>  | <span data-ttu-id="68c2c-p120">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="68c2c-203">пендингоператионс</span><span class="sxs-lookup"><span data-stu-id="68c2c-203">pendingOperations</span></span>    | <span data-ttu-id="68c2c-204">[пендингоператионс][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-204">[pendingOperations][]</span></span> | <span data-ttu-id="68c2c-205">Если указано, показывает, что одна или несколько операций, которые могут повлиять на состояние driveItem, ожидают завершения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-205">If present, indicates that indicates that one or more operations that may affect the state of the driveItem are pending completion.</span></span> <span data-ttu-id="68c2c-206">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-206">Read-only.</span></span>
| <span data-ttu-id="68c2c-207">Фотография
</span><span class="sxs-lookup"><span data-stu-id="68c2c-207">photo</span></span>                | <span data-ttu-id="68c2c-208">[photo][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-208">[photo][]</span></span>          | <span data-ttu-id="68c2c-p122">Метаданные фотографии, если в роли элемента выступает фотография. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p122">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="68c2c-211">publication</span><span class="sxs-lookup"><span data-stu-id="68c2c-211">publication</span></span>          | <span data-ttu-id="68c2c-212">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-212">[publicationFacet][]</span></span> | <span data-ttu-id="68c2c-213">Предоставляет сведения о состоянии элемента (опубликован или получен для изменения) в расположениях, поддерживающих такие действия.</span><span class="sxs-lookup"><span data-stu-id="68c2c-213">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="68c2c-214">Это свойство не возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="68c2c-214">This property is not returned by default.</span></span> <span data-ttu-id="68c2c-215">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-215">Read-only.</span></span> |
| <span data-ttu-id="68c2c-216">remoteItem</span><span class="sxs-lookup"><span data-stu-id="68c2c-216">remoteItem</span></span>           | <span data-ttu-id="68c2c-217">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-217">[remoteItem][]</span></span>     | <span data-ttu-id="68c2c-p124">Данные удаленного элемента, если элемент используется совместно на диске, но не на том, к которому получен доступ в данный момент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p124">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="68c2c-220">root</span><span class="sxs-lookup"><span data-stu-id="68c2c-220">root</span></span>                 | <span data-ttu-id="68c2c-221">[root][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-221">[root][]</span></span>           | <span data-ttu-id="68c2c-222">Ненулевое значение этого свойства указывает, что ресурс driveItem является самым верхним на диске.</span><span class="sxs-lookup"><span data-stu-id="68c2c-222">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="68c2c-223">searchResult</span><span class="sxs-lookup"><span data-stu-id="68c2c-223">searchResult</span></span>         | <span data-ttu-id="68c2c-224">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-224">[searchResult][]</span></span>   | <span data-ttu-id="68c2c-p125">Поиск метаданных, если элемент получен из результата поиска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p125">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="68c2c-227">общие</span><span class="sxs-lookup"><span data-stu-id="68c2c-227">shared</span></span>               | <span data-ttu-id="68c2c-228">[shared][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-228">[shared][]</span></span>         | <span data-ttu-id="68c2c-p126">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p126">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="68c2c-231">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="68c2c-231">sharepointIds</span></span>        | <span data-ttu-id="68c2c-232">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-232">[sharepointIds][]</span></span>  | <span data-ttu-id="68c2c-p127">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p127">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="68c2c-235">size</span><span class="sxs-lookup"><span data-stu-id="68c2c-235">size</span></span>                 | <span data-ttu-id="68c2c-236">Int64</span><span class="sxs-lookup"><span data-stu-id="68c2c-236">Int64</span></span>              | <span data-ttu-id="68c2c-p128">Размер элемента (в байтах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p128">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="68c2c-239">specialFolder</span><span class="sxs-lookup"><span data-stu-id="68c2c-239">specialFolder</span></span>        | <span data-ttu-id="68c2c-240">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-240">[specialFolder][]</span></span>  | <span data-ttu-id="68c2c-p129">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p129">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="68c2c-243">video</span><span class="sxs-lookup"><span data-stu-id="68c2c-243">video</span></span>                | <span data-ttu-id="68c2c-244">[video][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-244">[video][]</span></span>          | <span data-ttu-id="68c2c-p130">Метаданные видео, если в роли элемента выступает видео. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p130">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="68c2c-247">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="68c2c-247">webDavUrl</span></span>            | <span data-ttu-id="68c2c-248">Строка</span><span class="sxs-lookup"><span data-stu-id="68c2c-248">String</span></span>             | <span data-ttu-id="68c2c-249">URL-адрес элемента, совместимый с WebDAV.</span><span class="sxs-lookup"><span data-stu-id="68c2c-249">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="68c2c-250">webUrl</span><span class="sxs-lookup"><span data-stu-id="68c2c-250">webUrl</span></span>               | <span data-ttu-id="68c2c-251">String</span><span class="sxs-lookup"><span data-stu-id="68c2c-251">String</span></span>             | <span data-ttu-id="68c2c-p131">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p131">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="68c2c-p132">**Примечание.** Свойства тегов eTag и cTag по-разному действуют на контейнеры (папки). Значение cTag изменяется при изменении содержимого или метаданных любого потомка папки. Значение eTag изменяется только при изменении свойств папки, за исключением свойств, которые являются производными от потомков (например, свойство **childCount** или **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="68c2c-p132">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="68c2c-257">Отношения</span><span class="sxs-lookup"><span data-stu-id="68c2c-257">Relationships</span></span>

| <span data-ttu-id="68c2c-258">Связь</span><span class="sxs-lookup"><span data-stu-id="68c2c-258">Relationship</span></span>       | <span data-ttu-id="68c2c-259">Тип</span><span class="sxs-lookup"><span data-stu-id="68c2c-259">Type</span></span>                        | <span data-ttu-id="68c2c-260">Описание</span><span class="sxs-lookup"><span data-stu-id="68c2c-260">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="68c2c-261">activities</span><span class="sxs-lookup"><span data-stu-id="68c2c-261">activities</span></span>         | <span data-ttu-id="68c2c-262">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-262">[itemActivity][] collection</span></span> | <span data-ttu-id="68c2c-263">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="68c2c-263">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="68c2c-264">analytics</span><span class="sxs-lookup"><span data-stu-id="68c2c-264">analytics</span></span>          | <span data-ttu-id="68c2c-265">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-265">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="68c2c-266">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="68c2c-266">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="68c2c-267">children</span><span class="sxs-lookup"><span data-stu-id="68c2c-267">children</span></span>           | <span data-ttu-id="68c2c-268">Коллекция driveItem</span><span class="sxs-lookup"><span data-stu-id="68c2c-268">driveItem collection</span></span>        | <span data-ttu-id="68c2c-p133">Коллекция, содержащая объекты Item для непосредственных дочерних элементов Item. Дочерние элементы есть только у элементов, представляющих папки. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p133">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="68c2c-273">createdByUser</span><span class="sxs-lookup"><span data-stu-id="68c2c-273">createdByUser</span></span>      | <span data-ttu-id="68c2c-274">[user][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-274">[user][]</span></span>                    | <span data-ttu-id="68c2c-275">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="68c2c-275">Identity of the user who created the item.</span></span> <span data-ttu-id="68c2c-276">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-276">Read-only.</span></span>
| <span data-ttu-id="68c2c-277">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="68c2c-277">lastModifiedByUser</span></span> | <span data-ttu-id="68c2c-278">[user][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-278">[user][]</span></span>                    | <span data-ttu-id="68c2c-279">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="68c2c-279">Identity of the user who last modified the item.</span></span> <span data-ttu-id="68c2c-280">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-280">Read-only.</span></span>
| <span data-ttu-id="68c2c-281">listItem</span><span class="sxs-lookup"><span data-stu-id="68c2c-281">listItem</span></span>           | <span data-ttu-id="68c2c-282">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-282">[listItem][]</span></span>                | <span data-ttu-id="68c2c-283">Для дисков в SharePoint, связанный элемент библиотеки документов.</span><span class="sxs-lookup"><span data-stu-id="68c2c-283">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="68c2c-284">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-284">Read-only.</span></span> <span data-ttu-id="68c2c-285">Может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="68c2c-285">Nullable.</span></span>
| <span data-ttu-id="68c2c-286">permissions</span><span class="sxs-lookup"><span data-stu-id="68c2c-286">permissions</span></span>        | <span data-ttu-id="68c2c-287">Коллекция объектов [permission][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-287">[permission][] collection</span></span>   | <span data-ttu-id="68c2c-p137">Набор разрешений для элемента. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p137">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="68c2c-291">subscriptions</span><span class="sxs-lookup"><span data-stu-id="68c2c-291">subscriptions</span></span>      | <span data-ttu-id="68c2c-292">Коллекция [subscription][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-292">[subscription][] collection</span></span> | <span data-ttu-id="68c2c-293">Набор подписок на элемент.</span><span class="sxs-lookup"><span data-stu-id="68c2c-293">The set of subscriptions on the item.</span></span> <span data-ttu-id="68c2c-294">Поддерживается только в корне диска.</span><span class="sxs-lookup"><span data-stu-id="68c2c-294">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="68c2c-295">thumbnails</span><span class="sxs-lookup"><span data-stu-id="68c2c-295">thumbnails</span></span>         | <span data-ttu-id="68c2c-296">Коллекция объектов [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-296">[thumbnailSet][] collection</span></span> | <span data-ttu-id="68c2c-p139">Коллекция, содержащая объекты [ThumbnailSet][], связанные с элементом. Дополнительные сведения см. в статье о [получении эскизов][]. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p139">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="68c2c-301">versions</span><span class="sxs-lookup"><span data-stu-id="68c2c-301">versions</span></span>           | <span data-ttu-id="68c2c-302">Коллекция [driveItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-302">[driveItemVersion][] collection</span></span> | <span data-ttu-id="68c2c-303">Список предыдущих версий элемента.</span><span class="sxs-lookup"><span data-stu-id="68c2c-303">The list of previous versions of the item.</span></span> <span data-ttu-id="68c2c-304">Дополнительные сведения см. в статье, посвященной [получению предыдущих версий][].</span><span class="sxs-lookup"><span data-stu-id="68c2c-304">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="68c2c-305">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-305">Read-only.</span></span> <span data-ttu-id="68c2c-306">Может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="68c2c-306">Nullable.</span></span>
| <span data-ttu-id="68c2c-307">workbook</span><span class="sxs-lookup"><span data-stu-id="68c2c-307">workbook</span></span>           | <span data-ttu-id="68c2c-308">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-308">[workbook][]</span></span>                | <span data-ttu-id="68c2c-309">Для файлов, представляющих собой электронные таблицы Excel, получает доступ к API книги для работы с содержимым электронной таблицы.</span><span class="sxs-lookup"><span data-stu-id="68c2c-309">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="68c2c-310">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="68c2c-310">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="68c2c-311">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="68c2c-311">Instance Attributes</span></span>

<span data-ttu-id="68c2c-p142">Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p142">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="68c2c-314">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="68c2c-314">Property name</span></span>                     | <span data-ttu-id="68c2c-315">Тип</span><span class="sxs-lookup"><span data-stu-id="68c2c-315">Type</span></span>   | <span data-ttu-id="68c2c-316">Описание</span><span class="sxs-lookup"><span data-stu-id="68c2c-316">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="68c2c-317">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="68c2c-317">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="68c2c-318">string</span><span class="sxs-lookup"><span data-stu-id="68c2c-318">string</span></span> | <span data-ttu-id="68c2c-p143">Определяет поведение для разрешения конфликтов, возникающих при создании элементов. Вы можете использовать значения *fail*, *replace* или *rename*. Значение по умолчанию для метода PUT: *replace*. Элементы никогда не возвращаются с такой заметкой. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p143">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="68c2c-324">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="68c2c-324">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="68c2c-325">string</span><span class="sxs-lookup"><span data-stu-id="68c2c-325">string</span></span> | <span data-ttu-id="68c2c-p144">URL-адрес, который можно использовать для скачивания содержимого этого файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p144">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="68c2c-329">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="68c2c-329">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="68c2c-330">string</span><span class="sxs-lookup"><span data-stu-id="68c2c-330">string</span></span> | <span data-ttu-id="68c2c-p145">При создании запроса PUT такую заметку экземпляра можно использовать, чтобы указать службе скачать содержимое по URL-адресу и сохранить его как файл. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="68c2c-p145">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="68c2c-333">**Примечание.** Значение @microsoft.graph.downloadUrl — это краткосрочный URL-адрес, который не сохраняется в кэше.</span><span class="sxs-lookup"><span data-stu-id="68c2c-333">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="68c2c-334">URL-адрес будет доступен в течение короткого времени (1 час), после чего станет недействительным.</span><span class="sxs-lookup"><span data-stu-id="68c2c-334">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="68c2c-335">Удаление разрешений на доступ к файлу для пользователя может не сразу сделать URL-адрес недействительным.</span><span class="sxs-lookup"><span data-stu-id="68c2c-335">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

><span data-ttu-id="68c2c-336">**Примечание:** Параметр @microsoft.graph.conflictBehavior должен быть включен в URL-адрес, а не в текст запроса.</span><span class="sxs-lookup"><span data-stu-id="68c2c-336">**Note:** The parameter @microsoft.graph.conflictBehavior should be included in the URL instead of the body of the request.</span></span>

## <a name="methods"></a><span data-ttu-id="68c2c-337">Методы</span><span class="sxs-lookup"><span data-stu-id="68c2c-337">Methods</span></span>

| <span data-ttu-id="68c2c-338">Метод</span><span class="sxs-lookup"><span data-stu-id="68c2c-338">Method</span></span>                                                   | <span data-ttu-id="68c2c-339">Путь REST</span><span class="sxs-lookup"><span data-stu-id="68c2c-339">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="68c2c-340">Получение элемента</span><span class="sxs-lookup"><span data-stu-id="68c2c-340">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="68c2c-341">Список действий</span><span class="sxs-lookup"><span data-stu-id="68c2c-341">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="68c2c-342">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-342">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="68c2c-343">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="68c2c-343">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="68c2c-344">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="68c2c-344">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="68c2c-345">Список версий</span><span class="sxs-lookup"><span data-stu-id="68c2c-345">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="68c2c-346">Создание элемента</span><span class="sxs-lookup"><span data-stu-id="68c2c-346">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="68c2c-347">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="68c2c-347">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="68c2c-348">Отправка содержимого</span><span class="sxs-lookup"><span data-stu-id="68c2c-348">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="68c2c-349">Скачивание содержимого</span><span class="sxs-lookup"><span data-stu-id="68c2c-349">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="68c2c-350">[Скачивание файла в определенном формате][download-format]</span><span class="sxs-lookup"><span data-stu-id="68c2c-350">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="68c2c-351">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="68c2c-351">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="68c2c-352">Восстановление элемента</span><span class="sxs-lookup"><span data-stu-id="68c2c-352">Restore item</span></span>](../api/driveitem-restore.md)              | `POST /drive/items/{item-id}/restore`
| [<span data-ttu-id="68c2c-353">Перемещение элемента</span><span class="sxs-lookup"><span data-stu-id="68c2c-353">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="68c2c-354">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="68c2c-354">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="68c2c-355">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="68c2c-355">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="68c2c-356">Перечисление изменений на диске</span><span class="sxs-lookup"><span data-stu-id="68c2c-356">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="68c2c-357">Перечисление эскизов</span><span class="sxs-lookup"><span data-stu-id="68c2c-357">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="68c2c-358">Создание ссылки совместного доступа</span><span class="sxs-lookup"><span data-stu-id="68c2c-358">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="68c2c-359">Добавление разрешений</span><span class="sxs-lookup"><span data-stu-id="68c2c-359">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="68c2c-360">Список разрешений</span><span class="sxs-lookup"><span data-stu-id="68c2c-360">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="68c2c-361">Удаление разрешения</span><span class="sxs-lookup"><span data-stu-id="68c2c-361">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="68c2c-362">[Получение канала WebSocket][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="68c2c-362">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="68c2c-363">[Предварительный просмотр элемента][item-preview]</span><span class="sxs-lookup"><span data-stu-id="68c2c-363">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="68c2c-366">Заметки</span><span class="sxs-lookup"><span data-stu-id="68c2c-366">Remarks</span></span>

<span data-ttu-id="68c2c-367">В OneDrive для бизнеса и библиотеках документов SharePoint свойство **cTag** не возвращается, если у ресурса **driveItem** есть аспект [folder][].</span><span class="sxs-lookup"><span data-stu-id="68c2c-367">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[получение предыдущих версий]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[получение эскизов]: ../api/driveitem-list-thumbnails.md
[getting thumbnails]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[пендингоператионс]: pendingoperations.md
[pendingOperations]: pendingoperations.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[subscription]: subscription.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[workbook]: workbook.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": {
    "Resources/Item": "#"
  },
  "suppressions": []
}
-->
