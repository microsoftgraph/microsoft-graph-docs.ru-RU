---
title: Тип ресурса listItemVersion
description: Ресурс **listItemVersion** представляет предыдущую версию ресурса ListItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 73b1c0e8f98a5f7ef321632e06619ba040cbd020
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807754"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="bf7ef-103">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="bf7ef-103">ListItemVersion resource type</span></span>

<span data-ttu-id="bf7ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf7ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf7ef-105">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="bf7ef-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="bf7ef-106">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="bf7ef-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="bf7ef-107">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="bf7ef-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="bf7ef-108">Common task</span></span>             |         <span data-ttu-id="bf7ef-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="bf7ef-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="bf7ef-110">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="bf7ef-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="bf7ef-111">[Получение версии][version-get]</span><span class="sxs-lookup"><span data-stu-id="bf7ef-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="bf7ef-112">[Восстановление версии][version-restore]</span><span class="sxs-lookup"><span data-stu-id="bf7ef-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="bf7ef-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf7ef-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bf7ef-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf7ef-114">Properties</span></span>

|      <span data-ttu-id="bf7ef-115">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="bf7ef-115">Property name</span></span>       |                         <span data-ttu-id="bf7ef-116">Тип</span><span class="sxs-lookup"><span data-stu-id="bf7ef-116">Type</span></span>                         |                               <span data-ttu-id="bf7ef-117">Описание</span><span class="sxs-lookup"><span data-stu-id="bf7ef-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="bf7ef-118">**id**</span><span class="sxs-lookup"><span data-stu-id="bf7ef-118">**id**</span></span>                   | <span data-ttu-id="bf7ef-119">string</span><span class="sxs-lookup"><span data-stu-id="bf7ef-119">string</span></span>                                               | <span data-ttu-id="bf7ef-120">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-120">The ID of the version.</span></span> <span data-ttu-id="bf7ef-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-121">Read-only.</span></span>                                       |
| <span data-ttu-id="bf7ef-122">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="bf7ef-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="bf7ef-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="bf7ef-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="bf7ef-124">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="bf7ef-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-125">Read-only.</span></span>        |
| <span data-ttu-id="bf7ef-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="bf7ef-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="bf7ef-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf7ef-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="bf7ef-128">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-128">Date and time the version was last modified.</span></span> <span data-ttu-id="bf7ef-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-129">Read-only.</span></span>                 |
| <span data-ttu-id="bf7ef-130">**published**</span><span class="sxs-lookup"><span data-stu-id="bf7ef-130">**published**</span></span>            | [<span data-ttu-id="bf7ef-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="bf7ef-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="bf7ef-132">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="bf7ef-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="bf7ef-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="bf7ef-134">Relationships</span></span>

<span data-ttu-id="bf7ef-135">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="bf7ef-136">Имя связи</span><span class="sxs-lookup"><span data-stu-id="bf7ef-136">Relationship name</span></span> |                      <span data-ttu-id="bf7ef-137">Тип</span><span class="sxs-lookup"><span data-stu-id="bf7ef-137">Type</span></span>                      |                               <span data-ttu-id="bf7ef-138">Описание</span><span class="sxs-lookup"><span data-stu-id="bf7ef-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="bf7ef-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="bf7ef-139">**fields**</span></span>        | [<span data-ttu-id="bf7ef-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="bf7ef-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="bf7ef-141">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="bf7ef-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
