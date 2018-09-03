# <a name="listitemversion-resource-type"></a><span data-ttu-id="89264-101">Тип ресурса ListItemVersion</span><span class="sxs-lookup"><span data-stu-id="89264-101">ListItemVersion resource type</span></span>

<span data-ttu-id="89264-102">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="89264-102">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="89264-103">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="89264-103">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="89264-104">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="89264-104">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="89264-105">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="89264-105">Common task</span></span>             |         <span data-ttu-id="89264-106">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="89264-106">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="89264-107">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="89264-107">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="89264-108">[Получение версии][version-get]</span><span class="sxs-lookup"><span data-stu-id="89264-108">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="89264-109">[Восстановление версии][version-restore]</span><span class="sxs-lookup"><span data-stu-id="89264-109">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem_list_versions.md
[version-get]: ../api/listitemversion_get.md
[version-restore]: ../api/listitemversion_restore.md


## <a name="json-representation"></a><span data-ttu-id="89264-110">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89264-110">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="89264-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="89264-111">Properties</span></span>

|      <span data-ttu-id="89264-112">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="89264-112">Property name</span></span>       |                         <span data-ttu-id="89264-113">Тип</span><span class="sxs-lookup"><span data-stu-id="89264-113">Type</span></span>                         |                               <span data-ttu-id="89264-114">Описание</span><span class="sxs-lookup"><span data-stu-id="89264-114">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="89264-115">**id**</span><span class="sxs-lookup"><span data-stu-id="89264-115">**id**</span></span>                   | <span data-ttu-id="89264-116">строка</span><span class="sxs-lookup"><span data-stu-id="89264-116">string</span></span>                                               | <span data-ttu-id="89264-117">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="89264-117">The ID of the version.</span></span> <span data-ttu-id="89264-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89264-118">Read-only.</span></span>                                       |
| <span data-ttu-id="89264-119">****lastModifiedBy**;**</span><span class="sxs-lookup"><span data-stu-id="89264-119">**lastModifiedBy**</span></span>       | [<span data-ttu-id="89264-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="89264-120">IdentitySet</span></span>](../resources/identitySet.md)           | <span data-ttu-id="89264-121">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="89264-121">Identity of the user which last modified the version.</span></span> <span data-ttu-id="89264-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89264-122">Read-only.</span></span>        |
| <span data-ttu-id="89264-123">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="89264-123">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="89264-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89264-124">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="89264-125">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="89264-125">Date and time the version was last modified.</span></span> <span data-ttu-id="89264-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89264-126">Read-only.</span></span>                 |
| <span data-ttu-id="89264-127">**published**</span><span class="sxs-lookup"><span data-stu-id="89264-127">**published**</span></span>            | [<span data-ttu-id="89264-128">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="89264-128">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="89264-129">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="89264-129">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="89264-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89264-130">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="89264-131">Связи</span><span class="sxs-lookup"><span data-stu-id="89264-131">Relationships</span></span>

<span data-ttu-id="89264-132">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="89264-132">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="89264-133">Имя связи</span><span class="sxs-lookup"><span data-stu-id="89264-133">Relationship name</span></span> |                      <span data-ttu-id="89264-134">Тип</span><span class="sxs-lookup"><span data-stu-id="89264-134">Type</span></span>                      |                               <span data-ttu-id="89264-135">Описание</span><span class="sxs-lookup"><span data-stu-id="89264-135">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="89264-136">**fields**</span><span class="sxs-lookup"><span data-stu-id="89264-136">**fields**</span></span>        | [<span data-ttu-id="89264-137">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="89264-137">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="89264-138">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="89264-138">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
