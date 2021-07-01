---
author: JeremyKelley
description: Ресурс driveItem представляет файл, папку или другой элемент, хранящийся на диске.
title: driveItem
localization_priority: Normal
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 1be483b8309944c1a323c7274efe55b04feb6c3d
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236252"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="e65ee-103">Тип ресурса driveItem</span><span class="sxs-lookup"><span data-stu-id="e65ee-103">driveItem resource type</span></span>

<span data-ttu-id="e65ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e65ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e65ee-105">Ресурс **driveItem** представляет файл, папку или другой элемент, хранящийся на диске.</span><span class="sxs-lookup"><span data-stu-id="e65ee-105">The **driveItem** resource represents a file, folder, or other item stored in a drive.</span></span>

<span data-ttu-id="e65ee-106">Все объекты файловой системы в OneDrive и SharePoint возвращаются в виде ресурсов **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="e65ee-106">All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span> <span data-ttu-id="e65ee-107">Элементы в библиотеках документов SharePoint могут быть представлены как ресурсы [listItem][] или **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="e65ee-107">Items in SharePoint document libraries can be represented as [listItem][] or **driveItem** resources.</span></span>

<span data-ttu-id="e65ee-108">Обратиться к ресурсу **driveItem** можно двумя основными способами:</span><span class="sxs-lookup"><span data-stu-id="e65ee-108">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="e65ee-109">по уникальному идентификатору **driveItem** с помощью `drive/items/{item-id}`;</span><span class="sxs-lookup"><span data-stu-id="e65ee-109">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="e65ee-110">по пути файловой системы с помощью `/drive/root:/path/to/file`.</span><span class="sxs-lookup"><span data-stu-id="e65ee-110">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="e65ee-p102">У ресурсов **DriveItem** есть аспекты, смоделированные как свойства, которые предоставляют данные об идентификаторах и возможностях объекта driveItem. Пример:</span><span class="sxs-lookup"><span data-stu-id="e65ee-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="e65ee-113">У папок есть [**аспект folder**][folder].</span><span class="sxs-lookup"><span data-stu-id="e65ee-113">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="e65ee-114">У файлов есть [**аспект file**][file].</span><span class="sxs-lookup"><span data-stu-id="e65ee-114">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="e65ee-115">У изображений помимо аспекта file есть [**аспект image**][image].</span><span class="sxs-lookup"><span data-stu-id="e65ee-115">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="e65ee-116">У изображений, полученных с помощью камеры (фотографий), есть [**аспект photo**][photo], который определяет элемент как фотографию со свойствами времени съемки и устройства.</span><span class="sxs-lookup"><span data-stu-id="e65ee-116">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="e65ee-117">элементы с аспектом **folder** выполняют роль контейнеров элементов, поэтому у них есть ссылка `children`, указывающая на коллекцию объектов **driveItem** в папке.</span><span class="sxs-lookup"><span data-stu-id="e65ee-117">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e65ee-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e65ee-118">JSON representation</span></span>

<span data-ttu-id="e65ee-119">Ниже представлено описание ресурса **driveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e65ee-119">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="e65ee-120">Ресурс **driveItem** является производным от ресурса [**baseItem**][baseItem] и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="e65ee-120">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds", "source", "media"],
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
  "media": { "@odata.type": "microsoft.graph.media" },
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
  "source": { "@odata.type": "microsoft.graph.driveItemSource" },
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

## <a name="properties"></a><span data-ttu-id="e65ee-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="e65ee-121">Properties</span></span>

