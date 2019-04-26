---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенную версию DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fd6052464d40fcce86b83d93601282dda252c69b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562687"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="06c91-103">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="06c91-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="06c91-104">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="06c91-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="06c91-105">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="06c91-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="06c91-106">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="06c91-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="06c91-107">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="06c91-107">Common task</span></span>             |         <span data-ttu-id="06c91-108">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="06c91-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="06c91-109">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="06c91-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="06c91-110">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="06c91-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="06c91-111">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="06c91-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="06c91-112">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="06c91-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="06c91-113">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="06c91-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="06c91-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="06c91-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="06c91-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="06c91-115">Properties</span></span>

|      <span data-ttu-id="06c91-116">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="06c91-116">Property name</span></span>       |                         <span data-ttu-id="06c91-117">Тип</span><span class="sxs-lookup"><span data-stu-id="06c91-117">Type</span></span>                         |                               <span data-ttu-id="06c91-118">Описание</span><span class="sxs-lookup"><span data-stu-id="06c91-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="06c91-119">**id**</span><span class="sxs-lookup"><span data-stu-id="06c91-119">**id**</span></span>                   | <span data-ttu-id="06c91-120">string</span><span class="sxs-lookup"><span data-stu-id="06c91-120">string</span></span>                                               | <span data-ttu-id="06c91-121">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="06c91-121">The ID of the version.</span></span> <span data-ttu-id="06c91-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="06c91-122">Read-only.</span></span>                                       |
| <span data-ttu-id="06c91-123">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="06c91-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="06c91-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="06c91-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="06c91-125">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="06c91-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="06c91-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="06c91-126">Read-only.</span></span>        |
| <span data-ttu-id="06c91-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="06c91-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="06c91-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06c91-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="06c91-129">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="06c91-129">Date and time the version was last modified.</span></span> <span data-ttu-id="06c91-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="06c91-130">Read-only.</span></span>                 |
| <span data-ttu-id="06c91-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="06c91-131">**publication**</span></span>          | [<span data-ttu-id="06c91-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="06c91-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="06c91-133">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="06c91-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="06c91-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="06c91-134">Read-only.</span></span> |
| <span data-ttu-id="06c91-135">**size**</span><span class="sxs-lookup"><span data-stu-id="06c91-135">**size**</span></span>                 | <span data-ttu-id="06c91-136">Int64</span><span class="sxs-lookup"><span data-stu-id="06c91-136">Int64</span></span>                                                | <span data-ttu-id="06c91-137">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="06c91-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="06c91-138">**content**</span><span class="sxs-lookup"><span data-stu-id="06c91-138">**content**</span></span>              | <span data-ttu-id="06c91-139">Stream</span><span class="sxs-lookup"><span data-stu-id="06c91-139">Stream</span></span>                                               | <span data-ttu-id="06c91-140">Поток содержимого для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="06c91-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
