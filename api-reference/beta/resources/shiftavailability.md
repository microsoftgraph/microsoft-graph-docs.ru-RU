---
title: Тип ресурса Шифтаваилабилити
description: Доступность пользователя для планирования работы и расписания повторения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86ad11ae32977ac07a7755ebe0a169686f6f605e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058055"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="17781-103">Тип ресурса Шифтаваилабилити</span><span class="sxs-lookup"><span data-stu-id="17781-103">shiftAvailability resource type</span></span>

<span data-ttu-id="17781-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17781-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17781-105">Доступность пользователя, запланированного для [смены](shift.md) и шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="17781-105">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="17781-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="17781-106">Properties</span></span>

| <span data-ttu-id="17781-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="17781-107">Property</span></span>     | <span data-ttu-id="17781-108">Тип</span><span class="sxs-lookup"><span data-stu-id="17781-108">Type</span></span>        | <span data-ttu-id="17781-109">Описание</span><span class="sxs-lookup"><span data-stu-id="17781-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17781-110">recurrence</span><span class="sxs-lookup"><span data-stu-id="17781-110">recurrence</span></span>|[<span data-ttu-id="17781-111">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="17781-111">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="17781-112">Задает шаблон повторения</span><span class="sxs-lookup"><span data-stu-id="17781-112">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="17781-113">тимеслотс</span><span class="sxs-lookup"><span data-stu-id="17781-113">timeSlots</span></span>|<span data-ttu-id="17781-114">Коллекция [тимеранже](timerange.md)</span><span class="sxs-lookup"><span data-stu-id="17781-114">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="17781-115">Временные слоты, предпочитаемые пользователем.</span><span class="sxs-lookup"><span data-stu-id="17781-115">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="17781-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="17781-116">timeZone</span></span>|<span data-ttu-id="17781-117">String</span><span class="sxs-lookup"><span data-stu-id="17781-117">String</span></span>|<span data-ttu-id="17781-118">Указывает часовой пояс для указанного времени.</span><span class="sxs-lookup"><span data-stu-id="17781-118">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17781-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="17781-119">JSON representation</span></span>

<span data-ttu-id="17781-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17781-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftAvailability",
  "baseType": null
}-->

```json
{
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "timeSlots": [{"@odata.type": "microsoft.graph.timeRange"}],
  "timeZone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


