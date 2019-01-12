---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенной версии DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5b6e9ecd2c3c8ec14958cfa2645f8fb0dbfe30e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949593"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="c32c4-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="c32c4-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="c32c4-104">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c32c4-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="c32c4-105">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="c32c4-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="c32c4-106">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="c32c4-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="c32c4-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="c32c4-107">Common task</span></span>             |         <span data-ttu-id="c32c4-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="c32c4-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="c32c4-109">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="c32c4-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="c32c4-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="c32c4-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="c32c4-111">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="c32c4-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="c32c4-112">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="c32c4-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="c32c4-113">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="c32c4-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c32c4-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c32c4-114">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="c32c4-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="c32c4-115">Properties</span></span>

|      <span data-ttu-id="c32c4-116">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c32c4-116">Property name</span></span>       |                         <span data-ttu-id="c32c4-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c32c4-117">Type</span></span>                         |                               <span data-ttu-id="c32c4-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c32c4-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="c32c4-119">**id**</span><span class="sxs-lookup"><span data-stu-id="c32c4-119">**id**</span></span>                   | <span data-ttu-id="c32c4-120">строка</span><span class="sxs-lookup"><span data-stu-id="c32c4-120">string</span></span>                                               | <span data-ttu-id="c32c4-121">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="c32c4-121">The ID of the version.</span></span> <span data-ttu-id="c32c4-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c32c4-122">Read-only.</span></span>                                       |
| <span data-ttu-id="c32c4-123">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="c32c4-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="c32c4-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c32c4-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="c32c4-125">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="c32c4-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="c32c4-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c32c4-126">Read-only.</span></span>        |
| <span data-ttu-id="c32c4-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c32c4-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="c32c4-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c32c4-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="c32c4-129">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="c32c4-129">Date and time the version was last modified.</span></span> <span data-ttu-id="c32c4-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c32c4-130">Read-only.</span></span>                 |
| <span data-ttu-id="c32c4-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="c32c4-131">**publication**</span></span>          | [<span data-ttu-id="c32c4-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="c32c4-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="c32c4-133">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="c32c4-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="c32c4-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c32c4-134">Read-only.</span></span> |
| <span data-ttu-id="c32c4-135">**size**</span><span class="sxs-lookup"><span data-stu-id="c32c4-135">**size**</span></span>                 | <span data-ttu-id="c32c4-136">Int64</span><span class="sxs-lookup"><span data-stu-id="c32c4-136">Int64</span></span>                                                | <span data-ttu-id="c32c4-137">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="c32c4-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="c32c4-138">**content**</span><span class="sxs-lookup"><span data-stu-id="c32c4-138">**content**</span></span>              | <span data-ttu-id="c32c4-139">Stream</span><span class="sxs-lookup"><span data-stu-id="c32c4-139">Stream</span></span>                                               | <span data-ttu-id="c32c4-140">Поток содержимого для данной версии элемента.</span><span class="sxs-lookup"><span data-stu-id="c32c4-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
