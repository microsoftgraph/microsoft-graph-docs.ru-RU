---
title: Тип ресурсов timeConstraint
description: Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8393e4b501815dcbd0195e04ca82cd639d1a84c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964321"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="07942-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="07942-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07942-104">Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.</span><span class="sxs-lookup"><span data-stu-id="07942-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="07942-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07942-105">JSON representation</span></span>
<span data-ttu-id="07942-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="07942-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="07942-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="07942-107">Properties</span></span>
| <span data-ttu-id="07942-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="07942-108">Property</span></span>     | <span data-ttu-id="07942-109">Тип</span><span class="sxs-lookup"><span data-stu-id="07942-109">Type</span></span>   |<span data-ttu-id="07942-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07942-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07942-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="07942-111">activityDomain</span></span>|<span data-ttu-id="07942-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="07942-112">activityDomain</span></span>|<span data-ttu-id="07942-113">Описание действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="07942-113">The nature of the activity, optional.</span></span> <span data-ttu-id="07942-114">`work`Возможные значения: `personal`,, `unrestricted`, или. `unknown`</span><span class="sxs-lookup"><span data-stu-id="07942-114">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="07942-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="07942-115">timeslots</span></span>|<span data-ttu-id="07942-116">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="07942-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="07942-117">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="07942-117">An array of time periods.</span></span>|

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
