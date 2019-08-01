---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a5ad30474b23c6ef96bbc1a66142098e7f696138
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035569"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="c552a-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="c552a-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="c552a-104">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="c552a-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="c552a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c552a-105">Properties</span></span>
| <span data-ttu-id="c552a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c552a-106">Property</span></span>     | <span data-ttu-id="c552a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c552a-107">Type</span></span>   |<span data-ttu-id="c552a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c552a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c552a-109">pattern</span><span class="sxs-lookup"><span data-stu-id="c552a-109">pattern</span></span>|[<span data-ttu-id="c552a-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="c552a-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="c552a-111">Частота события.</span><span class="sxs-lookup"><span data-stu-id="c552a-111">The frequency of an event.</span></span>|
|<span data-ttu-id="c552a-112">range</span><span class="sxs-lookup"><span data-stu-id="c552a-112">range</span></span>|[<span data-ttu-id="c552a-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="c552a-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="c552a-114">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="c552a-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c552a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c552a-115">JSON representation</span></span>

<span data-ttu-id="c552a-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c552a-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
