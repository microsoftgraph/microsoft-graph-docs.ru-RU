---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveItem
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 58253683bfcc7407af398ba801885f9624bb2c28
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482422"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="41680-102">Тип ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="41680-102">DriveItem resource type</span></span>

<span data-ttu-id="41680-p101">Ресурс **driveItem** представляет файл, папку или другой элемент, хранящийся на диске. Все объекты файловой системы в OneDrive и SharePoint возвращаются в виде ресурсов **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="41680-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="41680-105">Обратиться к ресурсу **driveItem** можно двумя основными способами:</span><span class="sxs-lookup"><span data-stu-id="41680-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="41680-106">по уникальному идентификатору **driveItem** с помощью `drive/items/{item-id}`;</span><span class="sxs-lookup"><span data-stu-id="41680-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="41680-107">по пути файловой системы с помощью `/drive/root:/path/to/file`.</span><span class="sxs-lookup"><span data-stu-id="41680-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="41680-p102">У ресурсов **DriveItem** есть аспекты, смоделированные как свойства, которые предоставляют данные об идентификаторах и возможностях объекта driveItem. Пример:</span><span class="sxs-lookup"><span data-stu-id="41680-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="41680-110">У папок есть [**аспект folder**][folder].</span><span class="sxs-lookup"><span data-stu-id="41680-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="41680-111">У файлов есть [**аспект file**][file].</span><span class="sxs-lookup"><span data-stu-id="41680-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="41680-112">У изображений помимо аспекта file есть [**аспект image**][image].</span><span class="sxs-lookup"><span data-stu-id="41680-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="41680-113">У изображений, полученных с помощью камеры (фотографий), есть [**аспект photo**][photo], который определяет элемент как фотографию со свойствами времени съемки и устройства.</span><span class="sxs-lookup"><span data-stu-id="41680-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="41680-114">элементы с аспектом **folder** выполняют роль контейнеров элементов, поэтому у них есть ссылка `children`, указывающая на коллекцию объектов **driveItem** в папке.</span><span class="sxs-lookup"><span data-stu-id="41680-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41680-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="41680-115">JSON representation</span></span>

<span data-ttu-id="41680-116">Ниже представлено описание ресурса **driveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41680-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="41680-117">Ресурс **driveItem** является производным от ресурса [**baseItem**][baseItem] и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="41680-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
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

## <a name="properties"></a><span data-ttu-id="41680-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="41680-118">Properties</span></span>

