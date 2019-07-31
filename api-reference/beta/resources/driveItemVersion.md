---
author: JeremyKelley
description: Ресурс DriveItemVersion представляет определенную версию элемента DriveItem.
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e3886c27ded6b26082609933d5ac7382dc182b45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973094"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="7ff00-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="7ff00-103">DriveItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ff00-104">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7ff00-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="7ff00-105">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="7ff00-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="7ff00-106">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="7ff00-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="7ff00-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="7ff00-107">Common task</span></span>             |         <span data-ttu-id="7ff00-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="7ff00-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="7ff00-109">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="7ff00-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="7ff00-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="7ff00-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="7ff00-111">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="7ff00-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="7ff00-112">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="7ff00-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="7ff00-113">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="7ff00-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ff00-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7ff00-114">JSON representation</span></span>

<!-- { "blockType": "resource","keyProperty":"id", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": {"@odata.type": "Edm.Stream"},
  "id": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="7ff00-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ff00-115">Properties</span></span>

|      <span data-ttu-id="7ff00-116">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7ff00-116">Property name</span></span>       |                         <span data-ttu-id="7ff00-117">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff00-117">Type</span></span>                         |                               <span data-ttu-id="7ff00-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff00-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="7ff00-119">**id**</span><span class="sxs-lookup"><span data-stu-id="7ff00-119">**id**</span></span>                   | <span data-ttu-id="7ff00-120">string</span><span class="sxs-lookup"><span data-stu-id="7ff00-120">string</span></span>                                               | <span data-ttu-id="7ff00-121">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="7ff00-121">The ID of the version.</span></span> <span data-ttu-id="7ff00-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ff00-122">Read-only.</span></span>                                       |
| <span data-ttu-id="7ff00-123">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="7ff00-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="7ff00-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="7ff00-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="7ff00-125">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="7ff00-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="7ff00-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ff00-126">Read-only.</span></span>        |
| <span data-ttu-id="7ff00-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="7ff00-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="7ff00-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ff00-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="7ff00-129">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="7ff00-129">Date and time the version was last modified.</span></span> <span data-ttu-id="7ff00-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ff00-130">Read-only.</span></span>                 |
| <span data-ttu-id="7ff00-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="7ff00-131">**publication**</span></span>          | [<span data-ttu-id="7ff00-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="7ff00-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="7ff00-133">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="7ff00-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="7ff00-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ff00-134">Read-only.</span></span> |
| <span data-ttu-id="7ff00-135">**size**</span><span class="sxs-lookup"><span data-stu-id="7ff00-135">**size**</span></span>                 | <span data-ttu-id="7ff00-136">Int64</span><span class="sxs-lookup"><span data-stu-id="7ff00-136">Int64</span></span>                                                | <span data-ttu-id="7ff00-137">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="7ff00-137">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="7ff00-138">Связи</span><span class="sxs-lookup"><span data-stu-id="7ff00-138">Relationships</span></span>

<span data-ttu-id="7ff00-139">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="7ff00-139">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="7ff00-140">Имя связи</span><span class="sxs-lookup"><span data-stu-id="7ff00-140">Relationship name</span></span> |  <span data-ttu-id="7ff00-141">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff00-141">Type</span></span>  |            <span data-ttu-id="7ff00-142">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff00-142">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="7ff00-143">**content**</span><span class="sxs-lookup"><span data-stu-id="7ff00-143">**content**</span></span>       | <span data-ttu-id="7ff00-144">Stream</span><span class="sxs-lookup"><span data-stu-id="7ff00-144">Stream</span></span> | <span data-ttu-id="7ff00-145">Поток контента версии.</span><span class="sxs-lookup"><span data-stu-id="7ff00-145">The content stream of the version.</span></span> |

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
