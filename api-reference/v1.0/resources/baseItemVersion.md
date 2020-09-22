---
title: Тип ресурса baseItemVersion
description: Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a48059cf4341281336fb20e69ca4bfb53154ea8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032833"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="2df91-103">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="2df91-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="2df91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2df91-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2df91-105">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="2df91-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2df91-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2df91-106">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="2df91-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2df91-107">Properties</span></span>

|      <span data-ttu-id="2df91-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2df91-108">Property name</span></span>       |                         <span data-ttu-id="2df91-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2df91-109">Type</span></span>                         |                               <span data-ttu-id="2df91-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2df91-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="2df91-111">**id**</span><span class="sxs-lookup"><span data-stu-id="2df91-111">**id**</span></span>                   | <span data-ttu-id="2df91-112">string</span><span class="sxs-lookup"><span data-stu-id="2df91-112">string</span></span>                                               | <span data-ttu-id="2df91-113">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="2df91-113">The ID of the version.</span></span> <span data-ttu-id="2df91-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2df91-114">Read-only.</span></span>                                       |
| <span data-ttu-id="2df91-115">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="2df91-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="2df91-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="2df91-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="2df91-117">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="2df91-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="2df91-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2df91-118">Read-only.</span></span>        |
| <span data-ttu-id="2df91-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2df91-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="2df91-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df91-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="2df91-121">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="2df91-121">Date and time the version was last modified.</span></span> <span data-ttu-id="2df91-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2df91-122">Read-only.</span></span>                 |
| <span data-ttu-id="2df91-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="2df91-123">**publication**</span></span>          | [<span data-ttu-id="2df91-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="2df91-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="2df91-125">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="2df91-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="2df91-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2df91-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->

