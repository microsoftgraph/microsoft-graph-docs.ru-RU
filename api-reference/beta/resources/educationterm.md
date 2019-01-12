---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bc068df7a31c1b3903e8735ba1255cc3a6f0ae73
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962760"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="c05c5-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="c05c5-105">educationTerm resource type</span></span>

> <span data-ttu-id="c05c5-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c05c5-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c05c5-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c05c5-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c05c5-108">Срок.</span><span class="sxs-lookup"><span data-stu-id="c05c5-108">A term.</span></span> <span data-ttu-id="c05c5-109">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="c05c5-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="c05c5-110">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="c05c5-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c05c5-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="c05c5-111">Properties</span></span>
| <span data-ttu-id="c05c5-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="c05c5-112">Property</span></span>     | <span data-ttu-id="c05c5-113">Тип</span><span class="sxs-lookup"><span data-stu-id="c05c5-113">Type</span></span>   |<span data-ttu-id="c05c5-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c05c5-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c05c5-115">displayName</span><span class="sxs-lookup"><span data-stu-id="c05c5-115">displayName</span></span>| <span data-ttu-id="c05c5-116">String</span><span class="sxs-lookup"><span data-stu-id="c05c5-116">String</span></span>| <span data-ttu-id="c05c5-117">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="c05c5-117">Display name of the term.</span></span>| 
|<span data-ttu-id="c05c5-118">externalId</span><span class="sxs-lookup"><span data-stu-id="c05c5-118">externalId</span></span>|<span data-ttu-id="c05c5-119">String</span><span class="sxs-lookup"><span data-stu-id="c05c5-119">String</span></span>| <span data-ttu-id="c05c5-120">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c05c5-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="c05c5-121">startDate</span><span class="sxs-lookup"><span data-stu-id="c05c5-121">startDate</span></span>|<span data-ttu-id="c05c5-122">Date</span><span class="sxs-lookup"><span data-stu-id="c05c5-122">Date</span></span>|<span data-ttu-id="c05c5-123">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="c05c5-123">Start of the term.</span></span>|
|<span data-ttu-id="c05c5-124">endDate</span><span class="sxs-lookup"><span data-stu-id="c05c5-124">endDate</span></span>|<span data-ttu-id="c05c5-125">Date</span><span class="sxs-lookup"><span data-stu-id="c05c5-125">Date</span></span>|<span data-ttu-id="c05c5-126">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="c05c5-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c05c5-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c05c5-127">JSON representation</span></span>

<span data-ttu-id="c05c5-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c05c5-128">The following is a JSON representation of the resource.</span></span>

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
