---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3be7cd044b65eccd2370a2848258b415c5e70b00
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482366"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="c0194-102">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="c0194-102">DriveItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0194-103">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c0194-103">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="c0194-104">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="c0194-104">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="c0194-105">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="c0194-105">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="c0194-106">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="c0194-106">Common task</span></span>             |         <span data-ttu-id="c0194-107">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="c0194-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="c0194-108">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="c0194-108">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="c0194-109">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="c0194-109">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="c0194-110">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="c0194-110">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="c0194-111">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="c0194-111">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="c0194-112">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="c0194-112">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0194-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c0194-113">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="c0194-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0194-114">Properties</span></span>

|      <span data-ttu-id="c0194-115">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c0194-115">Property name</span></span>       |                         <span data-ttu-id="c0194-116">Тип</span><span class="sxs-lookup"><span data-stu-id="c0194-116">Type</span></span>                         |                               <span data-ttu-id="c0194-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c0194-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="c0194-118">**id**</span><span class="sxs-lookup"><span data-stu-id="c0194-118">**id**</span></span>                   | <span data-ttu-id="c0194-119">string</span><span class="sxs-lookup"><span data-stu-id="c0194-119">string</span></span>                                               | <span data-ttu-id="c0194-120">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="c0194-120">The ID of the version.</span></span> <span data-ttu-id="c0194-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0194-121">Read-only.</span></span>                                       |
| <span data-ttu-id="c0194-122">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="c0194-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="c0194-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c0194-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="c0194-124">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="c0194-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="c0194-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0194-125">Read-only.</span></span>        |
| <span data-ttu-id="c0194-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c0194-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="c0194-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0194-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="c0194-128">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="c0194-128">Date and time the version was last modified.</span></span> <span data-ttu-id="c0194-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0194-129">Read-only.</span></span>                 |
| <span data-ttu-id="c0194-130">**publication**</span><span class="sxs-lookup"><span data-stu-id="c0194-130">**publication**</span></span>          | [<span data-ttu-id="c0194-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="c0194-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="c0194-132">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="c0194-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="c0194-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0194-133">Read-only.</span></span> |
| <span data-ttu-id="c0194-134">**size**</span><span class="sxs-lookup"><span data-stu-id="c0194-134">**size**</span></span>                 | <span data-ttu-id="c0194-135">Int64</span><span class="sxs-lookup"><span data-stu-id="c0194-135">Int64</span></span>                                                | <span data-ttu-id="c0194-136">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="c0194-136">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="c0194-137">Связи</span><span class="sxs-lookup"><span data-stu-id="c0194-137">Relationships</span></span>

<span data-ttu-id="c0194-138">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="c0194-138">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="c0194-139">Имя связи</span><span class="sxs-lookup"><span data-stu-id="c0194-139">Relationship name</span></span> |  <span data-ttu-id="c0194-140">Тип</span><span class="sxs-lookup"><span data-stu-id="c0194-140">Type</span></span>  |            <span data-ttu-id="c0194-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c0194-141">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="c0194-142">**content**</span><span class="sxs-lookup"><span data-stu-id="c0194-142">**content**</span></span>       | <span data-ttu-id="c0194-143">Stream</span><span class="sxs-lookup"><span data-stu-id="c0194-143">Stream</span></span> | <span data-ttu-id="c0194-144">Поток контента версии.</span><span class="sxs-lookup"><span data-stu-id="c0194-144">The content stream of the version.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/driveItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
