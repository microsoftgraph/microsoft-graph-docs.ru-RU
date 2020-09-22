---
title: Тип ресурса listItemVersion
description: Ресурс **listItemVersion** представляет предыдущую версию ресурса ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 3d93917cab8e592a12385853d7c4051d37d3a3da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079153"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="d5d80-103">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="d5d80-103">ListItemVersion resource type</span></span>

<span data-ttu-id="d5d80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5d80-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5d80-105">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="d5d80-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="d5d80-106">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="d5d80-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="d5d80-107">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="d5d80-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="d5d80-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="d5d80-108">Common task</span></span>             |         <span data-ttu-id="d5d80-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="d5d80-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="d5d80-110">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="d5d80-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="d5d80-111">[Получение версии][version-get]</span><span class="sxs-lookup"><span data-stu-id="d5d80-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="d5d80-112">[Восстановление версии][version-restore]</span><span class="sxs-lookup"><span data-stu-id="d5d80-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="d5d80-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5d80-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d5d80-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5d80-114">Properties</span></span>

|      <span data-ttu-id="d5d80-115">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d5d80-115">Property name</span></span>       |                         <span data-ttu-id="d5d80-116">Тип</span><span class="sxs-lookup"><span data-stu-id="d5d80-116">Type</span></span>                         |                               <span data-ttu-id="d5d80-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d5d80-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="d5d80-118">**id**</span><span class="sxs-lookup"><span data-stu-id="d5d80-118">**id**</span></span>                   | <span data-ttu-id="d5d80-119">string</span><span class="sxs-lookup"><span data-stu-id="d5d80-119">string</span></span>                                               | <span data-ttu-id="d5d80-120">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="d5d80-120">The ID of the version.</span></span> <span data-ttu-id="d5d80-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5d80-121">Read-only.</span></span>                                       |
| <span data-ttu-id="d5d80-122">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="d5d80-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="d5d80-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d5d80-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="d5d80-124">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="d5d80-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="d5d80-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5d80-125">Read-only.</span></span>        |
| <span data-ttu-id="d5d80-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d5d80-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="d5d80-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5d80-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="d5d80-128">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="d5d80-128">Date and time the version was last modified.</span></span> <span data-ttu-id="d5d80-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5d80-129">Read-only.</span></span>                 |
| <span data-ttu-id="d5d80-130">**published**</span><span class="sxs-lookup"><span data-stu-id="d5d80-130">**published**</span></span>            | [<span data-ttu-id="d5d80-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="d5d80-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="d5d80-132">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="d5d80-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="d5d80-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5d80-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="d5d80-134">Связи</span><span class="sxs-lookup"><span data-stu-id="d5d80-134">Relationships</span></span>

<span data-ttu-id="d5d80-135">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="d5d80-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="d5d80-136">Имя связи</span><span class="sxs-lookup"><span data-stu-id="d5d80-136">Relationship name</span></span> |                      <span data-ttu-id="d5d80-137">Тип</span><span class="sxs-lookup"><span data-stu-id="d5d80-137">Type</span></span>                      |                               <span data-ttu-id="d5d80-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d5d80-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="d5d80-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="d5d80-139">**fields**</span></span>        | [<span data-ttu-id="d5d80-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="d5d80-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="d5d80-141">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="d5d80-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->

