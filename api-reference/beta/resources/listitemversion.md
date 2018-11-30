---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: ListItemVersion
ms.openlocfilehash: 7cda16159c6e5e58a0f60aef3c60198c7615f9e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074894"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="fc828-102">Тип ресурса listItemVersion</span><span class="sxs-lookup"><span data-stu-id="fc828-102">ListItemVersion resource type</span></span>

> <span data-ttu-id="fc828-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc828-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc828-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc828-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc828-105">Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="fc828-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="fc828-106">Задачи, которые можно выполнить для ресурсов listItemVersion</span><span class="sxs-lookup"><span data-stu-id="fc828-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="fc828-107">Ниже перечислены задачи, доступные для ресурсов listItemVersion.</span><span class="sxs-lookup"><span data-stu-id="fc828-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="fc828-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="fc828-108">Common task</span></span>             |         <span data-ttu-id="fc828-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="fc828-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="fc828-110">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="fc828-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="fc828-111">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="fc828-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="fc828-112">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="fc828-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="fc828-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc828-113">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fc828-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc828-114">Properties</span></span>

|      <span data-ttu-id="fc828-115">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="fc828-115">Property name</span></span>       |                         <span data-ttu-id="fc828-116">Тип</span><span class="sxs-lookup"><span data-stu-id="fc828-116">Type</span></span>                         |                               <span data-ttu-id="fc828-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fc828-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="fc828-118">**id**</span><span class="sxs-lookup"><span data-stu-id="fc828-118">**id**</span></span>                   | <span data-ttu-id="fc828-119">строка</span><span class="sxs-lookup"><span data-stu-id="fc828-119">string</span></span>                                               | <span data-ttu-id="fc828-120">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="fc828-120">The ID of the version.</span></span> <span data-ttu-id="fc828-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc828-121">Read-only.</span></span>                                       |
| <span data-ttu-id="fc828-122">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="fc828-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="fc828-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fc828-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="fc828-124">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="fc828-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="fc828-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc828-125">Read-only.</span></span>        |
| <span data-ttu-id="fc828-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="fc828-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="fc828-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc828-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="fc828-128">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="fc828-128">Date and time the version was last modified.</span></span> <span data-ttu-id="fc828-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc828-129">Read-only.</span></span>                 |
| <span data-ttu-id="fc828-130">**published**</span><span class="sxs-lookup"><span data-stu-id="fc828-130">**published**</span></span>            | [<span data-ttu-id="fc828-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="fc828-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="fc828-132">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="fc828-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="fc828-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc828-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="fc828-134">Связи</span><span class="sxs-lookup"><span data-stu-id="fc828-134">Relationships</span></span>

<span data-ttu-id="fc828-135">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="fc828-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="fc828-136">Имя связи</span><span class="sxs-lookup"><span data-stu-id="fc828-136">Relationship name</span></span> |                      <span data-ttu-id="fc828-137">Тип</span><span class="sxs-lookup"><span data-stu-id="fc828-137">Type</span></span>                      |                               <span data-ttu-id="fc828-138">Описание</span><span class="sxs-lookup"><span data-stu-id="fc828-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="fc828-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="fc828-139">**fields**</span></span>        | [<span data-ttu-id="fc828-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="fc828-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="fc828-141">Коллекция полей и значений для этой версии элемента списка.</span><span class="sxs-lookup"><span data-stu-id="fc828-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->