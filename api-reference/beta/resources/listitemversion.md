---
author: JeremyKelley
description: Ресурс listItemVersion представляет предыдущую версию ресурса ListItem.
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ff3fbd3144a62939f9d4f6077c556c9d5884c687
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966967"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="cbc6a-103">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="cbc6a-103">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbc6a-104">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="cbc6a-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="cbc6a-105">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="cbc6a-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="cbc6a-106">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="cbc6a-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="cbc6a-107">Common task</span></span>             |         <span data-ttu-id="cbc6a-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="cbc6a-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="cbc6a-109">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="cbc6a-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="cbc6a-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="cbc6a-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="cbc6a-111">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="cbc6a-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="cbc6a-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbc6a-112">JSON representation</span></span>

<!-- { "blockType": "resource","keyProperty":"id", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="cbc6a-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbc6a-113">Properties</span></span>

|      <span data-ttu-id="cbc6a-114">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="cbc6a-114">Property name</span></span>       |                         <span data-ttu-id="cbc6a-115">Тип</span><span class="sxs-lookup"><span data-stu-id="cbc6a-115">Type</span></span>                         |                               <span data-ttu-id="cbc6a-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cbc6a-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="cbc6a-117">**id**</span><span class="sxs-lookup"><span data-stu-id="cbc6a-117">**id**</span></span>                   | <span data-ttu-id="cbc6a-118">string</span><span class="sxs-lookup"><span data-stu-id="cbc6a-118">string</span></span>                                               | <span data-ttu-id="cbc6a-119">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-119">The ID of the version.</span></span> <span data-ttu-id="cbc6a-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-120">Read-only.</span></span>                                       |
| <span data-ttu-id="cbc6a-121">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="cbc6a-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="cbc6a-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="cbc6a-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="cbc6a-123">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="cbc6a-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-124">Read-only.</span></span>        |
| <span data-ttu-id="cbc6a-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="cbc6a-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="cbc6a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbc6a-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="cbc6a-127">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-127">Date and time the version was last modified.</span></span> <span data-ttu-id="cbc6a-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-128">Read-only.</span></span>                 |
| <span data-ttu-id="cbc6a-129">**published**</span><span class="sxs-lookup"><span data-stu-id="cbc6a-129">**published**</span></span>            | [<span data-ttu-id="cbc6a-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="cbc6a-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="cbc6a-131">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="cbc6a-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="cbc6a-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="cbc6a-133">Relationships</span></span>

<span data-ttu-id="cbc6a-134">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="cbc6a-135">Имя связи</span><span class="sxs-lookup"><span data-stu-id="cbc6a-135">Relationship name</span></span> |                      <span data-ttu-id="cbc6a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="cbc6a-136">Type</span></span>                      |                               <span data-ttu-id="cbc6a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="cbc6a-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="cbc6a-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="cbc6a-138">**fields**</span></span>        | [<span data-ttu-id="cbc6a-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="cbc6a-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="cbc6a-140">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="cbc6a-140">A collection of the fields and values for this version of the list item.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
