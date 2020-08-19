---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 7ca993e0639e532338ade3c3e1dc57d1baf284fc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807159"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="6b4ca-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="6b4ca-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="6b4ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b4ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b4ca-105">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="6b4ca-105">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="6b4ca-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b4ca-106">Properties</span></span>
| <span data-ttu-id="6b4ca-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b4ca-107">Property</span></span>     | <span data-ttu-id="6b4ca-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6b4ca-108">Type</span></span>   |<span data-ttu-id="6b4ca-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6b4ca-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b4ca-110">pattern</span><span class="sxs-lookup"><span data-stu-id="6b4ca-110">pattern</span></span>|[<span data-ttu-id="6b4ca-111">recurrencePattern</span><span class="sxs-lookup"><span data-stu-id="6b4ca-111">recurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="6b4ca-112">Частота события.</span><span class="sxs-lookup"><span data-stu-id="6b4ca-112">The frequency of an event.</span></span>|
|<span data-ttu-id="6b4ca-113">range</span><span class="sxs-lookup"><span data-stu-id="6b4ca-113">range</span></span>|[<span data-ttu-id="6b4ca-114">recurrenceRange</span><span class="sxs-lookup"><span data-stu-id="6b4ca-114">recurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="6b4ca-115">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="6b4ca-115">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b4ca-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6b4ca-116">JSON representation</span></span>

<span data-ttu-id="6b4ca-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b4ca-117">Here is a JSON representation of the resource</span></span>

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
