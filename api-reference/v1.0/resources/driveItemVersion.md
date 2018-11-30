---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенной версии DriveItem.
ms.openlocfilehash: e257e800b0ac8ad4d94027f9c8040ffb3b20ea90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026043"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="704b6-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="704b6-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="704b6-104">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="704b6-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="704b6-105">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="704b6-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="704b6-106">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="704b6-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="704b6-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="704b6-107">Common task</span></span>             |         <span data-ttu-id="704b6-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="704b6-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="704b6-109">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="704b6-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="704b6-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="704b6-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="704b6-111">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="704b6-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="704b6-112">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="704b6-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="704b6-113">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="704b6-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="704b6-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="704b6-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="704b6-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="704b6-115">Properties</span></span>

|      <span data-ttu-id="704b6-116">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="704b6-116">Property name</span></span>       |                         <span data-ttu-id="704b6-117">Тип</span><span class="sxs-lookup"><span data-stu-id="704b6-117">Type</span></span>                         |                               <span data-ttu-id="704b6-118">Описание</span><span class="sxs-lookup"><span data-stu-id="704b6-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="704b6-119">**id**</span><span class="sxs-lookup"><span data-stu-id="704b6-119">**id**</span></span>                   | <span data-ttu-id="704b6-120">строка</span><span class="sxs-lookup"><span data-stu-id="704b6-120">string</span></span>                                               | <span data-ttu-id="704b6-121">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="704b6-121">The ID of the version.</span></span> <span data-ttu-id="704b6-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="704b6-122">Read-only.</span></span>                                       |
| <span data-ttu-id="704b6-123">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="704b6-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="704b6-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="704b6-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="704b6-125">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="704b6-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="704b6-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="704b6-126">Read-only.</span></span>        |
| <span data-ttu-id="704b6-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="704b6-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="704b6-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="704b6-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="704b6-129">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="704b6-129">Date and time the version was last modified.</span></span> <span data-ttu-id="704b6-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="704b6-130">Read-only.</span></span>                 |
| <span data-ttu-id="704b6-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="704b6-131">**publication**</span></span>          | [<span data-ttu-id="704b6-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="704b6-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="704b6-133">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="704b6-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="704b6-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="704b6-134">Read-only.</span></span> |
| <span data-ttu-id="704b6-135">**size**</span><span class="sxs-lookup"><span data-stu-id="704b6-135">**size**</span></span>                 | <span data-ttu-id="704b6-136">Int64</span><span class="sxs-lookup"><span data-stu-id="704b6-136">Int64</span></span>                                                | <span data-ttu-id="704b6-137">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="704b6-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="704b6-138">**content**</span><span class="sxs-lookup"><span data-stu-id="704b6-138">**content**</span></span>              | <span data-ttu-id="704b6-139">Stream</span><span class="sxs-lookup"><span data-stu-id="704b6-139">Stream</span></span>                                               | <span data-ttu-id="704b6-140">Поток содержимого для данной версии элемента.</span><span class="sxs-lookup"><span data-stu-id="704b6-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
