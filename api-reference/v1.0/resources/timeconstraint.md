---
title: Тип ресурсов timeConstraint
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
ms.openlocfilehash: 82ab18eb09201236f3227c7dd0660519092a3133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025135"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="85781-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="85781-103">timeConstraint resource type</span></span>

<span data-ttu-id="85781-104">Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.</span><span class="sxs-lookup"><span data-stu-id="85781-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85781-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85781-105">JSON representation</span></span>

<span data-ttu-id="85781-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="85781-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="85781-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="85781-107">Properties</span></span>
| <span data-ttu-id="85781-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="85781-108">Property</span></span>     | <span data-ttu-id="85781-109">Тип</span><span class="sxs-lookup"><span data-stu-id="85781-109">Type</span></span>   |<span data-ttu-id="85781-110">Описание</span><span class="sxs-lookup"><span data-stu-id="85781-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85781-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="85781-111">activityDomain</span></span>|<span data-ttu-id="85781-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="85781-112">activityDomain</span></span>|<span data-ttu-id="85781-113">Природы действия, необязательно.</span><span class="sxs-lookup"><span data-stu-id="85781-113">The nature of the activity, optional.</span></span> <span data-ttu-id="85781-114">Возможные значения: `work`, `personal`, `unrestricted`, или `unknown`.</span><span class="sxs-lookup"><span data-stu-id="85781-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="85781-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="85781-115">timeslots</span></span>|<span data-ttu-id="85781-116">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="85781-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="85781-117">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="85781-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
