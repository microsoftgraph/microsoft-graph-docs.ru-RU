---
title: Тип ресурса baseItemVersion
description: Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 03b18712e62a37e546fb8f9e3d031eeedace0208
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033070"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="cb1ee-103">Тип ресурса baseItemVersion</span><span class="sxs-lookup"><span data-stu-id="cb1ee-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="cb1ee-104">Ресурс **baseItemVersion** представляет предыдущую версию элемента или записи.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="cb1ee-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cb1ee-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cb1ee-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb1ee-106">Properties</span></span>

|      <span data-ttu-id="cb1ee-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="cb1ee-107">Property name</span></span>       |                         <span data-ttu-id="cb1ee-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cb1ee-108">Type</span></span>                         |                               <span data-ttu-id="cb1ee-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cb1ee-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="cb1ee-110">**id**</span><span class="sxs-lookup"><span data-stu-id="cb1ee-110">**id**</span></span>                   | <span data-ttu-id="cb1ee-111">string</span><span class="sxs-lookup"><span data-stu-id="cb1ee-111">string</span></span>                                               | <span data-ttu-id="cb1ee-112">Идентификатор версии.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-112">The ID of the version.</span></span> <span data-ttu-id="cb1ee-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-113">Read-only.</span></span>                                       |
| <span data-ttu-id="cb1ee-114">**lastModifiedBy**;</span><span class="sxs-lookup"><span data-stu-id="cb1ee-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="cb1ee-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="cb1ee-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="cb1ee-116">Удостоверение пользователя, который последним изменил версию.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="cb1ee-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-117">Read-only.</span></span>        |
| <span data-ttu-id="cb1ee-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="cb1ee-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="cb1ee-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb1ee-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="cb1ee-120">Дата и время последнего изменения версии.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-120">Date and time the version was last modified.</span></span> <span data-ttu-id="cb1ee-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-121">Read-only.</span></span>                 |
| <span data-ttu-id="cb1ee-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="cb1ee-122">**publication**</span></span>          | [<span data-ttu-id="cb1ee-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="cb1ee-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="cb1ee-124">Указывает состояние публикации конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="cb1ee-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb1ee-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
