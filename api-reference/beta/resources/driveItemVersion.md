---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: DriveItemVersion
ms.openlocfilehash: 6abe10a14a4995231b12cf0c828325259775ffd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075538"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="7d9d1-102">Тип ресурса DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="7d9d1-102">DriveItemVersion resource type</span></span>

> <span data-ttu-id="7d9d1-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d9d1-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d9d1-105">Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7d9d1-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="7d9d1-106">Задачи, которые можно выполнить для ресурсов DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="7d9d1-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="7d9d1-107">Ниже перечислены задачи, доступные для ресурсов driveItemVersion.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="7d9d1-108">Стандартная задача</span><span class="sxs-lookup"><span data-stu-id="7d9d1-108">Common task</span></span>             |         <span data-ttu-id="7d9d1-109">Метод HTTP</span><span class="sxs-lookup"><span data-stu-id="7d9d1-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="7d9d1-110">[List versions][version-list]</span><span class="sxs-lookup"><span data-stu-id="7d9d1-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="7d9d1-111">[Get version][version-get]</span><span class="sxs-lookup"><span data-stu-id="7d9d1-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="7d9d1-112">[Get contents][content-get]</span><span class="sxs-lookup"><span data-stu-id="7d9d1-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="7d9d1-113">[Restore version][version-restore]</span><span class="sxs-lookup"><span data-stu-id="7d9d1-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="7d9d1-114">В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d9d1-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7d9d1-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7d9d1-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d9d1-116">Properties</span></span>

|      <span data-ttu-id="7d9d1-117">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7d9d1-117">Property name</span></span>       |                         <span data-ttu-id="7d9d1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7d9d1-118">Type</span></span>                         |                               <span data-ttu-id="7d9d1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7d9d1-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="7d9d1-120">**id**</span><span class="sxs-lookup"><span data-stu-id="7d9d1-120">**id**</span></span>                   | <span data-ttu-id="7d9d1-121">строка</span><span class="sxs-lookup"><span data-stu-id="7d9d1-121">string</span></span>                                               | <span data-ttu-id="7d9d1-122">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-122">The ID of the version.</span></span> <span data-ttu-id="7d9d1-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-123">Read-only.</span></span>                                       |
| <span data-ttu-id="7d9d1-124">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="7d9d1-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="7d9d1-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="7d9d1-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="7d9d1-126">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="7d9d1-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-127">Read-only.</span></span>        |
| <span data-ttu-id="7d9d1-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="7d9d1-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="7d9d1-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d9d1-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="7d9d1-130">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-130">Date and time the version was last modified.</span></span> <span data-ttu-id="7d9d1-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-131">Read-only.</span></span>                 |
| <span data-ttu-id="7d9d1-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="7d9d1-132">**publication**</span></span>          | [<span data-ttu-id="7d9d1-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="7d9d1-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="7d9d1-134">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="7d9d1-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-135">Read-only.</span></span> |
| <span data-ttu-id="7d9d1-136">**size**</span><span class="sxs-lookup"><span data-stu-id="7d9d1-136">**size**</span></span>                 | <span data-ttu-id="7d9d1-137">Int64</span><span class="sxs-lookup"><span data-stu-id="7d9d1-137">Int64</span></span>                                                | <span data-ttu-id="7d9d1-138">Указывает размер потока контента для этой версии элемента.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-138">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="7d9d1-139">Связи</span><span class="sxs-lookup"><span data-stu-id="7d9d1-139">Relationships</span></span>

<span data-ttu-id="7d9d1-140">В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-140">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="7d9d1-141">Имя связи</span><span class="sxs-lookup"><span data-stu-id="7d9d1-141">Relationship name</span></span> |  <span data-ttu-id="7d9d1-142">Тип</span><span class="sxs-lookup"><span data-stu-id="7d9d1-142">Type</span></span>  |            <span data-ttu-id="7d9d1-143">Описание</span><span class="sxs-lookup"><span data-stu-id="7d9d1-143">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="7d9d1-144">**content**</span><span class="sxs-lookup"><span data-stu-id="7d9d1-144">**content**</span></span>       | <span data-ttu-id="7d9d1-145">Stream</span><span class="sxs-lookup"><span data-stu-id="7d9d1-145">Stream</span></span> | <span data-ttu-id="7d9d1-146">Поток контента версии.</span><span class="sxs-lookup"><span data-stu-id="7d9d1-146">The content stream of the version.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->