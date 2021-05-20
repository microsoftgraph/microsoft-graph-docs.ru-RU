---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: harini84
ms.openlocfilehash: baff2147ee0a9e03e4e55a143341171707dee2d7
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579307"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="b31f1-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="b31f1-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="b31f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b31f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b31f1-105">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="b31f1-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="b31f1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b31f1-106">Properties</span></span>
| <span data-ttu-id="b31f1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b31f1-107">Property</span></span>     | <span data-ttu-id="b31f1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b31f1-108">Type</span></span>   |<span data-ttu-id="b31f1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b31f1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b31f1-110">pattern</span><span class="sxs-lookup"><span data-stu-id="b31f1-110">pattern</span></span>|[<span data-ttu-id="b31f1-111">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="b31f1-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="b31f1-112">Частота события.</span><span class="sxs-lookup"><span data-stu-id="b31f1-112">The frequency of an event.</span></span> <span data-ttu-id="b31f1-113">Не указывая для разового просмотра доступа.</span><span class="sxs-lookup"><span data-stu-id="b31f1-113">Do not specify for a one-time access review.</span></span>|
|<span data-ttu-id="b31f1-114">range</span><span class="sxs-lookup"><span data-stu-id="b31f1-114">range</span></span>|[<span data-ttu-id="b31f1-115">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="b31f1-115">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="b31f1-116">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="b31f1-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b31f1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b31f1-117">JSON representation</span></span>

<span data-ttu-id="b31f1-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b31f1-118">Here is a JSON representation of the resource</span></span>

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


