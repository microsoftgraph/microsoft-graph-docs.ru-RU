---
title: Тип ресурсов timeConstraint
description: Ограничивает количество предложений по времени собраний определенным часам и дням недели в соответствии с заданным характером действий и интервалами времени открытия.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d79fc1630522c30abea6ac5ec6f51d0f5a15e437
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472113"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="01cfb-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="01cfb-103">timeConstraint resource type</span></span>

<span data-ttu-id="01cfb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01cfb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01cfb-105">Ограничивает количество предложений по времени собраний определенным часам и дням недели в соответствии с заданным характером действий и интервалами времени открытия.</span><span class="sxs-lookup"><span data-stu-id="01cfb-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="01cfb-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01cfb-106">JSON representation</span></span>
<span data-ttu-id="01cfb-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="01cfb-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}
```

## <a name="properties"></a><span data-ttu-id="01cfb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="01cfb-108">Properties</span></span>
| <span data-ttu-id="01cfb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="01cfb-109">Property</span></span>     | <span data-ttu-id="01cfb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="01cfb-110">Type</span></span>   |<span data-ttu-id="01cfb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="01cfb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01cfb-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="01cfb-112">activityDomain</span></span>|<span data-ttu-id="01cfb-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="01cfb-113">activityDomain</span></span>|<span data-ttu-id="01cfb-114">Описание действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="01cfb-114">The nature of the activity, optional.</span></span> <span data-ttu-id="01cfb-115">Возможные значения: `work` `personal` , , , или `unrestricted` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="01cfb-115">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="01cfb-116">timeslots</span><span class="sxs-lookup"><span data-stu-id="01cfb-116">timeslots</span></span>|<span data-ttu-id="01cfb-117">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="01cfb-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="01cfb-118">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="01cfb-118">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


