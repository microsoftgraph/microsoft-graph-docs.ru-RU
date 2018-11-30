---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 526001ad9a6c52c5b031c1734466772861f1c67e
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="624da-102">Тип ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="624da-102">DriveItem resource type</span></span>

<span data-ttu-id="624da-p101">Ресурс **driveItem** представляет файл, папку или другой элемент, хранящийся на диске. Все объекты файловой системы в OneDrive и SharePoint возвращаются в виде ресурсов **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="624da-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="624da-105">Обратиться к ресурсу **driveItem** можно двумя основными способами:</span><span class="sxs-lookup"><span data-stu-id="624da-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="624da-106">по уникальному идентификатору **driveItem** с помощью `drive/items/{item-id}`;</span><span class="sxs-lookup"><span data-stu-id="624da-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="624da-107">по пути файловой системы с помощью `/drive/root:/path/to/file`.</span><span class="sxs-lookup"><span data-stu-id="624da-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="624da-p102">У ресурсов **DriveItem** есть аспекты, смоделированные как свойства, которые предоставляют данные об идентификаторах и возможностях объекта driveItem. Например:</span><span class="sxs-lookup"><span data-stu-id="624da-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="624da-110">У папок есть [**аспект folder**][folder].</span><span class="sxs-lookup"><span data-stu-id="624da-110">Folders have a [**folder facet**]</span></span>
* <span data-ttu-id="624da-111">У файлов есть [**аспект file**][file].</span><span class="sxs-lookup"><span data-stu-id="624da-111">Files have a [**file facet**].</span></span>
* <span data-ttu-id="624da-112">У изображений помимо аспекта file есть [**аспект image**][image].</span><span class="sxs-lookup"><span data-stu-id="624da-112">Images have an [**image facet**] in addition to their file facet.</span></span>
* <span data-ttu-id="624da-113">У изображений, полученных с помощью камеры (фотографий), есть [**аспект photo**][photo], который определяет элемент как фотографию со свойствами времени съемки и устройства.</span><span class="sxs-lookup"><span data-stu-id="624da-113">Images taken with a camera (photos) have a [**photo facet**] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="624da-114">элементы с аспектом **folder** выполняют роль контейнеров элементов, поэтому у них есть ссылка `children`, указывающая на коллекцию объектов **driveItem** в папке.</span><span class="sxs-lookup"><span data-stu-id="624da-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="624da-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="624da-115">JSON representation</span></span>

<span data-ttu-id="624da-116">Ниже представлено описание ресурса **driveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="624da-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="624da-117">Ресурс **driveItem** является производным от ресурса [**baseItem**][baseItem] и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="624da-117">The **driveItem** resource is derived from [**baseItem**] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
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
  "content": { "@odata.type": "Edm.Stream" },
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],

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

## <a name="properties"></a><span data-ttu-id="624da-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="624da-118">Properties</span></span>

