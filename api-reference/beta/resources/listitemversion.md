---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: abc6187f4e0ef415ec8a01088fd02aa406b1bc50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933416"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="e3423-102">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="e3423-102">ListItemVersion resource type</span></span>

> <span data-ttu-id="e3423-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3423-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3423-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3423-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3423-105">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="e3423-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="e3423-106">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="e3423-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="e3423-107">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="e3423-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="e3423-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="e3423-108">Common task</span></span>             |         <span data-ttu-id="e3423-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="e3423-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="e3423-110">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="e3423-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="e3423-111">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="e3423-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="e3423-112">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="e3423-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="e3423-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3423-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e3423-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3423-114">Properties</span></span>

|      <span data-ttu-id="e3423-115">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e3423-115">Property name</span></span>       |                         <span data-ttu-id="e3423-116">Тип</span><span class="sxs-lookup"><span data-stu-id="e3423-116">Type</span></span>                         |                               <span data-ttu-id="e3423-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e3423-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="e3423-118">**id**</span><span class="sxs-lookup"><span data-stu-id="e3423-118">**id**</span></span>                   | <span data-ttu-id="e3423-119">строка</span><span class="sxs-lookup"><span data-stu-id="e3423-119">string</span></span>                                               | <span data-ttu-id="e3423-120">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="e3423-120">The ID of the version.</span></span> <span data-ttu-id="e3423-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3423-121">Read-only.</span></span>                                       |
| <span data-ttu-id="e3423-122">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="e3423-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="e3423-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e3423-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="e3423-124">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="e3423-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="e3423-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3423-125">Read-only.</span></span>        |
| <span data-ttu-id="e3423-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e3423-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="e3423-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3423-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="e3423-128">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="e3423-128">Date and time the version was last modified.</span></span> <span data-ttu-id="e3423-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3423-129">Read-only.</span></span>                 |
| <span data-ttu-id="e3423-130">**published**</span><span class="sxs-lookup"><span data-stu-id="e3423-130">**published**</span></span>            | [<span data-ttu-id="e3423-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="e3423-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="e3423-132">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="e3423-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="e3423-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3423-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="e3423-134">Связи</span><span class="sxs-lookup"><span data-stu-id="e3423-134">Relationships</span></span>

<span data-ttu-id="e3423-135">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="e3423-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="e3423-136">Имя связи</span><span class="sxs-lookup"><span data-stu-id="e3423-136">Relationship name</span></span> |                      <span data-ttu-id="e3423-137">Тип</span><span class="sxs-lookup"><span data-stu-id="e3423-137">Type</span></span>                      |                               <span data-ttu-id="e3423-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e3423-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="e3423-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="e3423-139">**fields**</span></span>        | [<span data-ttu-id="e3423-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="e3423-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="e3423-141">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="e3423-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
