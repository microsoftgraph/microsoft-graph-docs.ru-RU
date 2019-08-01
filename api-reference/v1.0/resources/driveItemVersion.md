---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенную версию DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: resourcePageType
ms.openlocfilehash: e9521eb549bf84b900e6c49c4dedc5f2199de317
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029402"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="6b14c-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="6b14c-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="6b14c-104">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6b14c-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="6b14c-105">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="6b14c-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="6b14c-106">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="6b14c-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="6b14c-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="6b14c-107">Common task</span></span>             |         <span data-ttu-id="6b14c-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="6b14c-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="6b14c-109">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="6b14c-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="6b14c-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="6b14c-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="6b14c-111">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="6b14c-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="6b14c-112">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="6b14c-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="6b14c-113">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="6b14c-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b14c-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6b14c-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6b14c-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b14c-115">Properties</span></span>

|      <span data-ttu-id="6b14c-116">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6b14c-116">Property name</span></span>       |                         <span data-ttu-id="6b14c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="6b14c-117">Type</span></span>                         |                               <span data-ttu-id="6b14c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="6b14c-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="6b14c-119">**id**</span><span class="sxs-lookup"><span data-stu-id="6b14c-119">**id**</span></span>                   | <span data-ttu-id="6b14c-120">string</span><span class="sxs-lookup"><span data-stu-id="6b14c-120">string</span></span>                                               | <span data-ttu-id="6b14c-121">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="6b14c-121">The ID of the version.</span></span> <span data-ttu-id="6b14c-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b14c-122">Read-only.</span></span>                                       |
| <span data-ttu-id="6b14c-123">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="6b14c-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="6b14c-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6b14c-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="6b14c-125">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="6b14c-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="6b14c-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b14c-126">Read-only.</span></span>        |
| <span data-ttu-id="6b14c-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6b14c-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="6b14c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b14c-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="6b14c-129">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="6b14c-129">Date and time the version was last modified.</span></span> <span data-ttu-id="6b14c-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b14c-130">Read-only.</span></span>                 |
| <span data-ttu-id="6b14c-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="6b14c-131">**publication**</span></span>          | [<span data-ttu-id="6b14c-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="6b14c-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="6b14c-133">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="6b14c-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="6b14c-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b14c-134">Read-only.</span></span> |
| <span data-ttu-id="6b14c-135">**size**</span><span class="sxs-lookup"><span data-stu-id="6b14c-135">**size**</span></span>                 | <span data-ttu-id="6b14c-136">Int64</span><span class="sxs-lookup"><span data-stu-id="6b14c-136">Int64</span></span>                                                | <span data-ttu-id="6b14c-137">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="6b14c-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="6b14c-138">**content**</span><span class="sxs-lookup"><span data-stu-id="6b14c-138">**content**</span></span>              | <span data-ttu-id="6b14c-139">Stream</span><span class="sxs-lookup"><span data-stu-id="6b14c-139">Stream</span></span>                                               | <span data-ttu-id="6b14c-140">Поток содержимого для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="6b14c-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
