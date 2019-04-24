---
title: Тип ресурсов timeConstraint
description: Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.
localization_priority: Normal
ms.openlocfilehash: b6e239abbd0d9f7b4f83df4a60625a2f88131476
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456960"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="daa65-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="daa65-103">timeConstraint resource type</span></span>

<span data-ttu-id="daa65-104">Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.</span><span class="sxs-lookup"><span data-stu-id="daa65-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="daa65-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="daa65-105">JSON representation</span></span>

<span data-ttu-id="daa65-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="daa65-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="daa65-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="daa65-107">Properties</span></span>
| <span data-ttu-id="daa65-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="daa65-108">Property</span></span>     | <span data-ttu-id="daa65-109">Тип</span><span class="sxs-lookup"><span data-stu-id="daa65-109">Type</span></span>   |<span data-ttu-id="daa65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="daa65-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daa65-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="daa65-111">activityDomain</span></span>|<span data-ttu-id="daa65-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="daa65-112">activityDomain</span></span>|<span data-ttu-id="daa65-113">Описание действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="daa65-113">The nature of the activity, optional.</span></span> <span data-ttu-id="daa65-114">`work`Возможные значения: `personal`,, `unrestricted`, или. `unknown`</span><span class="sxs-lookup"><span data-stu-id="daa65-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="daa65-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="daa65-115">timeslots</span></span>|<span data-ttu-id="daa65-116">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="daa65-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="daa65-117">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="daa65-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
