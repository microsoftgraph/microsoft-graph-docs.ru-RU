---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: af11aa6b4a110417152c76dd606245a18ad51c28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851452"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="5a400-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="5a400-105">educationTerm resource type</span></span>

<span data-ttu-id="5a400-106">Срок.</span><span class="sxs-lookup"><span data-stu-id="5a400-106">A term.</span></span> <span data-ttu-id="5a400-107">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="5a400-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="5a400-108">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="5a400-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a400-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a400-109">Properties</span></span>
| <span data-ttu-id="5a400-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a400-110">Property</span></span>     | <span data-ttu-id="5a400-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5a400-111">Type</span></span>   |<span data-ttu-id="5a400-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5a400-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a400-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5a400-113">displayName</span></span>| <span data-ttu-id="5a400-114">String</span><span class="sxs-lookup"><span data-stu-id="5a400-114">String</span></span>| <span data-ttu-id="5a400-115">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="5a400-115">Display name of the term.</span></span>| 
|<span data-ttu-id="5a400-116">externalId</span><span class="sxs-lookup"><span data-stu-id="5a400-116">externalId</span></span>|<span data-ttu-id="5a400-117">String</span><span class="sxs-lookup"><span data-stu-id="5a400-117">String</span></span>| <span data-ttu-id="5a400-118">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5a400-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="5a400-119">startDate</span><span class="sxs-lookup"><span data-stu-id="5a400-119">startDate</span></span>|<span data-ttu-id="5a400-120">Date</span><span class="sxs-lookup"><span data-stu-id="5a400-120">Date</span></span>|<span data-ttu-id="5a400-121">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="5a400-121">Start of the term.</span></span>|
|<span data-ttu-id="5a400-122">endDate</span><span class="sxs-lookup"><span data-stu-id="5a400-122">endDate</span></span>|<span data-ttu-id="5a400-123">Date</span><span class="sxs-lookup"><span data-stu-id="5a400-123">Date</span></span>|<span data-ttu-id="5a400-124">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="5a400-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a400-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5a400-125">JSON representation</span></span>

<span data-ttu-id="5a400-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a400-126">The following is a JSON representation of the resource.</span></span>

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
