---
title: Тип ресурсов timeConstraint
description: Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 3ce27e94ff4f201def558ae4478e12642efeb638
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342053"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="31c97-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="31c97-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31c97-104">Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.</span><span class="sxs-lookup"><span data-stu-id="31c97-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="31c97-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31c97-105">JSON representation</span></span>
<span data-ttu-id="31c97-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="31c97-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="31c97-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="31c97-107">Properties</span></span>
| <span data-ttu-id="31c97-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="31c97-108">Property</span></span>     | <span data-ttu-id="31c97-109">Тип</span><span class="sxs-lookup"><span data-stu-id="31c97-109">Type</span></span>   |<span data-ttu-id="31c97-110">Описание</span><span class="sxs-lookup"><span data-stu-id="31c97-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31c97-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="31c97-111">activityDomain</span></span>|<span data-ttu-id="31c97-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="31c97-112">activityDomain</span></span>|<span data-ttu-id="31c97-113">Описание действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="31c97-113">The nature of the activity, optional.</span></span> <span data-ttu-id="31c97-114">`work`Возможные значения: `personal`,, `unrestricted`, или. `unknown`</span><span class="sxs-lookup"><span data-stu-id="31c97-114">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="31c97-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="31c97-115">timeslots</span></span>|<span data-ttu-id="31c97-116">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="31c97-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="31c97-117">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="31c97-117">An array of time periods.</span></span>|

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
