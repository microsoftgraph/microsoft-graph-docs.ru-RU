---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
ms.openlocfilehash: 31925f336dbb0ce0f83ffd6b36b38e7a0916cdb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303453"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="9ff5d-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="9ff5d-105">educationTerm resource type</span></span>

> <span data-ttu-id="9ff5d-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ff5d-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ff5d-108">Срок.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-108">A term.</span></span> <span data-ttu-id="9ff5d-109">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="9ff5d-110">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="9ff5d-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9ff5d-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ff5d-111">Properties</span></span>
| <span data-ttu-id="9ff5d-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ff5d-112">Property</span></span>     | <span data-ttu-id="9ff5d-113">Тип</span><span class="sxs-lookup"><span data-stu-id="9ff5d-113">Type</span></span>   |<span data-ttu-id="9ff5d-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9ff5d-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ff5d-115">displayName</span><span class="sxs-lookup"><span data-stu-id="9ff5d-115">displayName</span></span>| <span data-ttu-id="9ff5d-116">String</span><span class="sxs-lookup"><span data-stu-id="9ff5d-116">String</span></span>| <span data-ttu-id="9ff5d-117">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-117">Display name of the term.</span></span>| 
|<span data-ttu-id="9ff5d-118">externalId</span><span class="sxs-lookup"><span data-stu-id="9ff5d-118">externalId</span></span>|<span data-ttu-id="9ff5d-119">String</span><span class="sxs-lookup"><span data-stu-id="9ff5d-119">String</span></span>| <span data-ttu-id="9ff5d-120">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="9ff5d-121">startDate</span><span class="sxs-lookup"><span data-stu-id="9ff5d-121">startDate</span></span>|<span data-ttu-id="9ff5d-122">Date</span><span class="sxs-lookup"><span data-stu-id="9ff5d-122">Date</span></span>|<span data-ttu-id="9ff5d-123">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-123">Start of the term.</span></span>|
|<span data-ttu-id="9ff5d-124">endDate</span><span class="sxs-lookup"><span data-stu-id="9ff5d-124">endDate</span></span>|<span data-ttu-id="9ff5d-125">Date</span><span class="sxs-lookup"><span data-stu-id="9ff5d-125">Date</span></span>|<span data-ttu-id="9ff5d-126">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ff5d-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9ff5d-127">JSON representation</span></span>

<span data-ttu-id="9ff5d-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ff5d-128">The following is a JSON representation of the resource.</span></span>

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