---
title: Тип ресурсов timeConstraint
description: Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cc6ace98b84e8b844139c148215eeffdd4c3ad49
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446823"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="284b7-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="284b7-103">timeConstraint resource type</span></span>

<span data-ttu-id="284b7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="284b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="284b7-105">Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.</span><span class="sxs-lookup"><span data-stu-id="284b7-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="284b7-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="284b7-106">JSON representation</span></span>

<span data-ttu-id="284b7-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="284b7-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="284b7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="284b7-108">Properties</span></span>
| <span data-ttu-id="284b7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="284b7-109">Property</span></span>     | <span data-ttu-id="284b7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="284b7-110">Type</span></span>   |<span data-ttu-id="284b7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="284b7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="284b7-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="284b7-112">activityDomain</span></span>|<span data-ttu-id="284b7-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="284b7-113">activityDomain</span></span>|<span data-ttu-id="284b7-114">Описание действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="284b7-114">The nature of the activity, optional.</span></span> <span data-ttu-id="284b7-115">`work`Возможные значения: `personal`,, `unrestricted`, или. `unknown`</span><span class="sxs-lookup"><span data-stu-id="284b7-115">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="284b7-116">timeslots</span><span class="sxs-lookup"><span data-stu-id="284b7-116">timeslots</span></span>|<span data-ttu-id="284b7-117">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="284b7-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="284b7-118">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="284b7-118">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
