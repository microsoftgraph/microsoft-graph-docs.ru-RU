---
title: Тип ресурсов timeConstraint
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
localization_priority: Normal
ms.openlocfilehash: b6e239abbd0d9f7b4f83df4a60625a2f88131476
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815094"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="8948d-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="8948d-103">timeConstraint resource type</span></span>

<span data-ttu-id="8948d-104">Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.</span><span class="sxs-lookup"><span data-stu-id="8948d-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8948d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8948d-105">JSON representation</span></span>

<span data-ttu-id="8948d-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8948d-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8948d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8948d-107">Properties</span></span>
| <span data-ttu-id="8948d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8948d-108">Property</span></span>     | <span data-ttu-id="8948d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8948d-109">Type</span></span>   |<span data-ttu-id="8948d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8948d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8948d-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="8948d-111">activityDomain</span></span>|<span data-ttu-id="8948d-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="8948d-112">activityDomain</span></span>|<span data-ttu-id="8948d-113">Природы действия, необязательно.</span><span class="sxs-lookup"><span data-stu-id="8948d-113">The nature of the activity, optional.</span></span> <span data-ttu-id="8948d-114">Возможные значения: `work`, `personal`, `unrestricted`, или `unknown`.</span><span class="sxs-lookup"><span data-stu-id="8948d-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="8948d-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="8948d-115">timeslots</span></span>|<span data-ttu-id="8948d-116">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="8948d-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="8948d-117">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="8948d-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
