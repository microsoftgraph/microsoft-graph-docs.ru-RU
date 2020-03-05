---
title: Тип ресурса Шифтаваилабилити
description: Доступность пользователя для планирования работы и расписания повторения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8e06b64bc01be163149468c9090df2a8ea59497d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520627"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="f03b9-103">Тип ресурса Шифтаваилабилити</span><span class="sxs-lookup"><span data-stu-id="f03b9-103">shiftAvailability resource type</span></span>

<span data-ttu-id="f03b9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f03b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f03b9-105">Доступность пользователя, запланированного для [смены](shift.md) и шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="f03b9-105">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="f03b9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f03b9-106">Properties</span></span>

| <span data-ttu-id="f03b9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f03b9-107">Property</span></span>     | <span data-ttu-id="f03b9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f03b9-108">Type</span></span>        | <span data-ttu-id="f03b9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f03b9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f03b9-110">recurrence</span><span class="sxs-lookup"><span data-stu-id="f03b9-110">recurrence</span></span>|[<span data-ttu-id="f03b9-111">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f03b9-111">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="f03b9-112">Задает шаблон повторения</span><span class="sxs-lookup"><span data-stu-id="f03b9-112">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="f03b9-113">тимеслотс</span><span class="sxs-lookup"><span data-stu-id="f03b9-113">timeSlots</span></span>|<span data-ttu-id="f03b9-114">Коллекция [тимеранже](timerange.md)</span><span class="sxs-lookup"><span data-stu-id="f03b9-114">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="f03b9-115">Временные слоты, предпочитаемые пользователем.</span><span class="sxs-lookup"><span data-stu-id="f03b9-115">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="f03b9-116">timeZone</span><span class="sxs-lookup"><span data-stu-id="f03b9-116">timeZone</span></span>|<span data-ttu-id="f03b9-117">String</span><span class="sxs-lookup"><span data-stu-id="f03b9-117">String</span></span>|<span data-ttu-id="f03b9-118">Указывает часовой пояс для указанного времени.</span><span class="sxs-lookup"><span data-stu-id="f03b9-118">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f03b9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f03b9-119">JSON representation</span></span>

<span data-ttu-id="f03b9-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f03b9-120">The following is a JSON representation of the resource.</span></span>

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
