---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9c26565b552471fe2601d8e3cb629fd933d72937
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947584"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="fabc0-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="fabc0-105">educationTerm resource type</span></span>

<span data-ttu-id="fabc0-106">Срок.</span><span class="sxs-lookup"><span data-stu-id="fabc0-106">A term.</span></span> <span data-ttu-id="fabc0-107">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="fabc0-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="fabc0-108">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="fabc0-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fabc0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fabc0-109">Properties</span></span>
| <span data-ttu-id="fabc0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fabc0-110">Property</span></span>     | <span data-ttu-id="fabc0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fabc0-111">Type</span></span>   |<span data-ttu-id="fabc0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fabc0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fabc0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="fabc0-113">displayName</span></span>| <span data-ttu-id="fabc0-114">String</span><span class="sxs-lookup"><span data-stu-id="fabc0-114">String</span></span>| <span data-ttu-id="fabc0-115">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="fabc0-115">Display name of the term.</span></span>| 
|<span data-ttu-id="fabc0-116">externalId</span><span class="sxs-lookup"><span data-stu-id="fabc0-116">externalId</span></span>|<span data-ttu-id="fabc0-117">String</span><span class="sxs-lookup"><span data-stu-id="fabc0-117">String</span></span>| <span data-ttu-id="fabc0-118">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fabc0-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="fabc0-119">startDate</span><span class="sxs-lookup"><span data-stu-id="fabc0-119">startDate</span></span>|<span data-ttu-id="fabc0-120">Date</span><span class="sxs-lookup"><span data-stu-id="fabc0-120">Date</span></span>|<span data-ttu-id="fabc0-121">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="fabc0-121">Start of the term.</span></span>|
|<span data-ttu-id="fabc0-122">endDate</span><span class="sxs-lookup"><span data-stu-id="fabc0-122">endDate</span></span>|<span data-ttu-id="fabc0-123">Date</span><span class="sxs-lookup"><span data-stu-id="fabc0-123">Date</span></span>|<span data-ttu-id="fabc0-124">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="fabc0-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fabc0-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fabc0-125">JSON representation</span></span>

<span data-ttu-id="fabc0-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fabc0-126">The following is a JSON representation of the resource.</span></span>

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
