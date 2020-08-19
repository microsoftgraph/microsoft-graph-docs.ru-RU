---
title: Тип ресурсов timeConstraint
description: Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e2ecde664dbdf0335ce84083dfe3c29473c5b1d5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812143"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="d8ceb-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="d8ceb-103">timeConstraint resource type</span></span>

<span data-ttu-id="d8ceb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8ceb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8ceb-105">Запрещает предложения по времени собранию определенным часам и дням недели в соответствии с заданным характером активности и временем открытия.</span><span class="sxs-lookup"><span data-stu-id="d8ceb-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8ceb-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d8ceb-106">JSON representation</span></span>

<span data-ttu-id="d8ceb-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d8ceb-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d8ceb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8ceb-108">Properties</span></span>
| <span data-ttu-id="d8ceb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8ceb-109">Property</span></span>     | <span data-ttu-id="d8ceb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d8ceb-110">Type</span></span>   |<span data-ttu-id="d8ceb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8ceb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8ceb-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="d8ceb-112">activityDomain</span></span>|<span data-ttu-id="d8ceb-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="d8ceb-113">activityDomain</span></span>|<span data-ttu-id="d8ceb-114">Описание действия (необязательно).</span><span class="sxs-lookup"><span data-stu-id="d8ceb-114">The nature of the activity, optional.</span></span> <span data-ttu-id="d8ceb-115">Возможные значения: `work` , `personal` , `unrestricted` , или `unknown` .</span><span class="sxs-lookup"><span data-stu-id="d8ceb-115">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="d8ceb-116">timeslots</span><span class="sxs-lookup"><span data-stu-id="d8ceb-116">timeslots</span></span>|<span data-ttu-id="d8ceb-117">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="d8ceb-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="d8ceb-118">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="d8ceb-118">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
