---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
ms.openlocfilehash: 319eedbaebde4f1e76c2f1b3e124c0dad2642538
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353090"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="efe3d-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="efe3d-105">educationTerm resource type</span></span>

<span data-ttu-id="efe3d-106">Срок.</span><span class="sxs-lookup"><span data-stu-id="efe3d-106">A term.</span></span> <span data-ttu-id="efe3d-107">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="efe3d-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="efe3d-108">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="efe3d-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="efe3d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="efe3d-109">Properties</span></span>
| <span data-ttu-id="efe3d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="efe3d-110">Property</span></span>     | <span data-ttu-id="efe3d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="efe3d-111">Type</span></span>   |<span data-ttu-id="efe3d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="efe3d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efe3d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="efe3d-113">displayName</span></span>| <span data-ttu-id="efe3d-114">String</span><span class="sxs-lookup"><span data-stu-id="efe3d-114">String</span></span>| <span data-ttu-id="efe3d-115">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="efe3d-115">Display name of the term.</span></span>| 
|<span data-ttu-id="efe3d-116">externalId</span><span class="sxs-lookup"><span data-stu-id="efe3d-116">externalId</span></span>|<span data-ttu-id="efe3d-117">String</span><span class="sxs-lookup"><span data-stu-id="efe3d-117">String</span></span>| <span data-ttu-id="efe3d-118">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="efe3d-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="efe3d-119">startDate</span><span class="sxs-lookup"><span data-stu-id="efe3d-119">startDate</span></span>|<span data-ttu-id="efe3d-120">Date</span><span class="sxs-lookup"><span data-stu-id="efe3d-120">Date</span></span>|<span data-ttu-id="efe3d-121">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="efe3d-121">Start of the term.</span></span>|
|<span data-ttu-id="efe3d-122">endDate</span><span class="sxs-lookup"><span data-stu-id="efe3d-122">endDate</span></span>|<span data-ttu-id="efe3d-123">Date</span><span class="sxs-lookup"><span data-stu-id="efe3d-123">Date</span></span>|<span data-ttu-id="efe3d-124">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="efe3d-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efe3d-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="efe3d-125">JSON representation</span></span>

<span data-ttu-id="efe3d-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efe3d-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->