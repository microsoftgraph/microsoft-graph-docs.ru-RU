---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: listItemVersion.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d153a8ae8291e0299d1a470db6c8c7e0c8bd3e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524753"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="b31fa-102">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="b31fa-102">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b31fa-103">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="b31fa-103">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="b31fa-104">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="b31fa-104">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="b31fa-105">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="b31fa-105">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="b31fa-106">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="b31fa-106">Common task</span></span>             |         <span data-ttu-id="b31fa-107">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="b31fa-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="b31fa-108">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="b31fa-108">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="b31fa-109">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="b31fa-109">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="b31fa-110">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="b31fa-110">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="b31fa-111">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b31fa-111">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

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

## <a name="properties"></a><span data-ttu-id="b31fa-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="b31fa-112">Properties</span></span>

|      <span data-ttu-id="b31fa-113">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b31fa-113">Property name</span></span>       |                         <span data-ttu-id="b31fa-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b31fa-114">Type</span></span>                         |                               <span data-ttu-id="b31fa-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b31fa-115">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="b31fa-116">**id**</span><span class="sxs-lookup"><span data-stu-id="b31fa-116">**id**</span></span>                   | <span data-ttu-id="b31fa-117">string</span><span class="sxs-lookup"><span data-stu-id="b31fa-117">string</span></span>                                               | <span data-ttu-id="b31fa-118">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="b31fa-118">The ID of the version.</span></span> <span data-ttu-id="b31fa-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b31fa-119">Read-only.</span></span>                                       |
| <span data-ttu-id="b31fa-120">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="b31fa-120">**lastModifiedBy**</span></span>       | [<span data-ttu-id="b31fa-121">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b31fa-121">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="b31fa-122">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="b31fa-122">Identity of the user which last modified the version.</span></span> <span data-ttu-id="b31fa-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b31fa-123">Read-only.</span></span>        |
| <span data-ttu-id="b31fa-124">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b31fa-124">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="b31fa-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b31fa-125">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="b31fa-126">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="b31fa-126">Date and time the version was last modified.</span></span> <span data-ttu-id="b31fa-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b31fa-127">Read-only.</span></span>                 |
| <span data-ttu-id="b31fa-128">**published**</span><span class="sxs-lookup"><span data-stu-id="b31fa-128">**published**</span></span>            | [<span data-ttu-id="b31fa-129">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="b31fa-129">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="b31fa-130">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="b31fa-130">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="b31fa-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b31fa-131">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="b31fa-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b31fa-132">Relationships</span></span>

<span data-ttu-id="b31fa-133">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="b31fa-133">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="b31fa-134">Имя связи</span><span class="sxs-lookup"><span data-stu-id="b31fa-134">Relationship name</span></span> |                      <span data-ttu-id="b31fa-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b31fa-135">Type</span></span>                      |                               <span data-ttu-id="b31fa-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b31fa-136">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="b31fa-137">**fields**</span><span class="sxs-lookup"><span data-stu-id="b31fa-137">**fields**</span></span>        | [<span data-ttu-id="b31fa-138">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="b31fa-138">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="b31fa-139">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="b31fa-139">A collection of the fields and values for this version of the list item.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/listitemversion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
