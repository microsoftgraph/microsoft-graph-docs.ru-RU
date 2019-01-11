---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.openlocfilehash: 255b9de7ad565228da093a9a40d23c3360df28b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882266"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="c319e-102">Тип ресурса driveItem</span><span class="sxs-lookup"><span data-stu-id="c319e-102">driveItem resource type</span></span>

> <span data-ttu-id="c319e-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c319e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c319e-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c319e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c319e-p102">Ресурс **driveItem** представляет файл, папку или другой элемент, хранящийся на диске. Все объекты файловой системы в OneDrive и SharePoint возвращаются в виде ресурсов **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="c319e-p102">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="c319e-107">Обратиться к ресурсу **driveItem** можно двумя основными способами:</span><span class="sxs-lookup"><span data-stu-id="c319e-107">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="c319e-108">по уникальному идентификатору **driveItem** с помощью `drive/items/{item-id}`;</span><span class="sxs-lookup"><span data-stu-id="c319e-108">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="c319e-109">по пути файловой системы с помощью `/drive/root:/path/to/file`.</span><span class="sxs-lookup"><span data-stu-id="c319e-109">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="c319e-p103">У ресурсов **DriveItem** есть аспекты, смоделированные как свойства, которые предоставляют данные об идентификаторах и возможностях объекта driveItem. Пример:</span><span class="sxs-lookup"><span data-stu-id="c319e-p103">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="c319e-112">у папок есть [**аспект folder**][folder];</span><span class="sxs-lookup"><span data-stu-id="c319e-112">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="c319e-113">у файлов есть [**аспект file**][file];</span><span class="sxs-lookup"><span data-stu-id="c319e-113">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="c319e-114">у изображений, помимо аспекта file, есть [**аспект image**][image];</span><span class="sxs-lookup"><span data-stu-id="c319e-114">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="c319e-115">у изображений, полученных с помощью камеры (фотографий), есть [**аспект photo**][photo], который определяет элемент как фотографию со свойствами времени съемки и устройства;</span><span class="sxs-lookup"><span data-stu-id="c319e-115">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="c319e-116">элементы с аспектом **folder** выполняют роль контейнеров элементов, поэтому у них есть ссылка `children`, указывающая на коллекцию объектов **driveItem** в папке.</span><span class="sxs-lookup"><span data-stu-id="c319e-116">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c319e-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c319e-117">JSON representation</span></span>

<span data-ttu-id="c319e-118">Ниже представлено описание ресурса **driveItem** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c319e-118">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="c319e-119">Ресурс **driveItem** является производным от ресурса [**baseItem**][baseItem] и наследует его свойства.</span><span class="sxs-lookup"><span data-stu-id="c319e-119">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "content": { "@odata.type": "Edm.Stream" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "Collection(microsoft.graph.driveItemVersion)"}],

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

## <a name="properties"></a><span data-ttu-id="c319e-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="c319e-120">Properties</span></span>

