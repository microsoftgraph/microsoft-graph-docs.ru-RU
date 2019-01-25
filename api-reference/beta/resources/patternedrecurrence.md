---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
ms.openlocfilehash: f4ffd62b54eb6d577269b36d0ee3bea0a3a0002c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512026"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="f9240-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f9240-103">patternedRecurrence resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9240-104">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="f9240-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="f9240-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9240-105">Properties</span></span>
| <span data-ttu-id="f9240-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9240-106">Property</span></span>     | <span data-ttu-id="f9240-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f9240-107">Type</span></span>   |<span data-ttu-id="f9240-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f9240-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9240-109">pattern</span><span class="sxs-lookup"><span data-stu-id="f9240-109">pattern</span></span>|[<span data-ttu-id="f9240-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="f9240-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="f9240-111">Частота события.</span><span class="sxs-lookup"><span data-stu-id="f9240-111">The frequency of an event.</span></span>|
|<span data-ttu-id="f9240-112">range</span><span class="sxs-lookup"><span data-stu-id="f9240-112">range</span></span>|[<span data-ttu-id="f9240-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="f9240-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="f9240-114">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="f9240-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9240-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9240-115">JSON representation</span></span>

<span data-ttu-id="f9240-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9240-116">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/patternedrecurrence.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
