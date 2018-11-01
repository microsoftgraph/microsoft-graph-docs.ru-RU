# <a name="driveitemversion-resource-type"></a><span data-ttu-id="76fbe-101">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="76fbe-101">DriveItemVersion resource type</span></span>

<span data-ttu-id="76fbe-102">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="76fbe-102">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="76fbe-103">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="76fbe-103">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="76fbe-104">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="76fbe-104">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="76fbe-105">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="76fbe-105">Common task</span></span>             |         <span data-ttu-id="76fbe-106">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="76fbe-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="76fbe-107">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="76fbe-107">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="76fbe-108">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="76fbe-108">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="76fbe-109">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="76fbe-109">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="76fbe-110">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="76fbe-110">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem_list_versions.md
[version-get]: ../api/driveitemversion_get.md
[content-get]: ../api/driveitemversion_get_contents.md
[version-restore]: ../api/driveitemversion_restore.md

<span data-ttu-id="76fbe-111">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="76fbe-111">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76fbe-112">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="76fbe-112">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="76fbe-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="76fbe-113">Properties</span></span>

|      <span data-ttu-id="76fbe-114">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="76fbe-114">Property name</span></span>       |                         <span data-ttu-id="76fbe-115">Тип</span><span class="sxs-lookup"><span data-stu-id="76fbe-115">Type</span></span>                         |                               <span data-ttu-id="76fbe-116">Описание</span><span class="sxs-lookup"><span data-stu-id="76fbe-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="76fbe-117">**id**</span><span class="sxs-lookup"><span data-stu-id="76fbe-117">**id**</span></span>                   | <span data-ttu-id="76fbe-118">string</span><span class="sxs-lookup"><span data-stu-id="76fbe-118">string</span></span>                                               | <span data-ttu-id="76fbe-119">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="76fbe-119">The ID of the version.</span></span> <span data-ttu-id="76fbe-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76fbe-120">Read-only.</span></span>                                       |
| <span data-ttu-id="76fbe-121">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="76fbe-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="76fbe-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="76fbe-122">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="76fbe-123">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="76fbe-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="76fbe-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76fbe-124">Read-only.</span></span>        |
| <span data-ttu-id="76fbe-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="76fbe-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="76fbe-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76fbe-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="76fbe-127">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="76fbe-127">Date and time the version was last modified.</span></span> <span data-ttu-id="76fbe-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76fbe-128">Read-only.</span></span>                 |
| <span data-ttu-id="76fbe-129">**publication**</span><span class="sxs-lookup"><span data-stu-id="76fbe-129">**publication**</span></span>          | [<span data-ttu-id="76fbe-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="76fbe-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="76fbe-131">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="76fbe-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="76fbe-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76fbe-132">Read-only.</span></span> |
| <span data-ttu-id="76fbe-133">**size**</span><span class="sxs-lookup"><span data-stu-id="76fbe-133">**size**</span></span>                 | <span data-ttu-id="76fbe-134">Int64</span><span class="sxs-lookup"><span data-stu-id="76fbe-134">Int64</span></span>                                                | <span data-ttu-id="76fbe-135">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="76fbe-135">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="76fbe-136">**content**</span><span class="sxs-lookup"><span data-stu-id="76fbe-136">**content**</span></span>              | <span data-ttu-id="76fbe-137">Stream</span><span class="sxs-lookup"><span data-stu-id="76fbe-137">Stream</span></span>                                               | <span data-ttu-id="76fbe-138">Поток содержимого для данной версии элемента.</span><span class="sxs-lookup"><span data-stu-id="76fbe-138">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
