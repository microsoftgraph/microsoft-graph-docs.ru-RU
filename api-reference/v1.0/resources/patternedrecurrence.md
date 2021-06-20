---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5bc4c78a4996c6690f40de863d20ba6f2d55949a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030875"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="e083a-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e083a-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="e083a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e083a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e083a-105">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="e083a-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="e083a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e083a-106">Properties</span></span>
| <span data-ttu-id="e083a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e083a-107">Property</span></span>     | <span data-ttu-id="e083a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e083a-108">Type</span></span>   |<span data-ttu-id="e083a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e083a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e083a-110">pattern</span><span class="sxs-lookup"><span data-stu-id="e083a-110">pattern</span></span>|[<span data-ttu-id="e083a-111">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="e083a-111">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="e083a-112">Частота события.</span><span class="sxs-lookup"><span data-stu-id="e083a-112">The frequency of an event.</span></span> <span data-ttu-id="e083a-113">Не указывая для разового просмотра доступа.</span><span class="sxs-lookup"><span data-stu-id="e083a-113">Do not specify for a one-time access review.</span></span>|
|<span data-ttu-id="e083a-114">range</span><span class="sxs-lookup"><span data-stu-id="e083a-114">range</span></span>|[<span data-ttu-id="e083a-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="e083a-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="e083a-116">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="e083a-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e083a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e083a-117">JSON representation</span></span>

<span data-ttu-id="e083a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e083a-118">Here is a JSON representation of the resource</span></span>

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

