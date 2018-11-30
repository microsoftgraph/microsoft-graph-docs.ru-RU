---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
ms.openlocfilehash: 10a90db032cd7461e28bc096fd6213df44f3ea45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025408"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="8cacf-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8cacf-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="8cacf-104">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="8cacf-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="8cacf-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cacf-105">Properties</span></span>
| <span data-ttu-id="8cacf-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cacf-106">Property</span></span>     | <span data-ttu-id="8cacf-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8cacf-107">Type</span></span>   |<span data-ttu-id="8cacf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8cacf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cacf-109">pattern</span><span class="sxs-lookup"><span data-stu-id="8cacf-109">pattern</span></span>|[<span data-ttu-id="8cacf-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="8cacf-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="8cacf-111">Частота события.</span><span class="sxs-lookup"><span data-stu-id="8cacf-111">The frequency of an event.</span></span>|
|<span data-ttu-id="8cacf-112">range</span><span class="sxs-lookup"><span data-stu-id="8cacf-112">range</span></span>|[<span data-ttu-id="8cacf-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="8cacf-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="8cacf-114">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="8cacf-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cacf-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cacf-115">JSON representation</span></span>

<span data-ttu-id="8cacf-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cacf-116">Here is a JSON representation of the resource</span></span>

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
