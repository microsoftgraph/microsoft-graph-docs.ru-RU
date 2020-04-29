---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 77c413f98e4c329e7dc7ebcb2412ac12bedfad8d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447229"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="6e969-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="6e969-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="6e969-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e969-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e969-105">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="6e969-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="6e969-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e969-106">Properties</span></span>
| <span data-ttu-id="6e969-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e969-107">Property</span></span>     | <span data-ttu-id="6e969-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6e969-108">Type</span></span>   |<span data-ttu-id="6e969-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6e969-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e969-110">pattern</span><span class="sxs-lookup"><span data-stu-id="6e969-110">pattern</span></span>|[<span data-ttu-id="6e969-111">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="6e969-111">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="6e969-112">Частота события.</span><span class="sxs-lookup"><span data-stu-id="6e969-112">The frequency of an event.</span></span>|
|<span data-ttu-id="6e969-113">range</span><span class="sxs-lookup"><span data-stu-id="6e969-113">range</span></span>|[<span data-ttu-id="6e969-114">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="6e969-114">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="6e969-115">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="6e969-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e969-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e969-116">JSON representation</span></span>

<span data-ttu-id="6e969-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e969-117">Here is a JSON representation of the resource</span></span>

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
