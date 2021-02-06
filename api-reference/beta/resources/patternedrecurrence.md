---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: harini84
ms.openlocfilehash: e64fa16f1aceb22eccd744588bd325943f79e930
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137650"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="e50b6-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e50b6-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="e50b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e50b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e50b6-105">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="e50b6-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="e50b6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e50b6-106">Properties</span></span>
| <span data-ttu-id="e50b6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e50b6-107">Property</span></span>     | <span data-ttu-id="e50b6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e50b6-108">Type</span></span>   |<span data-ttu-id="e50b6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e50b6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e50b6-110">pattern</span><span class="sxs-lookup"><span data-stu-id="e50b6-110">pattern</span></span>|[<span data-ttu-id="e50b6-111">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="e50b6-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="e50b6-112">Частота события.</span><span class="sxs-lookup"><span data-stu-id="e50b6-112">The frequency of an event.</span></span>|
|<span data-ttu-id="e50b6-113">range</span><span class="sxs-lookup"><span data-stu-id="e50b6-113">range</span></span>|[<span data-ttu-id="e50b6-114">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="e50b6-114">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="e50b6-115">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="e50b6-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e50b6-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e50b6-116">JSON representation</span></span>

<span data-ttu-id="e50b6-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e50b6-117">Here is a JSON representation of the resource</span></span>

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


