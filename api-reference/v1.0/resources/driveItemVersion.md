---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенной версии DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fd6052464d40fcce86b83d93601282dda252c69b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643988"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="af5fb-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="af5fb-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="af5fb-104">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="af5fb-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="af5fb-105">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="af5fb-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="af5fb-106">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="af5fb-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="af5fb-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="af5fb-107">Common task</span></span>             |         <span data-ttu-id="af5fb-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="af5fb-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="af5fb-109">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="af5fb-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="af5fb-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="af5fb-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="af5fb-111">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="af5fb-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="af5fb-112">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="af5fb-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="af5fb-113">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="af5fb-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af5fb-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="af5fb-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="af5fb-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="af5fb-115">Properties</span></span>

|      <span data-ttu-id="af5fb-116">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="af5fb-116">Property name</span></span>       |                         <span data-ttu-id="af5fb-117">Тип</span><span class="sxs-lookup"><span data-stu-id="af5fb-117">Type</span></span>                         |                               <span data-ttu-id="af5fb-118">Описание</span><span class="sxs-lookup"><span data-stu-id="af5fb-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="af5fb-119">**id**</span><span class="sxs-lookup"><span data-stu-id="af5fb-119">**id**</span></span>                   | <span data-ttu-id="af5fb-120">строка</span><span class="sxs-lookup"><span data-stu-id="af5fb-120">string</span></span>                                               | <span data-ttu-id="af5fb-121">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="af5fb-121">The ID of the version.</span></span> <span data-ttu-id="af5fb-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af5fb-122">Read-only.</span></span>                                       |
| <span data-ttu-id="af5fb-123">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="af5fb-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="af5fb-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="af5fb-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="af5fb-125">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="af5fb-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="af5fb-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af5fb-126">Read-only.</span></span>        |
| <span data-ttu-id="af5fb-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="af5fb-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="af5fb-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af5fb-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="af5fb-129">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="af5fb-129">Date and time the version was last modified.</span></span> <span data-ttu-id="af5fb-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af5fb-130">Read-only.</span></span>                 |
| <span data-ttu-id="af5fb-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="af5fb-131">**publication**</span></span>          | [<span data-ttu-id="af5fb-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="af5fb-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="af5fb-133">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="af5fb-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="af5fb-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af5fb-134">Read-only.</span></span> |
| <span data-ttu-id="af5fb-135">**size**</span><span class="sxs-lookup"><span data-stu-id="af5fb-135">**size**</span></span>                 | <span data-ttu-id="af5fb-136">Int64</span><span class="sxs-lookup"><span data-stu-id="af5fb-136">Int64</span></span>                                                | <span data-ttu-id="af5fb-137">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="af5fb-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="af5fb-138">**content**</span><span class="sxs-lookup"><span data-stu-id="af5fb-138">**content**</span></span>              | <span data-ttu-id="af5fb-139">Stream</span><span class="sxs-lookup"><span data-stu-id="af5fb-139">Stream</span></span>                                               | <span data-ttu-id="af5fb-140">Поток содержимого для данной версии элемента.</span><span class="sxs-lookup"><span data-stu-id="af5fb-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
