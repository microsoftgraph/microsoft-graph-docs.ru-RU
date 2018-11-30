---
title: Тип ресурсов timeConstraint
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
ms.openlocfilehash: 092133d34e12fe5c06bfd8a76e8a33afb33892f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076034"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="d6bff-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="d6bff-103">timeConstraint resource type</span></span>

> <span data-ttu-id="d6bff-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6bff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6bff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6bff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6bff-106">Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.</span><span class="sxs-lookup"><span data-stu-id="d6bff-106">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6bff-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6bff-107">JSON representation</span></span>

<span data-ttu-id="d6bff-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d6bff-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="d6bff-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6bff-109">Properties</span></span>
| <span data-ttu-id="d6bff-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6bff-110">Property</span></span>     | <span data-ttu-id="d6bff-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d6bff-111">Type</span></span>   |<span data-ttu-id="d6bff-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d6bff-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6bff-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="d6bff-113">activityDomain</span></span>|<span data-ttu-id="d6bff-114">String</span><span class="sxs-lookup"><span data-stu-id="d6bff-114">String</span></span>|<span data-ttu-id="d6bff-p102">Описание действия (необязательно). Возможные значения: `work`, `personal`, `unrestricted` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d6bff-p102">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="d6bff-117">timeslots</span><span class="sxs-lookup"><span data-stu-id="d6bff-117">timeslots</span></span>|<span data-ttu-id="d6bff-118">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="d6bff-118">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="d6bff-119">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="d6bff-119">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->