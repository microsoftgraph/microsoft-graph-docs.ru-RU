---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 60f2d58331f349f9990f78f36f04df055ce90b9e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23269840"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="5f40f-102">Тип ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="5f40f-102">DriveItem resource type</span></span>

<span data-ttu-id="5f40f-p101">Ресурс **driveItem** представляет файл, папку или другой элемент, хранящийся на диске. Все объекты файловой системы в OneDrive и SharePoint возвращаются в виде ресурсов **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="5f40f-105">Обратиться к ресурсу **driveItem** можно двумя основными способами:</span><span class="sxs-lookup"><span data-stu-id="5f40f-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="5f40f-106">по уникальному идентификатору **driveItem** с помощью `drive/items/{item-id}`; `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="5f40f-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="5f40f-107">по пути файловой системы с помощью `/drive/root:/path/to/file`. `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="5f40f-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="5f40f-p102">У ресурсов **DriveItem** есть аспекты, смоделированные как свойства, которые предоставляют данные об идентификаторах и возможностях объекта driveItem. Пример:</span><span class="sxs-lookup"><span data-stu-id="5f40f-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="5f40f-110">у папок есть [**аспект folder**][folder];</span><span class="sxs-lookup"><span data-stu-id="5f40f-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="5f40f-111">у файлов есть [**аспект file**][file];</span><span class="sxs-lookup"><span data-stu-id="5f40f-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="5f40f-112">у изображений, помимо аспекта file, есть [**аспект image**][image];</span><span class="sxs-lookup"><span data-stu-id="5f40f-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="5f40f-113">у изображений, полученных с помощью камеры (фотографий), есть [**аспект photo**][photo], который определяет элемент как фотографию со свойствами времени съемки и устройства;</span><span class="sxs-lookup"><span data-stu-id="5f40f-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="5f40f-114">элементы с аспектом **folder** выполняют роль контейнеров элементов, поэтому у них есть ссылка `children`, указывающая на коллекцию объектов **driveItem** в папке.</span><span class="sxs-lookup"><span data-stu-id="5f40f-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f40f-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5f40f-115">JSON representation</span></span>

<span data-ttu-id="5f40f-116">Ниже представлено описание ресурса **driveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f40f-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="5f40f-117">Ресурс **driveItem** является производным от ресурса [**baseItem**][baseItem] и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="5f40f-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5f40f-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f40f-118">Properties</span></span>

| <span data-ttu-id="5f40f-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f40f-119">Property</span></span>             | <span data-ttu-id="5f40f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5f40f-120">Type</span></span>               | <span data-ttu-id="5f40f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5f40f-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="5f40f-122">audio</span><span class="sxs-lookup"><span data-stu-id="5f40f-122">audio</span></span>                | <span data-ttu-id="5f40f-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-123">[audio][]</span></span>          | <span data-ttu-id="5f40f-p103">Метаданные звукового файла, если элемент — звуковой файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="5f40f-126">content</span><span class="sxs-lookup"><span data-stu-id="5f40f-126">content</span></span>              | <span data-ttu-id="5f40f-127">Поток</span><span class="sxs-lookup"><span data-stu-id="5f40f-127">Stream</span></span>             | <span data-ttu-id="5f40f-128">Поток содержимого, если элемент представляет файл.</span><span class="sxs-lookup"><span data-stu-id="5f40f-128">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="5f40f-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="5f40f-129">createdBy</span></span>            | <span data-ttu-id="5f40f-130">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-130">[identitySet][]</span></span>    | <span data-ttu-id="5f40f-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="5f40f-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f40f-133">createdDateTime</span></span>      | <span data-ttu-id="5f40f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f40f-134">DateTimeOffset</span></span>     | <span data-ttu-id="5f40f-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="5f40f-137">cTag</span><span class="sxs-lookup"><span data-stu-id="5f40f-137">cTag</span></span>                 | <span data-ttu-id="5f40f-138">String</span><span class="sxs-lookup"><span data-stu-id="5f40f-138">String</span></span>             | <span data-ttu-id="5f40f-p106">ETag для содержимого элемента. Такой тег сущности не изменяется, если изменяются только метаданные. **Примечание.** Это свойство не возвращается, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="5f40f-143">deleted</span><span class="sxs-lookup"><span data-stu-id="5f40f-143">deleted</span></span>              | <span data-ttu-id="5f40f-144">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-144">[deleted][]</span></span>        | <span data-ttu-id="5f40f-p107">Сведения о состоянии удаления элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="5f40f-147">description</span><span class="sxs-lookup"><span data-stu-id="5f40f-147">description</span></span>          | <span data-ttu-id="5f40f-148">String</span><span class="sxs-lookup"><span data-stu-id="5f40f-148">String</span></span>             | <span data-ttu-id="5f40f-p108">Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive</span><span class="sxs-lookup"><span data-stu-id="5f40f-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="5f40f-152">eTag</span><span class="sxs-lookup"><span data-stu-id="5f40f-152">eTag</span></span>                 | <span data-ttu-id="5f40f-153">String</span><span class="sxs-lookup"><span data-stu-id="5f40f-153">String</span></span>             | <span data-ttu-id="5f40f-p109">Тег сущности для всего элемента (метаданные и содержимое). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="5f40f-156">file</span><span class="sxs-lookup"><span data-stu-id="5f40f-156">file</span></span>                 | <span data-ttu-id="5f40f-157">[file][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-157">[file][]</span></span>           | <span data-ttu-id="5f40f-p110">Файл метаданных, если в роли элемента выступает файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="5f40f-160">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="5f40f-160">fileSystemInfo</span></span>       | <span data-ttu-id="5f40f-161">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-161">[fileSystemInfo][]</span></span> | <span data-ttu-id="5f40f-p111">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="5f40f-164">folder</span><span class="sxs-lookup"><span data-stu-id="5f40f-164">folder</span></span>               | <span data-ttu-id="5f40f-165">[folder][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-165">[folder][]</span></span>         | <span data-ttu-id="5f40f-p112">Метаданные папки, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="5f40f-168">id</span><span class="sxs-lookup"><span data-stu-id="5f40f-168">id</span></span>                   | <span data-ttu-id="5f40f-169">String</span><span class="sxs-lookup"><span data-stu-id="5f40f-169">String</span></span>             | <span data-ttu-id="5f40f-p113">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="5f40f-172">image</span><span class="sxs-lookup"><span data-stu-id="5f40f-172">image</span></span>                | <span data-ttu-id="5f40f-173">[image][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-173">[image][]</span></span>          | <span data-ttu-id="5f40f-p114">Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="5f40f-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5f40f-176">lastModifiedBy</span></span>       | <span data-ttu-id="5f40f-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-177">[identitySet][]</span></span>    | <span data-ttu-id="5f40f-p115">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="5f40f-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f40f-180">lastModifiedDateTime</span></span> | <span data-ttu-id="5f40f-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f40f-181">DateTimeOffset</span></span>     | <span data-ttu-id="5f40f-p116">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="5f40f-184">location</span><span class="sxs-lookup"><span data-stu-id="5f40f-184">location</span></span>             | <span data-ttu-id="5f40f-185">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-185">[geoCoordinates][]</span></span> | <span data-ttu-id="5f40f-p117">Метаданные местоположения, если в роли элемента выступают данные о местоположении. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="5f40f-188">name</span><span class="sxs-lookup"><span data-stu-id="5f40f-188">name</span></span>                 | <span data-ttu-id="5f40f-189">String</span><span class="sxs-lookup"><span data-stu-id="5f40f-189">String</span></span>             | <span data-ttu-id="5f40f-p118">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="5f40f-192">package</span><span class="sxs-lookup"><span data-stu-id="5f40f-192">package</span></span>              | <span data-ttu-id="5f40f-193">[package][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-193">[package][]</span></span>        | <span data-ttu-id="5f40f-p119">При наличии этого свойства оно указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="5f40f-197">parentReference</span><span class="sxs-lookup"><span data-stu-id="5f40f-197">parentReference</span></span>      | <span data-ttu-id="5f40f-198">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-198">[itemReference][]</span></span>  | <span data-ttu-id="5f40f-p120">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="5f40f-201">photo</span><span class="sxs-lookup"><span data-stu-id="5f40f-201">photo</span></span>                | <span data-ttu-id="5f40f-202">[photo][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-202">[photo][]</span></span>          | <span data-ttu-id="5f40f-p121">Метаданные фотографии, если в роли элемента выступает фотография. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="5f40f-205">publication</span><span class="sxs-lookup"><span data-stu-id="5f40f-205">publication</span></span>          | <span data-ttu-id="5f40f-206">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-206">[publicationFacet][]</span></span> | <span data-ttu-id="5f40f-207">Предоставляет сведения о состоянии элемента (опубликован или получен для изменения) в расположениях, поддерживающих такие действия.</span><span class="sxs-lookup"><span data-stu-id="5f40f-207">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="5f40f-208">Это свойство не возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f40f-208">This property is not returned by default.</span></span> <span data-ttu-id="5f40f-209">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-209">Read-only.</span></span> |
| <span data-ttu-id="5f40f-210">remoteItem</span><span class="sxs-lookup"><span data-stu-id="5f40f-210">remoteItem</span></span>           | <span data-ttu-id="5f40f-211">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-211">[remoteItem][]</span></span>     | <span data-ttu-id="5f40f-p123">Данные удаленного элемента, если элемент используется совместно на диске, но не на том, к которому получен доступ в данный момент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="5f40f-214">root</span><span class="sxs-lookup"><span data-stu-id="5f40f-214">root</span></span>                 | <span data-ttu-id="5f40f-215">[root][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-215">[root][]</span></span>           | <span data-ttu-id="5f40f-216">Ненулевое значение этого свойства указывает, что ресурс driveItem является самым верхним на диске.</span><span class="sxs-lookup"><span data-stu-id="5f40f-216">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="5f40f-217">searchResult</span><span class="sxs-lookup"><span data-stu-id="5f40f-217">searchResult</span></span>         | <span data-ttu-id="5f40f-218">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-218">[searchResult][]</span></span>   | <span data-ttu-id="5f40f-p124">Поиск метаданных, если элемент получен из результата поиска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="5f40f-221">shared</span><span class="sxs-lookup"><span data-stu-id="5f40f-221">shared</span></span>               | <span data-ttu-id="5f40f-222">[shared][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-222">[shared][]</span></span>         | <span data-ttu-id="5f40f-p125">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="5f40f-225">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="5f40f-225">sharepointIds</span></span>        | <span data-ttu-id="5f40f-226">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-226">[sharepointIds][]</span></span>  | <span data-ttu-id="5f40f-p126">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="5f40f-229">size</span><span class="sxs-lookup"><span data-stu-id="5f40f-229">size</span></span>                 | <span data-ttu-id="5f40f-230">Int64</span><span class="sxs-lookup"><span data-stu-id="5f40f-230">Int64</span></span>              | <span data-ttu-id="5f40f-p127">Размер элемента (в байтах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="5f40f-233">specialFolder</span><span class="sxs-lookup"><span data-stu-id="5f40f-233">specialFolder</span></span>        | <span data-ttu-id="5f40f-234">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-234">[specialFolder][]</span></span>  | <span data-ttu-id="5f40f-p128">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="5f40f-237">video</span><span class="sxs-lookup"><span data-stu-id="5f40f-237">video</span></span>                | <span data-ttu-id="5f40f-238">[video][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-238">[video][]</span></span>          | <span data-ttu-id="5f40f-p129">Метаданные видео, если в роли элемента выступает видео. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="5f40f-241">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="5f40f-241">webDavUrl</span></span>            | <span data-ttu-id="5f40f-242">String</span><span class="sxs-lookup"><span data-stu-id="5f40f-242">String</span></span>             | <span data-ttu-id="5f40f-243">URL-адрес элемента, совместимый с WebDAV.</span><span class="sxs-lookup"><span data-stu-id="5f40f-243">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="5f40f-244">webUrl</span><span class="sxs-lookup"><span data-stu-id="5f40f-244">webUrl</span></span>               | <span data-ttu-id="5f40f-245">String</span><span class="sxs-lookup"><span data-stu-id="5f40f-245">String</span></span>             | <span data-ttu-id="5f40f-p130">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="5f40f-p131">**Примечание.** Свойства тегов eTag и cTag по-разному действуют на контейнеры (папки). Значение cTag изменяется при изменении содержимого или метаданных любого потомка папки. Значение eTag изменяется только при изменении свойств папки, за исключением свойств, которые являются производными от потомков (например, свойство **childCount** или **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="5f40f-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="5f40f-251">Отношения</span><span class="sxs-lookup"><span data-stu-id="5f40f-251">Relationships</span></span>

| <span data-ttu-id="5f40f-252">Связь</span><span class="sxs-lookup"><span data-stu-id="5f40f-252">Relationship</span></span>       | <span data-ttu-id="5f40f-253">Тип</span><span class="sxs-lookup"><span data-stu-id="5f40f-253">Type</span></span>                        | <span data-ttu-id="5f40f-254">Описание</span><span class="sxs-lookup"><span data-stu-id="5f40f-254">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="5f40f-255">Дочерние элементы (children)</span><span class="sxs-lookup"><span data-stu-id="5f40f-255">children</span></span>           | <span data-ttu-id="5f40f-256">Коллекция объектов driveItem</span><span class="sxs-lookup"><span data-stu-id="5f40f-256">driveitem collection</span></span>        | <span data-ttu-id="5f40f-p132">Коллекция, содержащая объекты Item для непосредственных дочерних элементов данного ресурса Item. Дочерние элементы есть только у элементов, представляющих папки. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="5f40f-261">createdByUser</span><span class="sxs-lookup"><span data-stu-id="5f40f-261">createdByUser</span></span>      | <span data-ttu-id="5f40f-262">[user][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-262">[user][]</span></span>                    | <span data-ttu-id="5f40f-263">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="5f40f-263">Identity of the user who created the item.</span></span> <span data-ttu-id="5f40f-264">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-264">Read-only.</span></span>
| <span data-ttu-id="5f40f-265">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="5f40f-265">lastModifiedByUser</span></span> | <span data-ttu-id="5f40f-266">[user][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-266">[user][]</span></span>                    | <span data-ttu-id="5f40f-267">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="5f40f-267">Identity of the user who last modified the item.</span></span> <span data-ttu-id="5f40f-268">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-268">Read-only.</span></span>
| <span data-ttu-id="5f40f-269">listItem</span><span class="sxs-lookup"><span data-stu-id="5f40f-269">listItem</span></span>           | <span data-ttu-id="5f40f-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-270">[listItem][]</span></span>                | <span data-ttu-id="5f40f-271">Для дисков в SharePoint – сопоставленный элемент списка библиотеки документов.</span><span class="sxs-lookup"><span data-stu-id="5f40f-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="5f40f-272">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-272">Read-only.</span></span> <span data-ttu-id="5f40f-273">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5f40f-273">Nullable.</span></span>
| <span data-ttu-id="5f40f-274">permissions</span><span class="sxs-lookup"><span data-stu-id="5f40f-274">permissions</span></span>        | <span data-ttu-id="5f40f-275">Коллекция объектов [permission][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-275">[permission][] collection</span></span>   | <span data-ttu-id="5f40f-p136">Набор разрешений для элемента. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p136">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="5f40f-279">thumbnails</span><span class="sxs-lookup"><span data-stu-id="5f40f-279">thumbnails</span></span>         | <span data-ttu-id="5f40f-280">Коллекция объектов [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-280">[thumbnailSet][] collection</span></span> | <span data-ttu-id="5f40f-p137">Коллекция, содержащая объекты [ThumbnailSet][], связанные с элементом. Дополнительные сведения см. в статье о [получении эскизов][]. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p137">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="5f40f-285">versions</span><span class="sxs-lookup"><span data-stu-id="5f40f-285">versions</span></span>           | <span data-ttu-id="5f40f-286">Коллекция [driveItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="5f40f-287">Список предыдущих версий элемента.</span><span class="sxs-lookup"><span data-stu-id="5f40f-287">The list of previous versions of the item.</span></span> <span data-ttu-id="5f40f-288">Дополнительные сведения см. в статье о [получении предыдущих версий][].</span><span class="sxs-lookup"><span data-stu-id="5f40f-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="5f40f-289">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-289">Read-only.</span></span> <span data-ttu-id="5f40f-290">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5f40f-290">Nullable.</span></span>
| <span data-ttu-id="5f40f-291">workbook</span><span class="sxs-lookup"><span data-stu-id="5f40f-291">workbook</span></span>           | <span data-ttu-id="5f40f-292">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="5f40f-292">[workbook][]</span></span>                | <span data-ttu-id="5f40f-293">Предоставляет файлам, которые являются электронными таблицами Excel, доступ к API книги для работы с содержимым электронной таблицы</span><span class="sxs-lookup"><span data-stu-id="5f40f-293">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="5f40f-294">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5f40f-294">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="5f40f-295">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="5f40f-295">Instance Attributes</span></span>

<span data-ttu-id="5f40f-p140">Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p140">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="5f40f-298">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5f40f-298">Property name</span></span>                     | <span data-ttu-id="5f40f-299">Тип</span><span class="sxs-lookup"><span data-stu-id="5f40f-299">Type</span></span>   | <span data-ttu-id="5f40f-300">Описание</span><span class="sxs-lookup"><span data-stu-id="5f40f-300">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="5f40f-301">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="5f40f-301">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="5f40f-302">string</span><span class="sxs-lookup"><span data-stu-id="5f40f-302">string</span></span> | <span data-ttu-id="5f40f-p141">Определяет поведение для разрешения конфликтов, возникающих при создании элементов. Вы можете использовать значения *fail*, *replace* или *rename*. Значение по умолчанию для метода PUT: *replace*. Элементы никогда не возвращаются с такой заметкой. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p141">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="5f40f-308">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="5f40f-308">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="5f40f-309">string</span><span class="sxs-lookup"><span data-stu-id="5f40f-309">string</span></span> | <span data-ttu-id="5f40f-p142">URL-адрес, который можно использовать для скачивания содержимого этого файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p142">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="5f40f-313">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="5f40f-313">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="5f40f-314">string</span><span class="sxs-lookup"><span data-stu-id="5f40f-314">string</span></span> | <span data-ttu-id="5f40f-p143">При создании запроса PUT такую заметку экземпляра можно использовать, чтобы указать службе скачать содержимое по URL-адресу и сохранить его как файл. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p143">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="5f40f-p144">**Примечание.** Значение @microsoft.graph.downloadUrl — это краткосрочный URL-адрес, который не сохраняется в кэше. URL-адрес будет доступен в течение короткого времени (1 час), после чего станет недействительным.</span><span class="sxs-lookup"><span data-stu-id="5f40f-p144">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="5f40f-319">Методы</span><span class="sxs-lookup"><span data-stu-id="5f40f-319">Methods</span></span>

| <span data-ttu-id="5f40f-320">Метод</span><span class="sxs-lookup"><span data-stu-id="5f40f-320">Method</span></span>                                                   | <span data-ttu-id="5f40f-321">Путь REST</span><span class="sxs-lookup"><span data-stu-id="5f40f-321">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="5f40f-322">Получение элемента</span><span class="sxs-lookup"><span data-stu-id="5f40f-322">Get item</span></span>](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="5f40f-323">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="5f40f-323">List children</span></span>](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="5f40f-324">Список версий</span><span class="sxs-lookup"><span data-stu-id="5f40f-324">List versions</span></span>](../api/driveitem_list_versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="5f40f-325">Создание элемента</span><span class="sxs-lookup"><span data-stu-id="5f40f-325">Create item</span></span>](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="5f40f-326">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="5f40f-326">Update item</span></span>](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="5f40f-327">Отправка содержимого</span><span class="sxs-lookup"><span data-stu-id="5f40f-327">Upload content</span></span>](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="5f40f-328">Скачивание содержимого</span><span class="sxs-lookup"><span data-stu-id="5f40f-328">Download content</span></span>](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="5f40f-329">[Скачивание файла в определенном формате][download-format]</span><span class="sxs-lookup"><span data-stu-id="5f40f-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="5f40f-330">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="5f40f-330">Delete item</span></span>](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="5f40f-331">Перемещение элемента</span><span class="sxs-lookup"><span data-stu-id="5f40f-331">Move item</span></span>](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="5f40f-332">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="5f40f-332">Copy item</span></span>](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="5f40f-333">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="5f40f-333">Search items</span></span>](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="5f40f-334">Перечисление изменений на диске</span><span class="sxs-lookup"><span data-stu-id="5f40f-334">List changes in a drive</span></span>](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="5f40f-335">Перечисление эскизов</span><span class="sxs-lookup"><span data-stu-id="5f40f-335">List thumbnails</span></span>](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="5f40f-336">Создание ссылки совместного доступа</span><span class="sxs-lookup"><span data-stu-id="5f40f-336">Create sharing link</span></span>](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="5f40f-337">Добавление разрешений</span><span class="sxs-lookup"><span data-stu-id="5f40f-337">Add permissions</span></span>](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="5f40f-338">Список разрешений</span><span class="sxs-lookup"><span data-stu-id="5f40f-338">List permissions</span></span>](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="5f40f-339">Удаление разрешения</span><span class="sxs-lookup"><span data-stu-id="5f40f-339">Delete permission</span></span>](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a><span data-ttu-id="5f40f-340">Заметки</span><span class="sxs-lookup"><span data-stu-id="5f40f-340">Remarks</span></span>

<span data-ttu-id="5f40f-341">В OneDrive для бизнеса и библиотеках документов SharePoint свойство **cTag** не возвращается, если у ресурса **driveItem** есть аспект [folder][].</span><span class="sxs-lookup"><span data-stu-id="5f40f-341">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseItem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[driveItemVersion]: driveItemVersion.md
[file]: file.md
[fileSystemInfo]: fileSystemInfo.md
[folder]: folder.md
[getting previous versions]: ../api/driveitem_list_versions.md
[getting thumbnails]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
[listItem]: listItem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteItem.md
[root]: root.md
[searchResult]: searchResult.md
[shared]: shared.md
[sharepointIds]: sharepointIds.md
[specialFolder]: specialFolder.md
[thumbnailSet]: thumbnailSet.md
[video]: video.md
[workbook]: workbook.md
[user]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