| <span data-ttu-id="41680-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="41680-119">Property</span></span>             | <span data-ttu-id="41680-120">Тип</span><span class="sxs-lookup"><span data-stu-id="41680-120">Type</span></span>               | <span data-ttu-id="41680-121">Описание</span><span class="sxs-lookup"><span data-stu-id="41680-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="41680-122">audio</span><span class="sxs-lookup"><span data-stu-id="41680-122">audio</span></span>                | <span data-ttu-id="41680-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="41680-123">[audio][]</span></span>          | <span data-ttu-id="41680-p103">Метаданные звукового файла, если элемент — звуковой файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="41680-126">содержимое</span><span class="sxs-lookup"><span data-stu-id="41680-126">content</span></span>              | <span data-ttu-id="41680-127">Поток</span><span class="sxs-lookup"><span data-stu-id="41680-127">Stream</span></span>             | <span data-ttu-id="41680-128">Поток содержимого, если элемент представляет файл.</span><span class="sxs-lookup"><span data-stu-id="41680-128">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="41680-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="41680-129">createdBy</span></span>            | <span data-ttu-id="41680-130">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="41680-130">[identitySet][]</span></span>    | <span data-ttu-id="41680-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="41680-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41680-133">createdDateTime</span></span>      | <span data-ttu-id="41680-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41680-134">DateTimeOffset</span></span>     | <span data-ttu-id="41680-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="41680-137">cTag</span><span class="sxs-lookup"><span data-stu-id="41680-137">cTag</span></span>                 | <span data-ttu-id="41680-138">String</span><span class="sxs-lookup"><span data-stu-id="41680-138">String</span></span>             | <span data-ttu-id="41680-p106">ETag для содержимого элемента. Такой тег сущности не изменяется, если изменяются только метаданные. **Примечание.** Это свойство не возвращается, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="41680-143">deleted</span><span class="sxs-lookup"><span data-stu-id="41680-143">deleted</span></span>              | <span data-ttu-id="41680-144">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="41680-144">[deleted][]</span></span>        | <span data-ttu-id="41680-p107">Сведения о состоянии удаления элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="41680-147">description</span><span class="sxs-lookup"><span data-stu-id="41680-147">description</span></span>          | <span data-ttu-id="41680-148">String</span><span class="sxs-lookup"><span data-stu-id="41680-148">String</span></span>             | <span data-ttu-id="41680-p108">Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive</span><span class="sxs-lookup"><span data-stu-id="41680-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="41680-152">eTag</span><span class="sxs-lookup"><span data-stu-id="41680-152">eTag</span></span>                 | <span data-ttu-id="41680-153">String</span><span class="sxs-lookup"><span data-stu-id="41680-153">String</span></span>             | <span data-ttu-id="41680-p109">Тег сущности для всего элемента (метаданные и содержимое). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="41680-156">file</span><span class="sxs-lookup"><span data-stu-id="41680-156">file</span></span>                 | <span data-ttu-id="41680-157">[file][]</span><span class="sxs-lookup"><span data-stu-id="41680-157">[file][]</span></span>           | <span data-ttu-id="41680-p110">Файл метаданных, если в роли элемента выступает файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="41680-160">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="41680-160">fileSystemInfo</span></span>       | <span data-ttu-id="41680-161">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="41680-161">[fileSystemInfo][]</span></span> | <span data-ttu-id="41680-p111">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="41680-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="41680-164">folder</span><span class="sxs-lookup"><span data-stu-id="41680-164">folder</span></span>               | <span data-ttu-id="41680-165">[folder][]</span><span class="sxs-lookup"><span data-stu-id="41680-165">[folder][]</span></span>         | <span data-ttu-id="41680-p112">Метаданные папки, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="41680-168">id</span><span class="sxs-lookup"><span data-stu-id="41680-168">id</span></span>                   | <span data-ttu-id="41680-169">String</span><span class="sxs-lookup"><span data-stu-id="41680-169">String</span></span>             | <span data-ttu-id="41680-p113">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="41680-172">изображение</span><span class="sxs-lookup"><span data-stu-id="41680-172">image</span></span>                | <span data-ttu-id="41680-173">[image][]</span><span class="sxs-lookup"><span data-stu-id="41680-173">[image][]</span></span>          | <span data-ttu-id="41680-p114">Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="41680-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="41680-176">lastModifiedBy</span></span>       | <span data-ttu-id="41680-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="41680-177">[identitySet][]</span></span>    | <span data-ttu-id="41680-p115">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="41680-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41680-180">lastModifiedDateTime</span></span> | <span data-ttu-id="41680-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41680-181">DateTimeOffset</span></span>     | <span data-ttu-id="41680-p116">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="41680-184">location</span><span class="sxs-lookup"><span data-stu-id="41680-184">location</span></span>             | <span data-ttu-id="41680-185">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="41680-185">[geoCoordinates][]</span></span> | <span data-ttu-id="41680-p117">Метаданные местоположения, если в роли элемента выступают данные о местоположении. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="41680-188">name</span><span class="sxs-lookup"><span data-stu-id="41680-188">name</span></span>                 | <span data-ttu-id="41680-189">String</span><span class="sxs-lookup"><span data-stu-id="41680-189">String</span></span>             | <span data-ttu-id="41680-p118">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="41680-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="41680-192">package</span><span class="sxs-lookup"><span data-stu-id="41680-192">package</span></span>              | <span data-ttu-id="41680-193">[package][]</span><span class="sxs-lookup"><span data-stu-id="41680-193">[package][]</span></span>        | <span data-ttu-id="41680-p119">В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="41680-197">parentReference</span><span class="sxs-lookup"><span data-stu-id="41680-197">parentReference</span></span>      | <span data-ttu-id="41680-198">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="41680-198">[itemReference][]</span></span>  | <span data-ttu-id="41680-p120">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="41680-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="41680-201">Фотография
</span><span class="sxs-lookup"><span data-stu-id="41680-201">photo</span></span>                | <span data-ttu-id="41680-202">[photo][]</span><span class="sxs-lookup"><span data-stu-id="41680-202">[photo][]</span></span>          | <span data-ttu-id="41680-p121">Метаданные фотографии, если в роли элемента выступает фотография. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="41680-205">publication</span><span class="sxs-lookup"><span data-stu-id="41680-205">publication</span></span>          | <span data-ttu-id="41680-206">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="41680-206">[publicationFacet][]</span></span> | <span data-ttu-id="41680-207">Предоставляет сведения о состоянии элемента (опубликован или получен для изменения) в расположениях, поддерживающих такие действия.</span><span class="sxs-lookup"><span data-stu-id="41680-207">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="41680-208">Это свойство не возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="41680-208">This property is not returned by default.</span></span> <span data-ttu-id="41680-209">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-209">Read-only.</span></span> |
| <span data-ttu-id="41680-210">remoteItem</span><span class="sxs-lookup"><span data-stu-id="41680-210">remoteItem</span></span>           | <span data-ttu-id="41680-211">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="41680-211">[remoteItem][]</span></span>     | <span data-ttu-id="41680-p123">Данные удаленного элемента, если элемент используется совместно на диске, но не на том, к которому получен доступ в данный момент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="41680-214">root</span><span class="sxs-lookup"><span data-stu-id="41680-214">root</span></span>                 | <span data-ttu-id="41680-215">[root][]</span><span class="sxs-lookup"><span data-stu-id="41680-215">[root][]</span></span>           | <span data-ttu-id="41680-216">Ненулевое значение этого свойства указывает, что ресурс driveItem является самым верхним на диске.</span><span class="sxs-lookup"><span data-stu-id="41680-216">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="41680-217">searchResult</span><span class="sxs-lookup"><span data-stu-id="41680-217">searchResult</span></span>         | <span data-ttu-id="41680-218">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="41680-218">[searchResult][]</span></span>   | <span data-ttu-id="41680-p124">Поиск метаданных, если элемент получен из результата поиска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="41680-221">общие</span><span class="sxs-lookup"><span data-stu-id="41680-221">shared</span></span>               | <span data-ttu-id="41680-222">[shared][]</span><span class="sxs-lookup"><span data-stu-id="41680-222">[shared][]</span></span>         | <span data-ttu-id="41680-p125">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="41680-225">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="41680-225">sharepointIds</span></span>        | <span data-ttu-id="41680-226">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="41680-226">[sharepointIds][]</span></span>  | <span data-ttu-id="41680-p126">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="41680-229">size</span><span class="sxs-lookup"><span data-stu-id="41680-229">size</span></span>                 | <span data-ttu-id="41680-230">Int64</span><span class="sxs-lookup"><span data-stu-id="41680-230">Int64</span></span>              | <span data-ttu-id="41680-p127">Размер элемента (в байтах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="41680-233">specialFolder</span><span class="sxs-lookup"><span data-stu-id="41680-233">specialFolder</span></span>        | <span data-ttu-id="41680-234">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="41680-234">[specialFolder][]</span></span>  | <span data-ttu-id="41680-p128">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="41680-237">video</span><span class="sxs-lookup"><span data-stu-id="41680-237">video</span></span>                | <span data-ttu-id="41680-238">[video][]</span><span class="sxs-lookup"><span data-stu-id="41680-238">[video][]</span></span>          | <span data-ttu-id="41680-p129">Метаданные видео, если в роли элемента выступает видео. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="41680-241">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="41680-241">webDavUrl</span></span>            | <span data-ttu-id="41680-242">Строка</span><span class="sxs-lookup"><span data-stu-id="41680-242">String</span></span>             | <span data-ttu-id="41680-243">URL-адрес элемента, совместимый с WebDAV.</span><span class="sxs-lookup"><span data-stu-id="41680-243">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="41680-244">webUrl</span><span class="sxs-lookup"><span data-stu-id="41680-244">webUrl</span></span>               | <span data-ttu-id="41680-245">String</span><span class="sxs-lookup"><span data-stu-id="41680-245">String</span></span>             | <span data-ttu-id="41680-p130">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="41680-p131">**Примечание.** Свойства тегов eTag и cTag по-разному действуют на контейнеры (папки). Значение cTag изменяется при изменении содержимого или метаданных любого потомка папки. Значение eTag изменяется только при изменении свойств папки, за исключением свойств, которые являются производными от потомков (например, свойство **childCount** или **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="41680-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="41680-251">Отношения</span><span class="sxs-lookup"><span data-stu-id="41680-251">Relationships</span></span>

| <span data-ttu-id="41680-252">Отношение</span><span class="sxs-lookup"><span data-stu-id="41680-252">Relationship</span></span>       | <span data-ttu-id="41680-253">Тип</span><span class="sxs-lookup"><span data-stu-id="41680-253">Type</span></span>                        | <span data-ttu-id="41680-254">Описание</span><span class="sxs-lookup"><span data-stu-id="41680-254">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="41680-255">children</span><span class="sxs-lookup"><span data-stu-id="41680-255">children</span></span>           | <span data-ttu-id="41680-256">Коллекция driveItem</span><span class="sxs-lookup"><span data-stu-id="41680-256">driveitem collection</span></span>        | <span data-ttu-id="41680-p132">Коллекция, содержащая объекты Item для непосредственных дочерних элементов Item. Дочерние элементы есть только у элементов, представляющих папки. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="41680-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="41680-261">createdByUser</span><span class="sxs-lookup"><span data-stu-id="41680-261">createdByUser</span></span>      | <span data-ttu-id="41680-262">[user][]</span><span class="sxs-lookup"><span data-stu-id="41680-262">[user][]</span></span>                    | <span data-ttu-id="41680-263">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="41680-263">Identity of the user who created the item.</span></span> <span data-ttu-id="41680-264">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-264">Read-only.</span></span>
| <span data-ttu-id="41680-265">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="41680-265">lastModifiedByUser</span></span> | <span data-ttu-id="41680-266">[user][]</span><span class="sxs-lookup"><span data-stu-id="41680-266">[user][]</span></span>                    | <span data-ttu-id="41680-267">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="41680-267">Identity of the user who last modified the item.</span></span> <span data-ttu-id="41680-268">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-268">Read-only.</span></span>
| <span data-ttu-id="41680-269">listItem</span><span class="sxs-lookup"><span data-stu-id="41680-269">listItem</span></span>           | <span data-ttu-id="41680-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="41680-270">[listItem][]</span></span>                | <span data-ttu-id="41680-271">Для дисков в SharePoint, связанный элемент библиотеки документов.</span><span class="sxs-lookup"><span data-stu-id="41680-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="41680-272">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-272">Read-only.</span></span> <span data-ttu-id="41680-273">Может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="41680-273">Nullable.</span></span>
| <span data-ttu-id="41680-274">permissions</span><span class="sxs-lookup"><span data-stu-id="41680-274">permissions</span></span>        | <span data-ttu-id="41680-275">Коллекция объектов [permission][]</span><span class="sxs-lookup"><span data-stu-id="41680-275">[permission][] collection</span></span>   | <span data-ttu-id="41680-p136">Набор разрешений для элемента. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="41680-p136">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="41680-279">thumbnails</span><span class="sxs-lookup"><span data-stu-id="41680-279">thumbnails</span></span>         | <span data-ttu-id="41680-280">Коллекция объектов [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="41680-280">[thumbnailSet][] collection</span></span> | <span data-ttu-id="41680-p137">Коллекция, содержащая объекты [ThumbnailSet][], связанные с элементом. Дополнительные сведения см. в статье о [получении эскизов][]. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="41680-p137">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="41680-285">versions</span><span class="sxs-lookup"><span data-stu-id="41680-285">Versions</span></span>           | <span data-ttu-id="41680-286">Коллекция [driveItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="41680-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="41680-287">Список предыдущих версий элемента.</span><span class="sxs-lookup"><span data-stu-id="41680-287">The list of previous versions of the item.</span></span> <span data-ttu-id="41680-288">Дополнительные сведения см. в статье, посвященной [получению предыдущих версий][].</span><span class="sxs-lookup"><span data-stu-id="41680-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="41680-289">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-289">Read-only.</span></span> <span data-ttu-id="41680-290">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="41680-290">Nullable.</span></span>
| <span data-ttu-id="41680-291">workbook</span><span class="sxs-lookup"><span data-stu-id="41680-291">workbook</span></span>           | <span data-ttu-id="41680-292">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="41680-292">[workbook][]</span></span>                | <span data-ttu-id="41680-293">Для файлов, представляющих собой электронные таблицы Excel, получает доступ к API книги для работы с содержимым электронной таблицы.</span><span class="sxs-lookup"><span data-stu-id="41680-293">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="41680-294">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="41680-294">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="41680-295">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="41680-295">Instance Attributes</span></span>

<span data-ttu-id="41680-p140">Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.</span><span class="sxs-lookup"><span data-stu-id="41680-p140">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="41680-298">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="41680-298">Property name</span></span>                     | <span data-ttu-id="41680-299">Тип</span><span class="sxs-lookup"><span data-stu-id="41680-299">Type</span></span>   | <span data-ttu-id="41680-300">Описание</span><span class="sxs-lookup"><span data-stu-id="41680-300">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="41680-301">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="41680-301">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="41680-302">string</span><span class="sxs-lookup"><span data-stu-id="41680-302">string</span></span> | <span data-ttu-id="41680-p141">Определяет поведение для разрешения конфликтов, возникающих при создании элементов. Вы можете использовать значения *fail*, *replace* или *rename*. Значение по умолчанию для метода PUT: *replace*. Элементы никогда не возвращаются с такой заметкой. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="41680-p141">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="41680-308">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="41680-308">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="41680-309">string</span><span class="sxs-lookup"><span data-stu-id="41680-309">string</span></span> | <span data-ttu-id="41680-p142">URL-адрес, который можно использовать для скачивания содержимого этого файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41680-p142">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="41680-313">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="41680-313">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="41680-314">string</span><span class="sxs-lookup"><span data-stu-id="41680-314">string</span></span> | <span data-ttu-id="41680-p143">При создании запроса PUT такую заметку экземпляра можно использовать, чтобы указать службе скачать содержимое по URL-адресу и сохранить его как файл. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="41680-p143">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="41680-p144">**Примечание.** Значение @microsoft.graph.downloadUrl — это краткосрочный URL-адрес, который не сохраняется в кэше. URL-адрес будет доступен в течение короткого времени (1 час), после чего станет недействительным.</span><span class="sxs-lookup"><span data-stu-id="41680-p144">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="41680-319">Методы</span><span class="sxs-lookup"><span data-stu-id="41680-319">Methods</span></span>

| <span data-ttu-id="41680-320">Метод</span><span class="sxs-lookup"><span data-stu-id="41680-320">Method</span></span>                                                   | <span data-ttu-id="41680-321">Путь REST</span><span class="sxs-lookup"><span data-stu-id="41680-321">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="41680-322">Получение элемента</span><span class="sxs-lookup"><span data-stu-id="41680-322">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="41680-323">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="41680-323">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="41680-324">Список версий</span><span class="sxs-lookup"><span data-stu-id="41680-324">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="41680-325">Создание элемента</span><span class="sxs-lookup"><span data-stu-id="41680-325">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="41680-326">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="41680-326">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="41680-327">Отправка содержимого</span><span class="sxs-lookup"><span data-stu-id="41680-327">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="41680-328">Скачивание содержимого</span><span class="sxs-lookup"><span data-stu-id="41680-328">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="41680-329">[Скачивание файла в определенном формате][download-format]</span><span class="sxs-lookup"><span data-stu-id="41680-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="41680-330">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="41680-330">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="41680-331">Перемещение элемента</span><span class="sxs-lookup"><span data-stu-id="41680-331">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="41680-332">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="41680-332">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="41680-333">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="41680-333">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="41680-334">Перечисление изменений на диске</span><span class="sxs-lookup"><span data-stu-id="41680-334">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="41680-335">Перечисление эскизов</span><span class="sxs-lookup"><span data-stu-id="41680-335">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="41680-336">Создание ссылки совместного доступа</span><span class="sxs-lookup"><span data-stu-id="41680-336">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="41680-337">Добавление разрешений</span><span class="sxs-lookup"><span data-stu-id="41680-337">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="41680-338">Список разрешений</span><span class="sxs-lookup"><span data-stu-id="41680-338">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="41680-339">Удаление разрешения</span><span class="sxs-lookup"><span data-stu-id="41680-339">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="41680-340">[Предварительный просмотр элемента][item-preview]</span><span class="sxs-lookup"><span data-stu-id="41680-340">Preview item</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md

## <a name="remarks"></a><span data-ttu-id="41680-341">Заметки</span><span class="sxs-lookup"><span data-stu-id="41680-341">Remarks</span></span>

<span data-ttu-id="41680-342">В OneDrive для бизнеса и библиотеках документов SharePoint свойство **cTag** не возвращается, если у ресурса **driveItem** есть аспект [folder][].</span><span class="sxs-lookup"><span data-stu-id="41680-342">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

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
[identitySet]: identityset.md
[image]: image.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[workbook]: workbook.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
