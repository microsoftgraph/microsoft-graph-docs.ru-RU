---
title: Тип ресурса listItemVersion
description: Ресурс **listItemVersion** представляет предыдущую версию ресурса ListItem.
ms.openlocfilehash: f036ea217abe766806e7f3c6b24bee4394f54889
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024506"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="c67bf-103">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="c67bf-103">ListItemVersion resource type</span></span>

<span data-ttu-id="c67bf-104">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="c67bf-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="c67bf-105">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="c67bf-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="c67bf-106">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="c67bf-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="c67bf-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="c67bf-107">Common task</span></span>             |         <span data-ttu-id="c67bf-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="c67bf-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="c67bf-109">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="c67bf-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="c67bf-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="c67bf-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="c67bf-111">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="c67bf-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="c67bf-112">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c67bf-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c67bf-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="c67bf-113">Properties</span></span>

|      <span data-ttu-id="c67bf-114">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c67bf-114">Property name</span></span>       |                         <span data-ttu-id="c67bf-115">Тип</span><span class="sxs-lookup"><span data-stu-id="c67bf-115">Type</span></span>                         |                               <span data-ttu-id="c67bf-116">Описание</span><span class="sxs-lookup"><span data-stu-id="c67bf-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="c67bf-117">**id**</span><span class="sxs-lookup"><span data-stu-id="c67bf-117">**id**</span></span>                   | <span data-ttu-id="c67bf-118">строка</span><span class="sxs-lookup"><span data-stu-id="c67bf-118">string</span></span>                                               | <span data-ttu-id="c67bf-119">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="c67bf-119">The ID of the version.</span></span> <span data-ttu-id="c67bf-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c67bf-120">Read-only.</span></span>                                       |
| <span data-ttu-id="c67bf-121">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="c67bf-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="c67bf-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c67bf-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="c67bf-123">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="c67bf-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="c67bf-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c67bf-124">Read-only.</span></span>        |
| <span data-ttu-id="c67bf-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c67bf-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="c67bf-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c67bf-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="c67bf-127">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="c67bf-127">Date and time the version was last modified.</span></span> <span data-ttu-id="c67bf-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c67bf-128">Read-only.</span></span>                 |
| <span data-ttu-id="c67bf-129">**published**</span><span class="sxs-lookup"><span data-stu-id="c67bf-129">**published**</span></span>            | [<span data-ttu-id="c67bf-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="c67bf-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="c67bf-131">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="c67bf-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="c67bf-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c67bf-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="c67bf-133">Связи</span><span class="sxs-lookup"><span data-stu-id="c67bf-133">Relationships</span></span>

<span data-ttu-id="c67bf-134">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="c67bf-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="c67bf-135">Имя связи</span><span class="sxs-lookup"><span data-stu-id="c67bf-135">Relationship name</span></span> |                      <span data-ttu-id="c67bf-136">Тип</span><span class="sxs-lookup"><span data-stu-id="c67bf-136">Type</span></span>                      |                               <span data-ttu-id="c67bf-137">Описание</span><span class="sxs-lookup"><span data-stu-id="c67bf-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="c67bf-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="c67bf-138">**fields**</span></span>        | [<span data-ttu-id="c67bf-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="c67bf-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="c67bf-140">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="c67bf-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
