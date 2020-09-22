---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенную версию DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 1f7c45ecc82a209094748410614d6b25993e2aa7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018580"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="23572-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="23572-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="23572-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23572-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23572-105">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="23572-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="23572-106">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="23572-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="23572-107">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="23572-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="23572-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="23572-108">Common task</span></span>             |         <span data-ttu-id="23572-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="23572-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="23572-110">[Список версий][version-list]</span><span class="sxs-lookup"><span data-stu-id="23572-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="23572-111">[Получение версии][version-get]</span><span class="sxs-lookup"><span data-stu-id="23572-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="23572-112">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="23572-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="23572-113">[Восстановление версии][version-restore]</span><span class="sxs-lookup"><span data-stu-id="23572-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="23572-114">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="23572-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23572-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="23572-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="23572-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="23572-116">Properties</span></span>

|      <span data-ttu-id="23572-117">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="23572-117">Property name</span></span>       |                         <span data-ttu-id="23572-118">Тип</span><span class="sxs-lookup"><span data-stu-id="23572-118">Type</span></span>                         |                               <span data-ttu-id="23572-119">Описание</span><span class="sxs-lookup"><span data-stu-id="23572-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="23572-120">**id**</span><span class="sxs-lookup"><span data-stu-id="23572-120">**id**</span></span>                   | <span data-ttu-id="23572-121">string</span><span class="sxs-lookup"><span data-stu-id="23572-121">string</span></span>                                               | <span data-ttu-id="23572-122">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="23572-122">The ID of the version.</span></span> <span data-ttu-id="23572-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23572-123">Read-only.</span></span>                                       |
| <span data-ttu-id="23572-124">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="23572-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="23572-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="23572-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="23572-126">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="23572-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="23572-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23572-127">Read-only.</span></span>        |
| <span data-ttu-id="23572-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="23572-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="23572-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23572-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="23572-130">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="23572-130">Date and time the version was last modified.</span></span> <span data-ttu-id="23572-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23572-131">Read-only.</span></span>                 |
| <span data-ttu-id="23572-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="23572-132">**publication**</span></span>          | [<span data-ttu-id="23572-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="23572-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="23572-134">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="23572-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="23572-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23572-135">Read-only.</span></span> |
| <span data-ttu-id="23572-136">**size**</span><span class="sxs-lookup"><span data-stu-id="23572-136">**size**</span></span>                 | <span data-ttu-id="23572-137">Int64</span><span class="sxs-lookup"><span data-stu-id="23572-137">Int64</span></span>                                                | <span data-ttu-id="23572-138">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="23572-138">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="23572-139">**content**</span><span class="sxs-lookup"><span data-stu-id="23572-139">**content**</span></span>              | <span data-ttu-id="23572-140">Stream</span><span class="sxs-lookup"><span data-stu-id="23572-140">Stream</span></span>                                               | <span data-ttu-id="23572-141">Поток содержимого для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="23572-141">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->

