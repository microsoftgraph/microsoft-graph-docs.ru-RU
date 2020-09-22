---
author: JeremyKelley
description: Ресурс baseItemVersion представляет предыдущую версию элемента или записи.
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0d007d18f6329763fa6a7a426f1f944ef1fb4106
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089735"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="617e4-103">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="617e4-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="617e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="617e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="617e4-105">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="617e4-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="617e4-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="617e4-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="617e4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="617e4-107">Properties</span></span>

|      <span data-ttu-id="617e4-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="617e4-108">Property name</span></span>       |                         <span data-ttu-id="617e4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="617e4-109">Type</span></span>                         |                               <span data-ttu-id="617e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="617e4-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="617e4-111">**id**</span><span class="sxs-lookup"><span data-stu-id="617e4-111">**id**</span></span>                   | <span data-ttu-id="617e4-112">string</span><span class="sxs-lookup"><span data-stu-id="617e4-112">string</span></span>                                               | <span data-ttu-id="617e4-113">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="617e4-113">The ID of the version.</span></span> <span data-ttu-id="617e4-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="617e4-114">Read-only.</span></span>                                       |
| <span data-ttu-id="617e4-115">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="617e4-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="617e4-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="617e4-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="617e4-117">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="617e4-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="617e4-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="617e4-118">Read-only.</span></span>        |
| <span data-ttu-id="617e4-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="617e4-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="617e4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="617e4-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="617e4-121">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="617e4-121">Date and time the version was last modified.</span></span> <span data-ttu-id="617e4-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="617e4-122">Read-only.</span></span>                 |
| <span data-ttu-id="617e4-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="617e4-123">**publication**</span></span>          | [<span data-ttu-id="617e4-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="617e4-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="617e4-125">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="617e4-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="617e4-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="617e4-126">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->