| <span data-ttu-id="c319e-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="c319e-121">Property</span></span>             | <span data-ttu-id="c319e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c319e-122">Type</span></span>               | <span data-ttu-id="c319e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c319e-123">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="c319e-124">audio</span><span class="sxs-lookup"><span data-stu-id="c319e-124">audio</span></span>                | <span data-ttu-id="c319e-125">[audio][]</span><span class="sxs-lookup"><span data-stu-id="c319e-125">[audio][]</span></span>          | <span data-ttu-id="c319e-p104">Метаданные звукового файла, если элемент — звуковой файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p104">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="c319e-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="c319e-128">createdBy</span></span>            | <span data-ttu-id="c319e-129">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c319e-129">[identitySet][]</span></span>    | <span data-ttu-id="c319e-p105">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="c319e-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c319e-132">createdDateTime</span></span>      | <span data-ttu-id="c319e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c319e-133">DateTimeOffset</span></span>     | <span data-ttu-id="c319e-p106">Дата и время создания элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p106">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="c319e-136">cTag</span><span class="sxs-lookup"><span data-stu-id="c319e-136">cTag</span></span>                 | <span data-ttu-id="c319e-137">String</span><span class="sxs-lookup"><span data-stu-id="c319e-137">String</span></span>             | <span data-ttu-id="c319e-p107">ETag для содержимого элемента. Такой тег сущности не изменяется, если изменяются только метаданные. **Примечание.** Это свойство не возвращается, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p107">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="c319e-142">deleted</span><span class="sxs-lookup"><span data-stu-id="c319e-142">deleted</span></span>              | <span data-ttu-id="c319e-143">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="c319e-143">[deleted][]</span></span>        | <span data-ttu-id="c319e-p108">Сведения о состоянии удаления элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p108">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="c319e-146">описание</span><span class="sxs-lookup"><span data-stu-id="c319e-146">description</span></span>          | <span data-ttu-id="c319e-147">Строка</span><span class="sxs-lookup"><span data-stu-id="c319e-147">String</span></span>             | <span data-ttu-id="c319e-p109">Предоставляет видимое пользователю описание элемента. Чтение и запись. Только в личном хранилище OneDrive</span><span class="sxs-lookup"><span data-stu-id="c319e-p109">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="c319e-151">eTag</span><span class="sxs-lookup"><span data-stu-id="c319e-151">eTag</span></span>                 | <span data-ttu-id="c319e-152">String</span><span class="sxs-lookup"><span data-stu-id="c319e-152">String</span></span>             | <span data-ttu-id="c319e-p110">Тег сущности для всего элемента (метаданные и содержимое). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p110">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="c319e-155">file</span><span class="sxs-lookup"><span data-stu-id="c319e-155">file</span></span>                 | <span data-ttu-id="c319e-156">[file][]</span><span class="sxs-lookup"><span data-stu-id="c319e-156">[file][]</span></span>           | <span data-ttu-id="c319e-p111">Файл метаданных, если в роли элемента выступает файл. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p111">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="c319e-159">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="c319e-159">fileSystemInfo</span></span>       | <span data-ttu-id="c319e-160">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="c319e-160">[fileSystemInfo][]</span></span> | <span data-ttu-id="c319e-p112">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="c319e-p112">File system information on client. Read-write.</span></span>
| <span data-ttu-id="c319e-163">folder</span><span class="sxs-lookup"><span data-stu-id="c319e-163">folder</span></span>               | <span data-ttu-id="c319e-164">[folder][]</span><span class="sxs-lookup"><span data-stu-id="c319e-164">[folder][]</span></span>         | <span data-ttu-id="c319e-p113">Метаданные папки, если в роли элемента выступает папка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p113">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="c319e-167">id</span><span class="sxs-lookup"><span data-stu-id="c319e-167">id</span></span>                   | <span data-ttu-id="c319e-168">Строка</span><span class="sxs-lookup"><span data-stu-id="c319e-168">String</span></span>             | <span data-ttu-id="c319e-p114">Уникальный идентификатор элемента на диске. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p114">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="c319e-171">изображение</span><span class="sxs-lookup"><span data-stu-id="c319e-171">image</span></span>                | <span data-ttu-id="c319e-172">[image][]</span><span class="sxs-lookup"><span data-stu-id="c319e-172">[image][]</span></span>          | <span data-ttu-id="c319e-p115">Метаданные изображения, если в роли элемента выступает изображение. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p115">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="c319e-175">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c319e-175">lastModifiedBy</span></span>       | <span data-ttu-id="c319e-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c319e-176">[identitySet][]</span></span>    | <span data-ttu-id="c319e-p116">Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p116">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="c319e-179">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c319e-179">lastModifiedDateTime</span></span> | <span data-ttu-id="c319e-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c319e-180">DateTimeOffset</span></span>     | <span data-ttu-id="c319e-p117">Дата и время последнего изменения элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p117">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="c319e-183">location</span><span class="sxs-lookup"><span data-stu-id="c319e-183">location</span></span>             | <span data-ttu-id="c319e-184">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="c319e-184">[geoCoordinates][]</span></span> | <span data-ttu-id="c319e-p118">Метаданные местоположения, если в роли элемента выступают данные о местоположении. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p118">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="c319e-187">name</span><span class="sxs-lookup"><span data-stu-id="c319e-187">name</span></span>                 | <span data-ttu-id="c319e-188">Строка</span><span class="sxs-lookup"><span data-stu-id="c319e-188">String</span></span>             | <span data-ttu-id="c319e-p119">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="c319e-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="c319e-191">package</span><span class="sxs-lookup"><span data-stu-id="c319e-191">package</span></span>              | <span data-ttu-id="c319e-192">[package][]</span><span class="sxs-lookup"><span data-stu-id="c319e-192">[package][]</span></span>        | <span data-ttu-id="c319e-p120">В случае наличия указывает, что этот элемент — пакет, а не папка или файл. Пакеты обрабатываются как файлы в одном контексте, и как папки — в другом. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="c319e-196">parentReference</span><span class="sxs-lookup"><span data-stu-id="c319e-196">parentReference</span></span>      | <span data-ttu-id="c319e-197">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="c319e-197">[itemReference][]</span></span>  | <span data-ttu-id="c319e-p121">Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="c319e-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="c319e-200">Фотография
</span><span class="sxs-lookup"><span data-stu-id="c319e-200">photo</span></span>                | <span data-ttu-id="c319e-201">[photo][]</span><span class="sxs-lookup"><span data-stu-id="c319e-201">[photo][]</span></span>          | <span data-ttu-id="c319e-p122">Метаданные фотографии, если в роли элемента выступает фотография. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p122">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="c319e-204">publication</span><span class="sxs-lookup"><span data-stu-id="c319e-204">publication</span></span>          | <span data-ttu-id="c319e-205">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="c319e-205">[publicationFacet][]</span></span> | <span data-ttu-id="c319e-206">Предоставляет сведения о состоянии элемента (опубликован или получен для изменения) в расположениях, поддерживающих такие действия.</span><span class="sxs-lookup"><span data-stu-id="c319e-206">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="c319e-207">Это свойство не возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c319e-207">This property is not returned by default.</span></span> <span data-ttu-id="c319e-208">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-208">Read-only.</span></span> |
| <span data-ttu-id="c319e-209">remoteItem</span><span class="sxs-lookup"><span data-stu-id="c319e-209">remoteItem</span></span>           | <span data-ttu-id="c319e-210">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="c319e-210">[remoteItem][]</span></span>     | <span data-ttu-id="c319e-p124">Данные удаленного элемента, если элемент используется совместно на диске, но не на том, к которому получен доступ в данный момент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p124">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="c319e-213">root</span><span class="sxs-lookup"><span data-stu-id="c319e-213">root</span></span>                 | <span data-ttu-id="c319e-214">[root][]</span><span class="sxs-lookup"><span data-stu-id="c319e-214">[root][]</span></span>           | <span data-ttu-id="c319e-215">Ненулевое значение этого свойства указывает, что ресурс driveItem является самым верхним на диске.</span><span class="sxs-lookup"><span data-stu-id="c319e-215">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="c319e-216">searchResult</span><span class="sxs-lookup"><span data-stu-id="c319e-216">searchResult</span></span>         | <span data-ttu-id="c319e-217">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="c319e-217">[searchResult][]</span></span>   | <span data-ttu-id="c319e-p125">Поиск метаданных, если элемент получен из результата поиска. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p125">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="c319e-220">shared</span><span class="sxs-lookup"><span data-stu-id="c319e-220">shared</span></span>               | <span data-ttu-id="c319e-221">[shared][]</span><span class="sxs-lookup"><span data-stu-id="c319e-221">[shared][]</span></span>         | <span data-ttu-id="c319e-p126">Указывает, что к элементу был предоставлен общий доступ для других пользователей, и предоставляет сведения о состоянии совместного использования элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p126">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="c319e-224">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="c319e-224">sharepointIds</span></span>        | <span data-ttu-id="c319e-225">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="c319e-225">[sharepointIds][]</span></span>  | <span data-ttu-id="c319e-p127">Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p127">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="c319e-228">size</span><span class="sxs-lookup"><span data-stu-id="c319e-228">size</span></span>                 | <span data-ttu-id="c319e-229">Int64</span><span class="sxs-lookup"><span data-stu-id="c319e-229">Int64</span></span>              | <span data-ttu-id="c319e-p128">Размер элемента (в байтах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p128">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="c319e-232">specialFolder</span><span class="sxs-lookup"><span data-stu-id="c319e-232">specialFolder</span></span>        | <span data-ttu-id="c319e-233">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="c319e-233">[specialFolder][]</span></span>  | <span data-ttu-id="c319e-p129">Если текущий элемент также доступен как специальная папка, возвращается этот аспект. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p129">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="c319e-236">video</span><span class="sxs-lookup"><span data-stu-id="c319e-236">video</span></span>                | <span data-ttu-id="c319e-237">[video][]</span><span class="sxs-lookup"><span data-stu-id="c319e-237">[video][]</span></span>          | <span data-ttu-id="c319e-p130">Метаданные видео, если в роли элемента выступает видео. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p130">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="c319e-240">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="c319e-240">webDavUrl</span></span>            | <span data-ttu-id="c319e-241">Строка</span><span class="sxs-lookup"><span data-stu-id="c319e-241">String</span></span>             | <span data-ttu-id="c319e-242">URL-адрес элемента, совместимый с WebDAV.</span><span class="sxs-lookup"><span data-stu-id="c319e-242">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="c319e-243">webUrl</span><span class="sxs-lookup"><span data-stu-id="c319e-243">webUrl</span></span>               | <span data-ttu-id="c319e-244">Строка</span><span class="sxs-lookup"><span data-stu-id="c319e-244">String</span></span>             | <span data-ttu-id="c319e-p131">URL-адрес для отображения ресурса в браузере. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p131">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="c319e-p132">**Примечание.** Свойства тегов eTag и cTag по-разному действуют на контейнеры (папки). Значение cTag изменяется при изменении содержимого или метаданных любого потомка папки. Значение eTag изменяется только при изменении свойств папки, за исключением свойств, которые являются производными от потомков (например, свойство **childCount** или **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="c319e-p132">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="c319e-250">Отношения</span><span class="sxs-lookup"><span data-stu-id="c319e-250">Relationships</span></span>

| <span data-ttu-id="c319e-251">Связь</span><span class="sxs-lookup"><span data-stu-id="c319e-251">Relationship</span></span>       | <span data-ttu-id="c319e-252">Тип</span><span class="sxs-lookup"><span data-stu-id="c319e-252">Type</span></span>                            | <span data-ttu-id="c319e-253">Описание</span><span class="sxs-lookup"><span data-stu-id="c319e-253">Description</span></span>
|:-------------------|:--------------------------------|:--------------------------
| <span data-ttu-id="c319e-254">activities</span><span class="sxs-lookup"><span data-stu-id="c319e-254">activities</span></span>         | <span data-ttu-id="c319e-255">Коллекция [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="c319e-255">[itemActivity][] collection</span></span>     | <span data-ttu-id="c319e-256">Список последних действий, выполненных с элементом.</span><span class="sxs-lookup"><span data-stu-id="c319e-256">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="c319e-257">Аналитика</span><span class="sxs-lookup"><span data-stu-id="c319e-257">analytics</span></span>          | <span data-ttu-id="c319e-258">[itemAnalytics][] ресурсов</span><span class="sxs-lookup"><span data-stu-id="c319e-258">[itemAnalytics][] resource</span></span>      | <span data-ttu-id="c319e-259">Аналитика о Просмотр действий, выполняемых по этому элементу.</span><span class="sxs-lookup"><span data-stu-id="c319e-259">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="c319e-260">content</span><span class="sxs-lookup"><span data-stu-id="c319e-260">content</span></span>            | <span data-ttu-id="c319e-261">Поток</span><span class="sxs-lookup"><span data-stu-id="c319e-261">Stream</span></span>                          | <span data-ttu-id="c319e-262">Поток содержимого, если элемент представляет файл.</span><span class="sxs-lookup"><span data-stu-id="c319e-262">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="c319e-263">children</span><span class="sxs-lookup"><span data-stu-id="c319e-263">children</span></span>           | <span data-ttu-id="c319e-264">Коллекция объектов driveItem</span><span class="sxs-lookup"><span data-stu-id="c319e-264">driveitem collection</span></span>            | <span data-ttu-id="c319e-p133">Коллекция, содержащая объекты Item для непосредственных дочерних элементов данного ресурса Item. Дочерние элементы есть только у элементов, представляющих папки. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c319e-p133">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="c319e-269">listItem</span><span class="sxs-lookup"><span data-stu-id="c319e-269">listItem</span></span>           | <span data-ttu-id="c319e-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="c319e-270">[listItem][]</span></span>                    | <span data-ttu-id="c319e-271">Для дисков в SharePoint, элемент списка библиотеки связанного с ним документа.</span><span class="sxs-lookup"><span data-stu-id="c319e-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="c319e-272">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-272">Read-only.</span></span> <span data-ttu-id="c319e-273">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c319e-273">Nullable.</span></span>
| <span data-ttu-id="c319e-274">permissions</span><span class="sxs-lookup"><span data-stu-id="c319e-274">permissions</span></span>        | <span data-ttu-id="c319e-275">Коллекция объектов [permission][]</span><span class="sxs-lookup"><span data-stu-id="c319e-275">[permission][] collection</span></span>       | <span data-ttu-id="c319e-p135">Набор разрешений для элемента. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c319e-p135">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="c319e-279">thumbnails</span><span class="sxs-lookup"><span data-stu-id="c319e-279">thumbnails</span></span>         | <span data-ttu-id="c319e-280">Коллекция объектов [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="c319e-280">[thumbnailSet][] collection</span></span>     | <span data-ttu-id="c319e-p136">Коллекция, содержащая объекты [ThumbnailSet][], связанные с элементом. Дополнительные сведения см. в статье о [получении эскизов][]. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c319e-p136">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="c319e-285">версии</span><span class="sxs-lookup"><span data-stu-id="c319e-285">versions</span></span>           | <span data-ttu-id="c319e-286">[driveItemVersion][] коллекции</span><span class="sxs-lookup"><span data-stu-id="c319e-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="c319e-287">Список предыдущих версий элемента.</span><span class="sxs-lookup"><span data-stu-id="c319e-287">The list of previous versions of the item.</span></span> <span data-ttu-id="c319e-288">Дополнительные сведения см.в [Получение предыдущих версий][].</span><span class="sxs-lookup"><span data-stu-id="c319e-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="c319e-289">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-289">Read-only.</span></span> <span data-ttu-id="c319e-290">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c319e-290">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="c319e-291">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="c319e-291">Instance Attributes</span></span>

<span data-ttu-id="c319e-p138">Атрибуты экземпляра — это свойства с особым поведением. Эти свойства — временные и а) определяют поведение выполнения службы; или б) предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, у которого истекает срок действия.</span><span class="sxs-lookup"><span data-stu-id="c319e-p138">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="c319e-294">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c319e-294">Property name</span></span>                     | <span data-ttu-id="c319e-295">Тип</span><span class="sxs-lookup"><span data-stu-id="c319e-295">Type</span></span>   | <span data-ttu-id="c319e-296">Описание</span><span class="sxs-lookup"><span data-stu-id="c319e-296">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="c319e-297">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="c319e-297">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="c319e-298">string</span><span class="sxs-lookup"><span data-stu-id="c319e-298">string</span></span> | <span data-ttu-id="c319e-p139">Определяет поведение для разрешения конфликтов, возникающих при создании элементов. Вы можете использовать значения *fail*, *replace* или *rename*. Значение по умолчанию для метода PUT: *replace*. Элементы никогда не возвращаются с такой заметкой. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="c319e-p139">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="c319e-304">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="c319e-304">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="c319e-305">string</span><span class="sxs-lookup"><span data-stu-id="c319e-305">string</span></span> | <span data-ttu-id="c319e-p140">URL-адрес, который можно использовать для скачивания содержимого этого файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c319e-p140">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="c319e-309">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="c319e-309">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="c319e-310">string</span><span class="sxs-lookup"><span data-stu-id="c319e-310">string</span></span> | <span data-ttu-id="c319e-p141">При создании запроса PUT такую заметку экземпляра можно использовать, чтобы указать службе скачать содержимое по URL-адресу и сохранить его как файл. Только для записи.</span><span class="sxs-lookup"><span data-stu-id="c319e-p141">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="c319e-313">**Примечание:** Значение @microsoft.graph.downloadUrl кратковременного URL-адрес и не может быть кэширования.</span><span class="sxs-lookup"><span data-stu-id="c319e-313">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="c319e-314">URL-адрес будет доступно только на короткое время (1 час) перед их недействительными.</span><span class="sxs-lookup"><span data-stu-id="c319e-314">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span> <span data-ttu-id="c319e-315">Удаление файла разрешения для пользователя может не делают недействительными сразу же URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="c319e-315">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="c319e-316">Методы</span><span class="sxs-lookup"><span data-stu-id="c319e-316">Methods</span></span>

| <span data-ttu-id="c319e-317">Метод</span><span class="sxs-lookup"><span data-stu-id="c319e-317">Method</span></span>                                                   | <span data-ttu-id="c319e-318">Путь REST</span><span class="sxs-lookup"><span data-stu-id="c319e-318">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="c319e-319">Получение элемента</span><span class="sxs-lookup"><span data-stu-id="c319e-319">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="c319e-320">Список действий</span><span class="sxs-lookup"><span data-stu-id="c319e-320">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="c319e-321">[Получение аналитики][]</span><span class="sxs-lookup"><span data-stu-id="c319e-321">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="c319e-322">[Получение действий по интервал][]</span><span class="sxs-lookup"><span data-stu-id="c319e-322">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="c319e-323">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="c319e-323">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="c319e-324">Список версий</span><span class="sxs-lookup"><span data-stu-id="c319e-324">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="c319e-325">Создание элемента</span><span class="sxs-lookup"><span data-stu-id="c319e-325">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="c319e-326">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="c319e-326">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="c319e-327">Отправка содержимого</span><span class="sxs-lookup"><span data-stu-id="c319e-327">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="c319e-328">Скачивание содержимого</span><span class="sxs-lookup"><span data-stu-id="c319e-328">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="c319e-329">[Скачивание файла в определенном формате][download-format]</span><span class="sxs-lookup"><span data-stu-id="c319e-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="c319e-330">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="c319e-330">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="c319e-331">Перемещение элемента</span><span class="sxs-lookup"><span data-stu-id="c319e-331">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="c319e-332">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="c319e-332">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="c319e-333">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="c319e-333">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="c319e-334">Перечисление изменений на диске</span><span class="sxs-lookup"><span data-stu-id="c319e-334">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="c319e-335">Перечисление эскизов</span><span class="sxs-lookup"><span data-stu-id="c319e-335">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="c319e-336">Создание ссылки совместного доступа</span><span class="sxs-lookup"><span data-stu-id="c319e-336">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="c319e-337">Добавление разрешений</span><span class="sxs-lookup"><span data-stu-id="c319e-337">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="c319e-338">Список разрешений</span><span class="sxs-lookup"><span data-stu-id="c319e-338">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="c319e-339">Удаление разрешения</span><span class="sxs-lookup"><span data-stu-id="c319e-339">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="c319e-340">[Получение WebSocket канала][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="c319e-340">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="c319e-341">[Просмотр элемента][item-preview]</span><span class="sxs-lookup"><span data-stu-id="c319e-341">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[Получение аналитики]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Получение действий по интервал]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="c319e-344">Заметки</span><span class="sxs-lookup"><span data-stu-id="c319e-344">Remarks</span></span>

<span data-ttu-id="c319e-345">В OneDrive для бизнеса и библиотеках документов SharePoint свойство **cTag** не возвращается, если у ресурса **driveItem** есть аспект [folder][].</span><span class="sxs-lookup"><span data-stu-id="c319e-345">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md;
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[Получение предыдущих версий.]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[получении эскизов]: ../api/driveitem-list-thumbnails.md
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
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