| <span data-ttu-id="e65ee-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="e65ee-122">Property</span></span>             | <span data-ttu-id="e65ee-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e65ee-123">Type</span></span>               | <span data-ttu-id="e65ee-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e65ee-124">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="e65ee-125">audio</span><span class="sxs-lookup"><span data-stu-id="e65ee-125">audio</span></span>                | <span data-ttu-id="e65ee-126">[audio][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-126">[audio][]</span></span>          | <span data-ttu-id="e65ee-p103">Метаданные звукового файла, если элемент — звуковой файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="e65ee-129">содержимое</span><span class="sxs-lookup"><span data-stu-id="e65ee-129">content</span></span>              | <span data-ttu-id="e65ee-130">Поток</span><span class="sxs-lookup"><span data-stu-id="e65ee-130">Stream</span></span>             | <span data-ttu-id="e65ee-131">Поток содержимого, если элемент представляет файл.</span><span class="sxs-lookup"><span data-stu-id="e65ee-131">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="e65ee-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="e65ee-132">createdBy</span></span>            | <span data-ttu-id="e65ee-133">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-133">[identitySet][]</span></span>    | <span data-ttu-id="e65ee-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="e65ee-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e65ee-136">createdDateTime</span></span>      | <span data-ttu-id="e65ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e65ee-137">DateTimeOffset</span></span>     | <span data-ttu-id="e65ee-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="e65ee-140">cTag</span><span class="sxs-lookup"><span data-stu-id="e65ee-140">cTag</span></span>                 | <span data-ttu-id="e65ee-141">String</span><span class="sxs-lookup"><span data-stu-id="e65ee-141">String</span></span>             | <span data-ttu-id="e65ee-p106">ETag для содержимого элемента. Такой тег сущности не изменяется, если изменяются только метаданные. **Примечание.** Это свойство не возвращается, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="e65ee-146">deleted</span><span class="sxs-lookup"><span data-stu-id="e65ee-146">deleted</span></span>              | <span data-ttu-id="e65ee-147">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-147">[deleted][]</span></span>        | <span data-ttu-id="e65ee-p107">Сведения о состоянии удаления элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="e65ee-150">description</span><span class="sxs-lookup"><span data-stu-id="e65ee-150">description</span></span>          | <span data-ttu-id="e65ee-151">String</span><span class="sxs-lookup"><span data-stu-id="e65ee-151">String</span></span>             | <span data-ttu-id="e65ee-p108">Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive</span><span class="sxs-lookup"><span data-stu-id="e65ee-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="e65ee-155">eTag</span><span class="sxs-lookup"><span data-stu-id="e65ee-155">eTag</span></span>                 | <span data-ttu-id="e65ee-156">String</span><span class="sxs-lookup"><span data-stu-id="e65ee-156">String</span></span>             | <span data-ttu-id="e65ee-p109">Тег сущности для всего элемента (метаданные и содержимое). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="e65ee-159">file</span><span class="sxs-lookup"><span data-stu-id="e65ee-159">file</span></span>                 | <span data-ttu-id="e65ee-160">[file][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-160">[file][]</span></span>           | <span data-ttu-id="e65ee-p110">Файл метаданных, если в роли элемента выступает файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="e65ee-163">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="e65ee-163">fileSystemInfo</span></span>       | <span data-ttu-id="e65ee-164">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-164">[fileSystemInfo][]</span></span> | <span data-ttu-id="e65ee-p111">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="e65ee-167">folder</span><span class="sxs-lookup"><span data-stu-id="e65ee-167">folder</span></span>               | <span data-ttu-id="e65ee-168">[folder][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-168">[folder][]</span></span>         | <span data-ttu-id="e65ee-p112">Метаданные папки, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="e65ee-171">id</span><span class="sxs-lookup"><span data-stu-id="e65ee-171">id</span></span>                   | <span data-ttu-id="e65ee-172">String</span><span class="sxs-lookup"><span data-stu-id="e65ee-172">String</span></span>             | <span data-ttu-id="e65ee-p113">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="e65ee-175">изображение</span><span class="sxs-lookup"><span data-stu-id="e65ee-175">image</span></span>                | <span data-ttu-id="e65ee-176">[image][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-176">[image][]</span></span>          | <span data-ttu-id="e65ee-p114">Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="e65ee-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e65ee-179">lastModifiedBy</span></span>       | <span data-ttu-id="e65ee-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-180">[identitySet][]</span></span>    | <span data-ttu-id="e65ee-p115">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="e65ee-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e65ee-183">lastModifiedDateTime</span></span> | <span data-ttu-id="e65ee-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e65ee-184">DateTimeOffset</span></span>     | <span data-ttu-id="e65ee-p116">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e65ee-187">location</span><span class="sxs-lookup"><span data-stu-id="e65ee-187">location</span></span>             | <span data-ttu-id="e65ee-188">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-188">[geoCoordinates][]</span></span> | <span data-ttu-id="e65ee-p117">Метаданные местоположения, если в роли элемента выступают данные о местоположении. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="e65ee-191">мультимедиа</span><span class="sxs-lookup"><span data-stu-id="e65ee-191">media</span></span>                | <span data-ttu-id="e65ee-192">[media][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-192">[media][]</span></span>          | <span data-ttu-id="e65ee-193">Сведения о элементе мультимедиа (аудио или видео).</span><span class="sxs-lookup"><span data-stu-id="e65ee-193">Information about the media (audio or video) item.</span></span> <span data-ttu-id="e65ee-194">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="e65ee-194">Read-write.</span></span> <span data-ttu-id="e65ee-195">Только на OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e65ee-195">Only on OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="e65ee-196">name</span><span class="sxs-lookup"><span data-stu-id="e65ee-196">name</span></span>                 | <span data-ttu-id="e65ee-197">String</span><span class="sxs-lookup"><span data-stu-id="e65ee-197">String</span></span>             | <span data-ttu-id="e65ee-p119">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="e65ee-200">package</span><span class="sxs-lookup"><span data-stu-id="e65ee-200">package</span></span>              | <span data-ttu-id="e65ee-201">[package][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-201">[package][]</span></span>        | <span data-ttu-id="e65ee-p120">В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="e65ee-205">parentReference</span><span class="sxs-lookup"><span data-stu-id="e65ee-205">parentReference</span></span>      | <span data-ttu-id="e65ee-206">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-206">[itemReference][]</span></span>  | <span data-ttu-id="e65ee-p121">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="e65ee-209">pendingOperations</span><span class="sxs-lookup"><span data-stu-id="e65ee-209">pendingOperations</span></span>    | <span data-ttu-id="e65ee-210">[pendingOperations][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-210">[pendingOperations][]</span></span> | <span data-ttu-id="e65ee-211">При этом указывается, что одна или несколько операций, которые могут повлиять на состояние driveItem, находятся в ожидании завершения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-211">If present, indicates that indicates that one or more operations that may affect the state of the driveItem are pending completion.</span></span> <span data-ttu-id="e65ee-212">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-212">Read-only.</span></span>
| <span data-ttu-id="e65ee-213">photo;</span><span class="sxs-lookup"><span data-stu-id="e65ee-213">photo</span></span>                | <span data-ttu-id="e65ee-214">[photo][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-214">[photo][]</span></span>          | <span data-ttu-id="e65ee-p123">Метаданные фотографии, если в роли элемента выступает фотография. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p123">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="e65ee-217">publication</span><span class="sxs-lookup"><span data-stu-id="e65ee-217">publication</span></span>          | <span data-ttu-id="e65ee-218">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-218">[publicationFacet][]</span></span> | <span data-ttu-id="e65ee-219">Предоставляет сведения о состоянии элемента (опубликован или получен для изменения) в расположениях, поддерживающих такие действия.</span><span class="sxs-lookup"><span data-stu-id="e65ee-219">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="e65ee-220">Это свойство не возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e65ee-220">This property is not returned by default.</span></span> <span data-ttu-id="e65ee-221">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-221">Read-only.</span></span> |
| <span data-ttu-id="e65ee-222">remoteItem</span><span class="sxs-lookup"><span data-stu-id="e65ee-222">remoteItem</span></span>           | <span data-ttu-id="e65ee-223">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-223">[remoteItem][]</span></span>     | <span data-ttu-id="e65ee-p125">Данные удаленного элемента, если элемент используется совместно на диске, но не на том, к которому получен доступ в данный момент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p125">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="e65ee-226">root</span><span class="sxs-lookup"><span data-stu-id="e65ee-226">root</span></span>                 | <span data-ttu-id="e65ee-227">[root][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-227">[root][]</span></span>           | <span data-ttu-id="e65ee-228">Ненулевое значение этого свойства указывает, что ресурс driveItem является самым верхним на диске.</span><span class="sxs-lookup"><span data-stu-id="e65ee-228">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="e65ee-229">searchResult</span><span class="sxs-lookup"><span data-stu-id="e65ee-229">searchResult</span></span>         | <span data-ttu-id="e65ee-230">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-230">[searchResult][]</span></span>   | <span data-ttu-id="e65ee-p126">Поиск метаданных, если элемент получен из результата поиска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p126">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="e65ee-233">общие</span><span class="sxs-lookup"><span data-stu-id="e65ee-233">shared</span></span>               | <span data-ttu-id="e65ee-234">[shared][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-234">[shared][]</span></span>         | <span data-ttu-id="e65ee-p127">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p127">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="e65ee-237">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="e65ee-237">sharepointIds</span></span>        | <span data-ttu-id="e65ee-238">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-238">[sharepointIds][]</span></span>  | <span data-ttu-id="e65ee-p128">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p128">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="e65ee-241">size</span><span class="sxs-lookup"><span data-stu-id="e65ee-241">size</span></span>                 | <span data-ttu-id="e65ee-242">Int64</span><span class="sxs-lookup"><span data-stu-id="e65ee-242">Int64</span></span>              | <span data-ttu-id="e65ee-p129">Размер элемента (в байтах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p129">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="e65ee-245">specialFolder</span><span class="sxs-lookup"><span data-stu-id="e65ee-245">specialFolder</span></span>        | <span data-ttu-id="e65ee-246">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-246">[specialFolder][]</span></span>  | <span data-ttu-id="e65ee-p130">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p130">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="e65ee-249">source</span><span class="sxs-lookup"><span data-stu-id="e65ee-249">source</span></span>               | <span data-ttu-id="e65ee-250">[driveItemSource][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-250">[driveItemSource][]</span></span>| <span data-ttu-id="e65ee-251">Сведения об источнике элемента диска.</span><span class="sxs-lookup"><span data-stu-id="e65ee-251">Information about the drive item source.</span></span> <span data-ttu-id="e65ee-252">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-252">Read-only.</span></span> <span data-ttu-id="e65ee-253">Только на OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e65ee-253">Only on OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="e65ee-254">video</span><span class="sxs-lookup"><span data-stu-id="e65ee-254">video</span></span>                | <span data-ttu-id="e65ee-255">[video][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-255">[video][]</span></span>          | <span data-ttu-id="e65ee-p132">Метаданные видео, если в роли элемента выступает видео. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p132">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="e65ee-258">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="e65ee-258">webDavUrl</span></span>            | <span data-ttu-id="e65ee-259">Строка</span><span class="sxs-lookup"><span data-stu-id="e65ee-259">String</span></span>             | <span data-ttu-id="e65ee-260">URL-адрес элемента, совместимый с WebDAV.</span><span class="sxs-lookup"><span data-stu-id="e65ee-260">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="e65ee-261">webUrl</span><span class="sxs-lookup"><span data-stu-id="e65ee-261">webUrl</span></span>               | <span data-ttu-id="e65ee-262">String</span><span class="sxs-lookup"><span data-stu-id="e65ee-262">String</span></span>             | <span data-ttu-id="e65ee-p133">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p133">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="e65ee-p134">**Примечание.** Свойства тегов eTag и cTag по-разному действуют на контейнеры (папки). Значение cTag изменяется при изменении содержимого или метаданных любого потомка папки. Значение eTag изменяется только при изменении свойств папки, за исключением свойств, которые являются производными от потомков (например, свойство **childCount** или **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="e65ee-p134">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="e65ee-268">Отношения</span><span class="sxs-lookup"><span data-stu-id="e65ee-268">Relationships</span></span>

| <span data-ttu-id="e65ee-269">Связь</span><span class="sxs-lookup"><span data-stu-id="e65ee-269">Relationship</span></span>       | <span data-ttu-id="e65ee-270">Тип</span><span class="sxs-lookup"><span data-stu-id="e65ee-270">Type</span></span>                        | <span data-ttu-id="e65ee-271">Описание</span><span class="sxs-lookup"><span data-stu-id="e65ee-271">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="e65ee-272">activities</span><span class="sxs-lookup"><span data-stu-id="e65ee-272">activities</span></span>         | <span data-ttu-id="e65ee-273">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-273">[itemActivity][] collection</span></span> | <span data-ttu-id="e65ee-274">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="e65ee-274">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="e65ee-275">analytics</span><span class="sxs-lookup"><span data-stu-id="e65ee-275">analytics</span></span>          | <span data-ttu-id="e65ee-276">Ресурс [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-276">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="e65ee-277">Аналитические данные о действиях просмотра, выполненных для элемента.</span><span class="sxs-lookup"><span data-stu-id="e65ee-277">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="e65ee-278">children</span><span class="sxs-lookup"><span data-stu-id="e65ee-278">children</span></span>           | <span data-ttu-id="e65ee-279">Коллекция driveItem</span><span class="sxs-lookup"><span data-stu-id="e65ee-279">driveItem collection</span></span>        | <span data-ttu-id="e65ee-p135">Коллекция, содержащая объекты Item для непосредственных дочерних элементов Item. Дочерние элементы есть только у элементов, представляющих папки. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p135">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="e65ee-284">createdByUser</span><span class="sxs-lookup"><span data-stu-id="e65ee-284">createdByUser</span></span>      | <span data-ttu-id="e65ee-285">[user][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-285">[user][]</span></span>                    | <span data-ttu-id="e65ee-286">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="e65ee-286">Identity of the user who created the item.</span></span> <span data-ttu-id="e65ee-287">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-287">Read-only.</span></span>
| <span data-ttu-id="e65ee-288">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="e65ee-288">lastModifiedByUser</span></span> | <span data-ttu-id="e65ee-289">[user][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-289">[user][]</span></span>                    | <span data-ttu-id="e65ee-290">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="e65ee-290">Identity of the user who last modified the item.</span></span> <span data-ttu-id="e65ee-291">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-291">Read-only.</span></span>
| <span data-ttu-id="e65ee-292">listItem</span><span class="sxs-lookup"><span data-stu-id="e65ee-292">listItem</span></span>           | <span data-ttu-id="e65ee-293">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-293">[listItem][]</span></span>                | <span data-ttu-id="e65ee-294">Для дисков в SharePoint, связанный элемент библиотеки документов.</span><span class="sxs-lookup"><span data-stu-id="e65ee-294">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="e65ee-295">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-295">Read-only.</span></span> <span data-ttu-id="e65ee-296">Может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="e65ee-296">Nullable.</span></span>
| <span data-ttu-id="e65ee-297">permissions</span><span class="sxs-lookup"><span data-stu-id="e65ee-297">permissions</span></span>        | <span data-ttu-id="e65ee-298">Коллекция объектов [permission][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-298">[permission][] collection</span></span>   | <span data-ttu-id="e65ee-p139">Набор разрешений для элемента. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p139">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="e65ee-302">subscriptions</span><span class="sxs-lookup"><span data-stu-id="e65ee-302">subscriptions</span></span>      | <span data-ttu-id="e65ee-303">Коллекция [subscription][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-303">[subscription][] collection</span></span> | <span data-ttu-id="e65ee-304">Набор подписок на элемент.</span><span class="sxs-lookup"><span data-stu-id="e65ee-304">The set of subscriptions on the item.</span></span> <span data-ttu-id="e65ee-305">Поддерживается только в корне диска.</span><span class="sxs-lookup"><span data-stu-id="e65ee-305">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="e65ee-306">thumbnails</span><span class="sxs-lookup"><span data-stu-id="e65ee-306">thumbnails</span></span>         | <span data-ttu-id="e65ee-307">Коллекция объектов [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-307">[thumbnailSet][] collection</span></span> | <span data-ttu-id="e65ee-p141">Коллекция, содержащая объекты [ThumbnailSet][], связанные с элементом. Дополнительные сведения см. в статье о [получении эскизов][]. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p141">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="e65ee-312">versions</span><span class="sxs-lookup"><span data-stu-id="e65ee-312">versions</span></span>           | <span data-ttu-id="e65ee-313">Коллекция [driveItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-313">[driveItemVersion][] collection</span></span> | <span data-ttu-id="e65ee-314">Список предыдущих версий элемента.</span><span class="sxs-lookup"><span data-stu-id="e65ee-314">The list of previous versions of the item.</span></span> <span data-ttu-id="e65ee-315">Дополнительные сведения см. в статье, посвященной [получению предыдущих версий][].</span><span class="sxs-lookup"><span data-stu-id="e65ee-315">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="e65ee-316">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-316">Read-only.</span></span> <span data-ttu-id="e65ee-317">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e65ee-317">Nullable.</span></span>
| <span data-ttu-id="e65ee-318">workbook</span><span class="sxs-lookup"><span data-stu-id="e65ee-318">workbook</span></span>           | <span data-ttu-id="e65ee-319">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-319">[workbook][]</span></span>                | <span data-ttu-id="e65ee-320">Для файлов, представляющих собой электронные таблицы Excel, получает доступ к API книги для работы с содержимым электронной таблицы.</span><span class="sxs-lookup"><span data-stu-id="e65ee-320">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="e65ee-321">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e65ee-321">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="e65ee-322">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="e65ee-322">Instance Attributes</span></span>

<span data-ttu-id="e65ee-p144">Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p144">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="e65ee-325">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e65ee-325">Property name</span></span>                     | <span data-ttu-id="e65ee-326">Тип</span><span class="sxs-lookup"><span data-stu-id="e65ee-326">Type</span></span>   | <span data-ttu-id="e65ee-327">Описание</span><span class="sxs-lookup"><span data-stu-id="e65ee-327">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="e65ee-328">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="e65ee-328">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="e65ee-329">string</span><span class="sxs-lookup"><span data-stu-id="e65ee-329">string</span></span> | <span data-ttu-id="e65ee-p145">Определяет поведение для разрешения конфликтов, возникающих при создании элементов. Вы можете использовать значения *fail*, *replace* или *rename*. Значение по умолчанию для метода PUT: *replace*. Элементы никогда не возвращаются с такой заметкой. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p145">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="e65ee-335">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="e65ee-335">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="e65ee-336">string</span><span class="sxs-lookup"><span data-stu-id="e65ee-336">string</span></span> | <span data-ttu-id="e65ee-p146">URL-адрес, который можно использовать для скачивания содержимого этого файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p146">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="e65ee-340">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="e65ee-340">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="e65ee-341">string</span><span class="sxs-lookup"><span data-stu-id="e65ee-341">string</span></span> | <span data-ttu-id="e65ee-p147">При создании запроса PUT такую заметку экземпляра можно использовать, чтобы указать службе скачать содержимое по URL-адресу и сохранить его как файл. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="e65ee-p147">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="e65ee-344">**Примечание.** Значение @microsoft.graph.downloadUrl — это краткосрочный URL-адрес, который не сохраняется в кэше.</span><span class="sxs-lookup"><span data-stu-id="e65ee-344">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="e65ee-345">URL-адрес будет доступен в течение короткого времени (1 час), после чего станет недействительным.</span><span class="sxs-lookup"><span data-stu-id="e65ee-345">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="e65ee-346">Удаление разрешений на доступ к файлу для пользователя может не сразу сделать URL-адрес недействительным.</span><span class="sxs-lookup"><span data-stu-id="e65ee-346">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

><span data-ttu-id="e65ee-347">**Примечание:** Параметр @microsoft.graph.conflictBehavior должен быть включен в URL-адрес, а не в текст запроса.</span><span class="sxs-lookup"><span data-stu-id="e65ee-347">**Note:** The parameter @microsoft.graph.conflictBehavior should be included in the URL instead of the body of the request.</span></span>

## <a name="methods"></a><span data-ttu-id="e65ee-348">Методы</span><span class="sxs-lookup"><span data-stu-id="e65ee-348">Methods</span></span>

| <span data-ttu-id="e65ee-349">Метод</span><span class="sxs-lookup"><span data-stu-id="e65ee-349">Method</span></span>                                                   | <span data-ttu-id="e65ee-350">Путь REST</span><span class="sxs-lookup"><span data-stu-id="e65ee-350">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="e65ee-351">Получение элемента</span><span class="sxs-lookup"><span data-stu-id="e65ee-351">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="e65ee-352">Список действий</span><span class="sxs-lookup"><span data-stu-id="e65ee-352">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="e65ee-353">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-353">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="e65ee-354">[Получение действий по интервалу][]</span><span class="sxs-lookup"><span data-stu-id="e65ee-354">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="e65ee-355">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="e65ee-355">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="e65ee-356">Список версий</span><span class="sxs-lookup"><span data-stu-id="e65ee-356">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="e65ee-357">Создание элемента</span><span class="sxs-lookup"><span data-stu-id="e65ee-357">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="e65ee-358">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="e65ee-358">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="e65ee-359">Отправка содержимого</span><span class="sxs-lookup"><span data-stu-id="e65ee-359">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="e65ee-360">Скачивание содержимого</span><span class="sxs-lookup"><span data-stu-id="e65ee-360">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="e65ee-361">[Скачивание файла в определенном формате][download-format]</span><span class="sxs-lookup"><span data-stu-id="e65ee-361">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="e65ee-362">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="e65ee-362">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="e65ee-363">Элемент восстановления</span><span class="sxs-lookup"><span data-stu-id="e65ee-363">Restore item</span></span>](../api/driveitem-restore.md)              | `POST /drive/items/{item-id}/restore`
| [<span data-ttu-id="e65ee-364">Перемещение элемента</span><span class="sxs-lookup"><span data-stu-id="e65ee-364">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="e65ee-365">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="e65ee-365">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="e65ee-366">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="e65ee-366">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="e65ee-367">Перечисление изменений на диске</span><span class="sxs-lookup"><span data-stu-id="e65ee-367">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="e65ee-368">Следуйте элементу</span><span class="sxs-lookup"><span data-stu-id="e65ee-368">Follow item</span></span>](../api/driveitem-follow.md)                | `POST /drives/{drive-id}/items/{item-id}/follow`
| [<span data-ttu-id="e65ee-369">Элемент unfollow</span><span class="sxs-lookup"><span data-stu-id="e65ee-369">Unfollow item</span></span>](../api/driveitem-unfollow.md)            | `POST /drives/{drive-id}/items/{item-id}/unfollow`
| [<span data-ttu-id="e65ee-370">Перечисление эскизов</span><span class="sxs-lookup"><span data-stu-id="e65ee-370">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="e65ee-371">Создание ссылки совместного доступа</span><span class="sxs-lookup"><span data-stu-id="e65ee-371">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="e65ee-372">Добавление разрешений</span><span class="sxs-lookup"><span data-stu-id="e65ee-372">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="e65ee-373">Список разрешений</span><span class="sxs-lookup"><span data-stu-id="e65ee-373">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="e65ee-374">Удаление разрешения</span><span class="sxs-lookup"><span data-stu-id="e65ee-374">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="e65ee-375">[Получение канала WebSocket][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="e65ee-375">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="e65ee-376">[Предварительный просмотр элемента][item-preview]</span><span class="sxs-lookup"><span data-stu-id="e65ee-376">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`
| [<span data-ttu-id="e65ee-377">Регистрация</span><span class="sxs-lookup"><span data-stu-id="e65ee-377">Check in</span></span>](../api/driveitem-checkin.md)                  | `POST /drives/{driveId}/items/{itemId}/checkin`
| [<span data-ttu-id="e65ee-378">Выписка</span><span class="sxs-lookup"><span data-stu-id="e65ee-378">Check out</span></span>](../api/driveitem-checkout.md)                | `POST /drives/{driveId}/items/{itemId}/checkout`
| [<span data-ttu-id="e65ee-379">Отоимка грантов</span><span class="sxs-lookup"><span data-stu-id="e65ee-379">Revoke grants</span></span>](../api/permission-revokegrants.md)   | `PATCH /drive/items/{item-id}/permissions/{perm-id}/revokeGrants`

[item-preview]: ../api/driveitem-preview.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервалу]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="e65ee-382">Заметки</span><span class="sxs-lookup"><span data-stu-id="e65ee-382">Remarks</span></span>

<span data-ttu-id="e65ee-383">В OneDrive для бизнеса и библиотеках документов SharePoint свойство **cTag** не возвращается, если у ресурса **driveItem** есть аспект [folder][].</span><span class="sxs-lookup"><span data-stu-id="e65ee-383">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemSource]: driveItemSource.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[получение предыдущих версий]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[получение эскизов]: ../api/driveitem-list-thumbnails.md
[getting thumbnails]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
[listItem]: listitem.md
[media]: media.md
[package]: package.md
[permission]: permission.md
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
[user]: /graph/api/resources/users
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
    "Resources/Item&quot;: &quot;#"
  },
  "suppressions": []
}
-->