---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
ms.openlocfilehash: 063df70dfeeb1d37cfc5e23710108dd4cfc9ae57
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344938"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="e5341-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e5341-103">patternedRecurrence resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5341-104">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="e5341-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="e5341-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5341-105">Properties</span></span>
| <span data-ttu-id="e5341-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5341-106">Property</span></span>     | <span data-ttu-id="e5341-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e5341-107">Type</span></span>   |<span data-ttu-id="e5341-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e5341-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5341-109">pattern</span><span class="sxs-lookup"><span data-stu-id="e5341-109">pattern</span></span>|[<span data-ttu-id="e5341-110">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="e5341-110">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="e5341-111">Частота события.</span><span class="sxs-lookup"><span data-stu-id="e5341-111">The frequency of an event.</span></span>|
|<span data-ttu-id="e5341-112">range</span><span class="sxs-lookup"><span data-stu-id="e5341-112">range</span></span>|[<span data-ttu-id="e5341-113">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="e5341-113">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="e5341-114">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="e5341-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5341-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5341-115">JSON representation</span></span>

<span data-ttu-id="e5341-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5341-116">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
