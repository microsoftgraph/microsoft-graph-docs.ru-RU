---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенную версию DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: a2b960fdde86909e0974fe49f21c9d787b95a0ae
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807845"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="0fc2b-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="0fc2b-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="0fc2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fc2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fc2b-105">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0fc2b-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="0fc2b-106">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="0fc2b-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="0fc2b-107">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="0fc2b-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="0fc2b-108">Common task</span></span>             |         <span data-ttu-id="0fc2b-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="0fc2b-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="0fc2b-110">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="0fc2b-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="0fc2b-111">[Получение версии][version-get]</span><span class="sxs-lookup"><span data-stu-id="0fc2b-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="0fc2b-112">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="0fc2b-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="0fc2b-113">[Восстановление версии][version-restore]</span><span class="sxs-lookup"><span data-stu-id="0fc2b-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="0fc2b-114">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fc2b-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0fc2b-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0fc2b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fc2b-116">Properties</span></span>

|      <span data-ttu-id="0fc2b-117">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0fc2b-117">Property name</span></span>       |                         <span data-ttu-id="0fc2b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="0fc2b-118">Type</span></span>                         |                               <span data-ttu-id="0fc2b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0fc2b-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="0fc2b-120">**id**</span><span class="sxs-lookup"><span data-stu-id="0fc2b-120">**id**</span></span>                   | <span data-ttu-id="0fc2b-121">string</span><span class="sxs-lookup"><span data-stu-id="0fc2b-121">string</span></span>                                               | <span data-ttu-id="0fc2b-122">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-122">The ID of the version.</span></span> <span data-ttu-id="0fc2b-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-123">Read-only.</span></span>                                       |
| <span data-ttu-id="0fc2b-124">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="0fc2b-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="0fc2b-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="0fc2b-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="0fc2b-126">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="0fc2b-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-127">Read-only.</span></span>        |
| <span data-ttu-id="0fc2b-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="0fc2b-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="0fc2b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc2b-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="0fc2b-130">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-130">Date and time the version was last modified.</span></span> <span data-ttu-id="0fc2b-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-131">Read-only.</span></span>                 |
| <span data-ttu-id="0fc2b-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="0fc2b-132">**publication**</span></span>          | [<span data-ttu-id="0fc2b-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="0fc2b-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="0fc2b-134">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="0fc2b-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-135">Read-only.</span></span> |
| <span data-ttu-id="0fc2b-136">**size**</span><span class="sxs-lookup"><span data-stu-id="0fc2b-136">**size**</span></span>                 | <span data-ttu-id="0fc2b-137">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc2b-137">Int64</span></span>                                                | <span data-ttu-id="0fc2b-138">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-138">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="0fc2b-139">**content**</span><span class="sxs-lookup"><span data-stu-id="0fc2b-139">**content**</span></span>              | <span data-ttu-id="0fc2b-140">Stream</span><span class="sxs-lookup"><span data-stu-id="0fc2b-140">Stream</span></span>                                               | <span data-ttu-id="0fc2b-141">Поток содержимого для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="0fc2b-141">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
