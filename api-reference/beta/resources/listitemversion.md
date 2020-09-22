---
author: JeremyKelley
description: Ресурс listItemVersion представляет предыдущую версию ресурса ListItem.
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: de11928d2ac6f0f78e2dabbd34ebb25d927c5aa9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055241"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="db716-103">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="db716-103">ListItemVersion resource type</span></span>

<span data-ttu-id="db716-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db716-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db716-105">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="db716-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="db716-106">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="db716-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="db716-107">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="db716-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="db716-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="db716-108">Common task</span></span>             |         <span data-ttu-id="db716-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="db716-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="db716-110">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="db716-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="db716-111">[Получение версии][version-get]</span><span class="sxs-lookup"><span data-stu-id="db716-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="db716-112">[Восстановление версии][version-restore]</span><span class="sxs-lookup"><span data-stu-id="db716-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="db716-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db716-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="db716-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="db716-114">Properties</span></span>

|      <span data-ttu-id="db716-115">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="db716-115">Property name</span></span>       |                         <span data-ttu-id="db716-116">Тип</span><span class="sxs-lookup"><span data-stu-id="db716-116">Type</span></span>                         |                               <span data-ttu-id="db716-117">Описание</span><span class="sxs-lookup"><span data-stu-id="db716-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="db716-118">**id**</span><span class="sxs-lookup"><span data-stu-id="db716-118">**id**</span></span>                   | <span data-ttu-id="db716-119">string</span><span class="sxs-lookup"><span data-stu-id="db716-119">string</span></span>                                               | <span data-ttu-id="db716-120">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="db716-120">The ID of the version.</span></span> <span data-ttu-id="db716-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db716-121">Read-only.</span></span>                                       |
| <span data-ttu-id="db716-122">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="db716-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="db716-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="db716-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="db716-124">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="db716-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="db716-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db716-125">Read-only.</span></span>        |
| <span data-ttu-id="db716-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="db716-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="db716-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db716-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="db716-128">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="db716-128">Date and time the version was last modified.</span></span> <span data-ttu-id="db716-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db716-129">Read-only.</span></span>                 |
| <span data-ttu-id="db716-130">**published**</span><span class="sxs-lookup"><span data-stu-id="db716-130">**published**</span></span>            | [<span data-ttu-id="db716-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="db716-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="db716-132">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="db716-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="db716-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db716-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="db716-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="db716-134">Relationships</span></span>

<span data-ttu-id="db716-135">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="db716-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="db716-136">Имя связи</span><span class="sxs-lookup"><span data-stu-id="db716-136">Relationship name</span></span> |                      <span data-ttu-id="db716-137">Тип</span><span class="sxs-lookup"><span data-stu-id="db716-137">Type</span></span>                      |                               <span data-ttu-id="db716-138">Описание</span><span class="sxs-lookup"><span data-stu-id="db716-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="db716-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="db716-139">**fields**</span></span>        | [<span data-ttu-id="db716-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="db716-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="db716-141">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="db716-141">A collection of the fields and values for this version of the list item.</span></span> |


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