| <span data-ttu-id="624da-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="624da-119">Property</span></span>             | <span data-ttu-id="624da-120">Тип</span><span class="sxs-lookup"><span data-stu-id="624da-120">Type</span></span>               | <span data-ttu-id="624da-121">Описание</span><span class="sxs-lookup"><span data-stu-id="624da-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="624da-122">audio</span><span class="sxs-lookup"><span data-stu-id="624da-122">audio</span></span>                | <span data-ttu-id="624da-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="624da-123">[audio][]</span></span>          | <span data-ttu-id="624da-p103">Метаданные звукового файла, если элемент — звуковой файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="624da-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="624da-126">createdBy</span></span>            | <span data-ttu-id="624da-127">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="624da-127">[identitySet][]</span></span>    | <span data-ttu-id="624da-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="624da-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="624da-130">createdDateTime</span></span>      | <span data-ttu-id="624da-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="624da-131">DateTimeOffset</span></span>     | <span data-ttu-id="624da-p105">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="624da-134">cTag</span><span class="sxs-lookup"><span data-stu-id="624da-134">cTag</span></span>                 | <span data-ttu-id="624da-135">String</span><span class="sxs-lookup"><span data-stu-id="624da-135">String</span></span>             | <span data-ttu-id="624da-p106">ETag для содержимого элемента. Такой тег сущности не изменяется, если изменяются только метаданные. **Примечание.** Это свойство не возвращается, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="624da-140">deleted</span><span class="sxs-lookup"><span data-stu-id="624da-140">deleted</span></span>              | <span data-ttu-id="624da-141">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="624da-141">[deleted][]</span></span>        | <span data-ttu-id="624da-p107">Сведения о состоянии удаления элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="624da-144">description</span><span class="sxs-lookup"><span data-stu-id="624da-144">description</span></span>          | <span data-ttu-id="624da-145">String</span><span class="sxs-lookup"><span data-stu-id="624da-145">String</span></span>             | <span data-ttu-id="624da-p108">Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive</span><span class="sxs-lookup"><span data-stu-id="624da-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="624da-149">eTag</span><span class="sxs-lookup"><span data-stu-id="624da-149">eTag</span></span>                 | <span data-ttu-id="624da-150">String</span><span class="sxs-lookup"><span data-stu-id="624da-150">String</span></span>             | <span data-ttu-id="624da-p109">Тег сущности для всего элемента (метаданные и содержимое). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="624da-153">file</span><span class="sxs-lookup"><span data-stu-id="624da-153">file</span></span>                 | <span data-ttu-id="624da-154">[file][]</span><span class="sxs-lookup"><span data-stu-id="624da-154">[file][]</span></span>           | <span data-ttu-id="624da-p110">Файл метаданных, если в роли элемента выступает файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="624da-157">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="624da-157">fileSystemInfo</span></span>       | <span data-ttu-id="624da-158">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="624da-158">[fileSystemInfo][]</span></span> | <span data-ttu-id="624da-p111">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="624da-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="624da-161">folder</span><span class="sxs-lookup"><span data-stu-id="624da-161">folder</span></span>               | <span data-ttu-id="624da-162">[folder][]</span><span class="sxs-lookup"><span data-stu-id="624da-162">[folder][]</span></span>         | <span data-ttu-id="624da-p112">Метаданные папки, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="624da-165">id</span><span class="sxs-lookup"><span data-stu-id="624da-165">id</span></span>                   | <span data-ttu-id="624da-166">String</span><span class="sxs-lookup"><span data-stu-id="624da-166">String</span></span>             | <span data-ttu-id="624da-p113">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="624da-169">изображение</span><span class="sxs-lookup"><span data-stu-id="624da-169">image</span></span>                | <span data-ttu-id="624da-170">[image][]</span><span class="sxs-lookup"><span data-stu-id="624da-170">[image][]</span></span>          | <span data-ttu-id="624da-p114">Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="624da-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="624da-173">lastModifiedBy</span></span>       | <span data-ttu-id="624da-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="624da-174">[identitySet][]</span></span>    | <span data-ttu-id="624da-p115">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="624da-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="624da-177">lastModifiedDateTime</span></span> | <span data-ttu-id="624da-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="624da-178">DateTimeOffset</span></span>     | <span data-ttu-id="624da-p116">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="624da-181">location</span><span class="sxs-lookup"><span data-stu-id="624da-181">location</span></span>             | <span data-ttu-id="624da-182">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="624da-182">[geoCoordinates][]</span></span> | <span data-ttu-id="624da-p117">Метаданные местоположения, если в роли элемента выступают данные о местоположении. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="624da-185">name</span><span class="sxs-lookup"><span data-stu-id="624da-185">name</span></span>                 | <span data-ttu-id="624da-186">String</span><span class="sxs-lookup"><span data-stu-id="624da-186">String</span></span>             | <span data-ttu-id="624da-p118">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="624da-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="624da-189">package</span><span class="sxs-lookup"><span data-stu-id="624da-189">package</span></span>              | <span data-ttu-id="624da-190">[package][]</span><span class="sxs-lookup"><span data-stu-id="624da-190">[package][]</span></span>        | <span data-ttu-id="624da-p119">В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="624da-194">parentReference</span><span class="sxs-lookup"><span data-stu-id="624da-194">parentReference</span></span>      | <span data-ttu-id="624da-195">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="624da-195">[itemReference][]</span></span>  | <span data-ttu-id="624da-p120">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="624da-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="624da-198">Фотография
</span><span class="sxs-lookup"><span data-stu-id="624da-198">photo</span></span>                | <span data-ttu-id="624da-199">[photo][]</span><span class="sxs-lookup"><span data-stu-id="624da-199">[photo][]</span></span>          | <span data-ttu-id="624da-p121">Метаданные фотографии, если в роли элемента выступает фотография. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="624da-202">remoteItem</span><span class="sxs-lookup"><span data-stu-id="624da-202">remoteItem</span></span>           | <span data-ttu-id="624da-203">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="624da-203">[remoteItem][]</span></span>     | <span data-ttu-id="624da-p122">Данные удаленного элемента, если элемент используется совместно на диске, но не на том, к которому получен доступ в данный момент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p122">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="624da-206">root</span><span class="sxs-lookup"><span data-stu-id="624da-206">root</span></span>                 | <span data-ttu-id="624da-207">[root][]</span><span class="sxs-lookup"><span data-stu-id="624da-207">[root][]</span></span>           | <span data-ttu-id="624da-208">Ненулевое значение этого свойства указывает, что ресурс driveItem является самым верхним на диске.</span><span class="sxs-lookup"><span data-stu-id="624da-208">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="624da-209">searchResult</span><span class="sxs-lookup"><span data-stu-id="624da-209">searchResult</span></span>         | <span data-ttu-id="624da-210">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="624da-210">[searchResult][]</span></span>   | <span data-ttu-id="624da-p123">Поиск метаданных, если элемент получен из результата поиска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p123">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="624da-213">общие</span><span class="sxs-lookup"><span data-stu-id="624da-213">shared</span></span>               | <span data-ttu-id="624da-214">[shared][]</span><span class="sxs-lookup"><span data-stu-id="624da-214">[shared][]</span></span>         | <span data-ttu-id="624da-p124">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p124">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="624da-217">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="624da-217">sharepointIds</span></span>        | <span data-ttu-id="624da-218">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="624da-218">[sharepointIds][]</span></span>  | <span data-ttu-id="624da-p125">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p125">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="624da-221">size</span><span class="sxs-lookup"><span data-stu-id="624da-221">size</span></span>                 | <span data-ttu-id="624da-222">Int64</span><span class="sxs-lookup"><span data-stu-id="624da-222">Int64</span></span>              | <span data-ttu-id="624da-p126">Размер элемента (в байтах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p126">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="624da-225">specialFolder</span><span class="sxs-lookup"><span data-stu-id="624da-225">specialFolder</span></span>        | <span data-ttu-id="624da-226">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="624da-226">[specialFolder][]</span></span>  | <span data-ttu-id="624da-p127">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p127">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="624da-229">video</span><span class="sxs-lookup"><span data-stu-id="624da-229">video</span></span>                | <span data-ttu-id="624da-230">[video][]</span><span class="sxs-lookup"><span data-stu-id="624da-230">[video][]</span></span>          | <span data-ttu-id="624da-p128">Метаданные видео, если в роли элемента выступает видео. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p128">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="624da-233">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="624da-233">webDavUrl</span></span>            | <span data-ttu-id="624da-234">Строка</span><span class="sxs-lookup"><span data-stu-id="624da-234">String</span></span>             | <span data-ttu-id="624da-235">URL-адрес элемента, совместимый с WebDAV.</span><span class="sxs-lookup"><span data-stu-id="624da-235">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="624da-236">webUrl</span><span class="sxs-lookup"><span data-stu-id="624da-236">webUrl</span></span>               | <span data-ttu-id="624da-237">String</span><span class="sxs-lookup"><span data-stu-id="624da-237">String</span></span>             | <span data-ttu-id="624da-p129">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p129">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="624da-p130">**Примечание.** Свойства тегов eTag и cTag по-разному действуют на контейнеры (папки). Значение cTag изменяется при изменении содержимого или метаданных любого потомка папки. Значение eTag изменяется только при изменении свойств папки, за исключением свойств, которые являются производными от потомков (например, свойство **childCount** или **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="624da-p130">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="624da-243">Отношения</span><span class="sxs-lookup"><span data-stu-id="624da-243">Relationships</span></span>

| <span data-ttu-id="624da-244">Связь</span><span class="sxs-lookup"><span data-stu-id="624da-244">Relationship</span></span>       | <span data-ttu-id="624da-245">Тип</span><span class="sxs-lookup"><span data-stu-id="624da-245">Type</span></span>                        | <span data-ttu-id="624da-246">Описание</span><span class="sxs-lookup"><span data-stu-id="624da-246">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="624da-247">content</span><span class="sxs-lookup"><span data-stu-id="624da-247">content</span></span>            | <span data-ttu-id="624da-248">Поток</span><span class="sxs-lookup"><span data-stu-id="624da-248">Stream</span></span>                      | <span data-ttu-id="624da-249">Поток содержимого, если элемент представляет файл.</span><span class="sxs-lookup"><span data-stu-id="624da-249">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="624da-250">children</span><span class="sxs-lookup"><span data-stu-id="624da-250">children</span></span>           | <span data-ttu-id="624da-251">Коллекция объектов driveItem</span><span class="sxs-lookup"><span data-stu-id="624da-251">driveitem collection</span></span>        | <span data-ttu-id="624da-p131">Коллекция, содержащая объекты Item для непосредственных дочерних элементов Item. Дочерние элементы есть только у элементов, представляющих папки. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="624da-p131">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="624da-256">createdByUser</span><span class="sxs-lookup"><span data-stu-id="624da-256">createdByUser</span></span>      | <span data-ttu-id="624da-257">[user][]</span><span class="sxs-lookup"><span data-stu-id="624da-257">[user][]</span></span>                    | <span data-ttu-id="624da-258">Удостоверение пользователя, создавшего элемент.</span><span class="sxs-lookup"><span data-stu-id="624da-258">Identity of the user who created the item.</span></span> <span data-ttu-id="624da-259">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-259">Read-only.</span></span>
| <span data-ttu-id="624da-260">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="624da-260">lastModifiedByUser</span></span> | <span data-ttu-id="624da-261">[user][]</span><span class="sxs-lookup"><span data-stu-id="624da-261">[user][]</span></span>                    | <span data-ttu-id="624da-262">Удостоверение пользователя, который последним изменил элемент.</span><span class="sxs-lookup"><span data-stu-id="624da-262">Identity of the user, device, and application which last modified the item. Read-only.</span></span> <span data-ttu-id="624da-263">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-263">Read-only.</span></span>
| <span data-ttu-id="624da-264">permissions</span><span class="sxs-lookup"><span data-stu-id="624da-264">permissions</span></span>        | <span data-ttu-id="624da-265">Коллекция объектов [permission][]</span><span class="sxs-lookup"><span data-stu-id="624da-265">[permission][] collection</span></span>   | <span data-ttu-id="624da-p134">Набор разрешений для элемента. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="624da-p134">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="624da-269">thumbnails</span><span class="sxs-lookup"><span data-stu-id="624da-269">thumbnails</span></span>         | <span data-ttu-id="624da-270">Коллекция объектов [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="624da-270">[thumbnailSet][] collection</span></span> | <span data-ttu-id="624da-p135">Коллекция, содержащая объекты [ThumbnailSet][], связанные с элементом. Дополнительные сведения см. в статье о [получении эскизов][]. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="624da-p135">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="624da-275">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="624da-275">Instance Attributes</span></span>

<span data-ttu-id="624da-p136">Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.</span><span class="sxs-lookup"><span data-stu-id="624da-p136">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="624da-278">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="624da-278">Property name</span></span>                     | <span data-ttu-id="624da-279">Тип</span><span class="sxs-lookup"><span data-stu-id="624da-279">Type</span></span>   | <span data-ttu-id="624da-280">Описание</span><span class="sxs-lookup"><span data-stu-id="624da-280">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="624da-281">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="624da-281">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="624da-282">string</span><span class="sxs-lookup"><span data-stu-id="624da-282">string</span></span> | <span data-ttu-id="624da-p137">Определяет поведение для разрешения конфликтов, возникающих при создании элементов. Вы можете использовать значения *fail*, *replace* или *rename*. Значение по умолчанию для метода PUT: *replace*. Элементы никогда не возвращаются с такой заметкой. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="624da-p137">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="624da-288">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="624da-288">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="624da-289">string</span><span class="sxs-lookup"><span data-stu-id="624da-289">string</span></span> | <span data-ttu-id="624da-p138">URL-адрес, который можно использовать для скачивания содержимого этого файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="624da-p138">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="624da-293">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="624da-293">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="624da-294">string</span><span class="sxs-lookup"><span data-stu-id="624da-294">string</span></span> | <span data-ttu-id="624da-p139">При создании запроса PUT такую заметку экземпляра можно использовать, чтобы указать службе скачать содержимое по URL-адресу и сохранить его как файл. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="624da-p139">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="624da-p140">**Примечание.** Значение @microsoft.graph.downloadUrl — это краткосрочный URL-адрес, который не сохраняется в кэше. URL-адрес будет доступен в течение короткого времени (1 час), после чего станет недействительным.</span><span class="sxs-lookup"><span data-stu-id="624da-p140">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="624da-299">Методы</span><span class="sxs-lookup"><span data-stu-id="624da-299">Methods</span></span>

| <span data-ttu-id="624da-300">Метод</span><span class="sxs-lookup"><span data-stu-id="624da-300">Method</span></span>                                                   | <span data-ttu-id="624da-301">Путь REST</span><span class="sxs-lookup"><span data-stu-id="624da-301">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="624da-302">Получение элемента</span><span class="sxs-lookup"><span data-stu-id="624da-302">Get item</span></span>](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="624da-303">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="624da-303">List children</span></span>](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="624da-304">Создание элемента</span><span class="sxs-lookup"><span data-stu-id="624da-304">Create item</span></span>](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="624da-305">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="624da-305">Update item</span></span>](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="624da-306">Отправка содержимого</span><span class="sxs-lookup"><span data-stu-id="624da-306">Upload content</span></span>](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="624da-307">Скачивание содержимого</span><span class="sxs-lookup"><span data-stu-id="624da-307">Download content</span></span>](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="624da-308">[Скачивание файла в определенном формате][download-format]</span><span class="sxs-lookup"><span data-stu-id="624da-308">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="624da-309">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="624da-309">Delete item</span></span>](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="624da-310">Перемещение элемента</span><span class="sxs-lookup"><span data-stu-id="624da-310">Move item</span></span>](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="624da-311">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="624da-311">Copy item</span></span>](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="624da-312">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="624da-312">Search items</span></span>](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="624da-313">Перечисление изменений на диске</span><span class="sxs-lookup"><span data-stu-id="624da-313">List changes in a drive</span></span>](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="624da-314">Перечисление эскизов</span><span class="sxs-lookup"><span data-stu-id="624da-314">List thumbnails</span></span>](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="624da-315">Создание ссылки совместного доступа</span><span class="sxs-lookup"><span data-stu-id="624da-315">Create sharing link</span></span>](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="624da-316">Добавление разрешений</span><span class="sxs-lookup"><span data-stu-id="624da-316">Add permissions</span></span>](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="624da-317">Список разрешений</span><span class="sxs-lookup"><span data-stu-id="624da-317">List permissions</span></span>](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="624da-318">Удаление разрешения</span><span class="sxs-lookup"><span data-stu-id="624da-318">Delete permission</span></span>](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a><span data-ttu-id="624da-319">Заметки</span><span class="sxs-lookup"><span data-stu-id="624da-319">Remarks</span></span>

<span data-ttu-id="624da-320">В OneDrive для бизнеса и библиотеках документов SharePoint свойство **cTag** не возвращается, если у ресурса **driveItem** есть аспект [folder][].</span><span class="sxs-lookup"><span data-stu-id="624da-320">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseItem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[file]: file.md
[fileSystemInfo]: fileSystemInfo.md
[folder]: folder.md
[getting thumbnails]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
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
[user]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
