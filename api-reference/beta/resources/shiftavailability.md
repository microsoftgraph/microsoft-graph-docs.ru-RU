---
title: Тип ресурса Шифтаваилабилити
description: Доступность пользователя для планирования работы и расписания повторения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4a284774b76774da0420322f0cd2e092aec6ce83
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952288"
---
# <a name="shiftavailability-resource-type"></a><span data-ttu-id="0de96-103">Тип ресурса Шифтаваилабилити</span><span class="sxs-lookup"><span data-stu-id="0de96-103">shiftAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0de96-104">Доступность пользователя, запланированного для [смены](shift.md) и шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="0de96-104">Availability of the user to be scheduled for a [shift](shift.md) and its recurrence pattern.</span></span>

## <a name="properties"></a><span data-ttu-id="0de96-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0de96-105">Properties</span></span>

| <span data-ttu-id="0de96-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0de96-106">Property</span></span>     | <span data-ttu-id="0de96-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0de96-107">Type</span></span>        | <span data-ttu-id="0de96-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0de96-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0de96-109">recurrence</span><span class="sxs-lookup"><span data-stu-id="0de96-109">recurrence</span></span>|[<span data-ttu-id="0de96-110">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="0de96-110">patternedRecurrence</span></span>](patternedrecurrence.md)| <span data-ttu-id="0de96-111">Задает шаблон повторения</span><span class="sxs-lookup"><span data-stu-id="0de96-111">Specifies the pattern for recurrence</span></span> |
|<span data-ttu-id="0de96-112">тимеслотс</span><span class="sxs-lookup"><span data-stu-id="0de96-112">timeSlots</span></span>|<span data-ttu-id="0de96-113">Коллекция [тимеранже](timerange.md)</span><span class="sxs-lookup"><span data-stu-id="0de96-113">[timeRange](timerange.md) collection</span></span>|<span data-ttu-id="0de96-114">Временные слоты, предпочитаемые пользователем.</span><span class="sxs-lookup"><span data-stu-id="0de96-114">The time slot(s) preferred by the user.</span></span>|
|<span data-ttu-id="0de96-115">timeZone</span><span class="sxs-lookup"><span data-stu-id="0de96-115">timeZone</span></span>|<span data-ttu-id="0de96-116">String</span><span class="sxs-lookup"><span data-stu-id="0de96-116">String</span></span>|<span data-ttu-id="0de96-117">Указывает часовой пояс для указанного времени.</span><span class="sxs-lookup"><span data-stu-id="0de96-117">Specifies the time zone for the indicated time.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0de96-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0de96-118">JSON representation</span></span>

<span data-ttu-id="0de96-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0de96-119">The following is a JSON representation of the resource.</span></span>

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
