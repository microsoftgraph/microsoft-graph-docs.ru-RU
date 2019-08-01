---
title: Тип ресурса listItemVersion
description: Ресурс **listItemVersion** представляет предыдущую версию ресурса ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 8523e77fd308ab4863a0c3d90ccacad73cc766cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036451"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="db81b-103">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="db81b-103">ListItemVersion resource type</span></span>

<span data-ttu-id="db81b-104">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="db81b-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="db81b-105">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="db81b-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="db81b-106">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="db81b-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="db81b-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="db81b-107">Common task</span></span>             |         <span data-ttu-id="db81b-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="db81b-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="db81b-109">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="db81b-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="db81b-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="db81b-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="db81b-111">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="db81b-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="db81b-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db81b-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="db81b-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="db81b-113">Properties</span></span>

|      <span data-ttu-id="db81b-114">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="db81b-114">Property name</span></span>       |                         <span data-ttu-id="db81b-115">Тип</span><span class="sxs-lookup"><span data-stu-id="db81b-115">Type</span></span>                         |                               <span data-ttu-id="db81b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="db81b-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="db81b-117">**id**</span><span class="sxs-lookup"><span data-stu-id="db81b-117">**id**</span></span>                   | <span data-ttu-id="db81b-118">string</span><span class="sxs-lookup"><span data-stu-id="db81b-118">string</span></span>                                               | <span data-ttu-id="db81b-119">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="db81b-119">The ID of the version.</span></span> <span data-ttu-id="db81b-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db81b-120">Read-only.</span></span>                                       |
| <span data-ttu-id="db81b-121">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="db81b-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="db81b-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="db81b-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="db81b-123">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="db81b-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="db81b-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db81b-124">Read-only.</span></span>        |
| <span data-ttu-id="db81b-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="db81b-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="db81b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db81b-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="db81b-127">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="db81b-127">Date and time the version was last modified.</span></span> <span data-ttu-id="db81b-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db81b-128">Read-only.</span></span>                 |
| <span data-ttu-id="db81b-129">**published**</span><span class="sxs-lookup"><span data-stu-id="db81b-129">**published**</span></span>            | [<span data-ttu-id="db81b-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="db81b-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="db81b-131">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="db81b-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="db81b-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db81b-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="db81b-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="db81b-133">Relationships</span></span>

<span data-ttu-id="db81b-134">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="db81b-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="db81b-135">Имя связи</span><span class="sxs-lookup"><span data-stu-id="db81b-135">Relationship name</span></span> |                      <span data-ttu-id="db81b-136">Тип</span><span class="sxs-lookup"><span data-stu-id="db81b-136">Type</span></span>                      |                               <span data-ttu-id="db81b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="db81b-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="db81b-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="db81b-138">**fields**</span></span>        | [<span data-ttu-id="db81b-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="db81b-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="db81b-140">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="db81b-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
