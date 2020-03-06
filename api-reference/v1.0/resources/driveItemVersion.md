---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенную версию DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: resourcePageType
ms.openlocfilehash: b0ca825a0cd920ba10575ad2cd826da7e0b64055
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531558"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="f21fa-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="f21fa-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="f21fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f21fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f21fa-105">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f21fa-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="f21fa-106">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="f21fa-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="f21fa-107">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="f21fa-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="f21fa-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="f21fa-108">Common task</span></span>             |         <span data-ttu-id="f21fa-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="f21fa-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="f21fa-110">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="f21fa-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="f21fa-111">[Получение версии][version-get]</span><span class="sxs-lookup"><span data-stu-id="f21fa-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="f21fa-112">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="f21fa-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="f21fa-113">[Восстановление версии][version-restore]</span><span class="sxs-lookup"><span data-stu-id="f21fa-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="f21fa-114">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="f21fa-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f21fa-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f21fa-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f21fa-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="f21fa-116">Properties</span></span>

|      <span data-ttu-id="f21fa-117">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f21fa-117">Property name</span></span>       |                         <span data-ttu-id="f21fa-118">Тип</span><span class="sxs-lookup"><span data-stu-id="f21fa-118">Type</span></span>                         |                               <span data-ttu-id="f21fa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f21fa-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="f21fa-120">**id**</span><span class="sxs-lookup"><span data-stu-id="f21fa-120">**id**</span></span>                   | <span data-ttu-id="f21fa-121">string</span><span class="sxs-lookup"><span data-stu-id="f21fa-121">string</span></span>                                               | <span data-ttu-id="f21fa-122">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="f21fa-122">The ID of the version.</span></span> <span data-ttu-id="f21fa-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f21fa-123">Read-only.</span></span>                                       |
| <span data-ttu-id="f21fa-124">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="f21fa-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="f21fa-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f21fa-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="f21fa-126">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="f21fa-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="f21fa-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f21fa-127">Read-only.</span></span>        |
| <span data-ttu-id="f21fa-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f21fa-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="f21fa-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f21fa-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="f21fa-130">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="f21fa-130">Date and time the version was last modified.</span></span> <span data-ttu-id="f21fa-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f21fa-131">Read-only.</span></span>                 |
| <span data-ttu-id="f21fa-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="f21fa-132">**publication**</span></span>          | [<span data-ttu-id="f21fa-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="f21fa-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="f21fa-134">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="f21fa-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="f21fa-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f21fa-135">Read-only.</span></span> |
| <span data-ttu-id="f21fa-136">**size**</span><span class="sxs-lookup"><span data-stu-id="f21fa-136">**size**</span></span>                 | <span data-ttu-id="f21fa-137">Int64</span><span class="sxs-lookup"><span data-stu-id="f21fa-137">Int64</span></span>                                                | <span data-ttu-id="f21fa-138">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="f21fa-138">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="f21fa-139">**content**</span><span class="sxs-lookup"><span data-stu-id="f21fa-139">**content**</span></span>              | <span data-ttu-id="f21fa-140">Stream</span><span class="sxs-lookup"><span data-stu-id="f21fa-140">Stream</span></span>                                               | <span data-ttu-id="f21fa-141">Поток содержимого для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="f21fa-141">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
