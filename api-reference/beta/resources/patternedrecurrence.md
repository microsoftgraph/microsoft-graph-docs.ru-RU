---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b26a5272611e27ffe29afc0254c1d1384f6a9c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521992"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="99a77-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="99a77-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="99a77-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="99a77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99a77-105">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="99a77-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="99a77-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="99a77-106">Properties</span></span>
| <span data-ttu-id="99a77-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="99a77-107">Property</span></span>     | <span data-ttu-id="99a77-108">Тип</span><span class="sxs-lookup"><span data-stu-id="99a77-108">Type</span></span>   |<span data-ttu-id="99a77-109">Описание</span><span class="sxs-lookup"><span data-stu-id="99a77-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99a77-110">pattern</span><span class="sxs-lookup"><span data-stu-id="99a77-110">pattern</span></span>|[<span data-ttu-id="99a77-111">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="99a77-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="99a77-112">Частота события.</span><span class="sxs-lookup"><span data-stu-id="99a77-112">The frequency of an event.</span></span>|
|<span data-ttu-id="99a77-113">range</span><span class="sxs-lookup"><span data-stu-id="99a77-113">range</span></span>|[<span data-ttu-id="99a77-114">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="99a77-114">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="99a77-115">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="99a77-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99a77-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99a77-116">JSON representation</span></span>

<span data-ttu-id="99a77-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99a77-117">Here is a JSON representation of the resource</span></span>

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
