---
title: Тип ресурсов timeConstraint
description: Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4215b4350236956bfcad3bdf6f787b7f6c77f5dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075520"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="3a002-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="3a002-103">timeConstraint resource type</span></span>

<span data-ttu-id="3a002-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a002-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a002-105">Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.</span><span class="sxs-lookup"><span data-stu-id="3a002-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3a002-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a002-106">JSON representation</span></span>
<span data-ttu-id="3a002-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3a002-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3a002-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a002-108">Properties</span></span>
| <span data-ttu-id="3a002-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a002-109">Property</span></span>     | <span data-ttu-id="3a002-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3a002-110">Type</span></span>   |<span data-ttu-id="3a002-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3a002-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a002-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="3a002-112">activityDomain</span></span>|<span data-ttu-id="3a002-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="3a002-113">activityDomain</span></span>|<span data-ttu-id="3a002-114">Описание действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="3a002-114">The nature of the activity, optional.</span></span> <span data-ttu-id="3a002-115">Возможные значения: `work` , `personal` , `unrestricted` , или `unknown` .</span><span class="sxs-lookup"><span data-stu-id="3a002-115">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="3a002-116">timeslots</span><span class="sxs-lookup"><span data-stu-id="3a002-116">timeslots</span></span>|<span data-ttu-id="3a002-117">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="3a002-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="3a002-118">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="3a002-118">An array of time periods.</span></span>|

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


