---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 56413ad243e5c6c2c2a7ae3a81dab50586f42db8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345245"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="aacd5-102">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="aacd5-102">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aacd5-103">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="aacd5-103">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="aacd5-104">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="aacd5-104">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="aacd5-105">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="aacd5-105">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="aacd5-106">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="aacd5-106">Common task</span></span>             |         <span data-ttu-id="aacd5-107">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="aacd5-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="aacd5-108">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="aacd5-108">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="aacd5-109">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="aacd5-109">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="aacd5-110">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="aacd5-110">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="aacd5-111">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aacd5-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="aacd5-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="aacd5-112">Properties</span></span>

|      <span data-ttu-id="aacd5-113">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="aacd5-113">Property name</span></span>       |                         <span data-ttu-id="aacd5-114">Тип</span><span class="sxs-lookup"><span data-stu-id="aacd5-114">Type</span></span>                         |                               <span data-ttu-id="aacd5-115">Описание</span><span class="sxs-lookup"><span data-stu-id="aacd5-115">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="aacd5-116">**id**</span><span class="sxs-lookup"><span data-stu-id="aacd5-116">**id**</span></span>                   | <span data-ttu-id="aacd5-117">string</span><span class="sxs-lookup"><span data-stu-id="aacd5-117">string</span></span>                                               | <span data-ttu-id="aacd5-118">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="aacd5-118">The ID of the version.</span></span> <span data-ttu-id="aacd5-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aacd5-119">Read-only.</span></span>                                       |
| <span data-ttu-id="aacd5-120">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="aacd5-120">**lastModifiedBy**</span></span>       | [<span data-ttu-id="aacd5-121">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="aacd5-121">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="aacd5-122">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="aacd5-122">Identity of the user which last modified the version.</span></span> <span data-ttu-id="aacd5-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aacd5-123">Read-only.</span></span>        |
| <span data-ttu-id="aacd5-124">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="aacd5-124">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="aacd5-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aacd5-125">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="aacd5-126">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="aacd5-126">Date and time the version was last modified.</span></span> <span data-ttu-id="aacd5-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aacd5-127">Read-only.</span></span>                 |
| <span data-ttu-id="aacd5-128">**published**</span><span class="sxs-lookup"><span data-stu-id="aacd5-128">**published**</span></span>            | [<span data-ttu-id="aacd5-129">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="aacd5-129">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="aacd5-130">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="aacd5-130">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="aacd5-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aacd5-131">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="aacd5-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="aacd5-132">Relationships</span></span>

<span data-ttu-id="aacd5-133">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="aacd5-133">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="aacd5-134">Имя связи</span><span class="sxs-lookup"><span data-stu-id="aacd5-134">Relationship name</span></span> |                      <span data-ttu-id="aacd5-135">Тип</span><span class="sxs-lookup"><span data-stu-id="aacd5-135">Type</span></span>                      |                               <span data-ttu-id="aacd5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="aacd5-136">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="aacd5-137">**fields**</span><span class="sxs-lookup"><span data-stu-id="aacd5-137">**fields**</span></span>        | [<span data-ttu-id="aacd5-138">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="aacd5-138">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="aacd5-139">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="aacd5-139">A collection of the fields and values for this version of the list item.</span></span> |


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
