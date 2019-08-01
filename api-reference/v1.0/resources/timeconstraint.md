---
title: Тип ресурсов timeConstraint
description: Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7da2a3a2c712cdbe1fc3fb961781e35099a565d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033616"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="5e70b-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="5e70b-103">timeConstraint resource type</span></span>

<span data-ttu-id="5e70b-104">Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.</span><span class="sxs-lookup"><span data-stu-id="5e70b-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e70b-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e70b-105">JSON representation</span></span>

<span data-ttu-id="5e70b-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="5e70b-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="5e70b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e70b-107">Properties</span></span>
| <span data-ttu-id="5e70b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e70b-108">Property</span></span>     | <span data-ttu-id="5e70b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5e70b-109">Type</span></span>   |<span data-ttu-id="5e70b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e70b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e70b-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="5e70b-111">activityDomain</span></span>|<span data-ttu-id="5e70b-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="5e70b-112">activityDomain</span></span>|<span data-ttu-id="5e70b-113">Описание действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="5e70b-113">The nature of the activity, optional.</span></span> <span data-ttu-id="5e70b-114">`work`Возможные значения: `personal`,, `unrestricted`, или. `unknown`</span><span class="sxs-lookup"><span data-stu-id="5e70b-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="5e70b-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="5e70b-115">timeslots</span></span>|<span data-ttu-id="5e70b-116">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="5e70b-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="5e70b-117">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="5e70b-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
