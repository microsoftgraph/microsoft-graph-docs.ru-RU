---
title: Тип ресурсов timeConstraint
description: Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.
localization_priority: Normal
ms.openlocfilehash: 6e3cc56f1495eae60bb84c458caa25c79557e033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832909"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="0f143-103">Тип ресурсов timeConstraint</span><span class="sxs-lookup"><span data-stu-id="0f143-103">timeConstraint resource type</span></span>

> <span data-ttu-id="0f143-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f143-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f143-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f143-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f143-106">Ограничивает предложения по времени проведения собрания определенными временными рамками и днями недели в соответствии с указанным описанием действия и доступными периодами времени.</span><span class="sxs-lookup"><span data-stu-id="0f143-106">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f143-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f143-107">JSON representation</span></span>

<span data-ttu-id="0f143-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="0f143-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0f143-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f143-109">Properties</span></span>
| <span data-ttu-id="0f143-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f143-110">Property</span></span>     | <span data-ttu-id="0f143-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0f143-111">Type</span></span>   |<span data-ttu-id="0f143-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0f143-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f143-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="0f143-113">activityDomain</span></span>|<span data-ttu-id="0f143-114">String</span><span class="sxs-lookup"><span data-stu-id="0f143-114">String</span></span>|<span data-ttu-id="0f143-p102">Описание действия (необязательно). Возможные значения: `work`, `personal`, `unrestricted` и `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0f143-p102">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="0f143-117">timeslots</span><span class="sxs-lookup"><span data-stu-id="0f143-117">timeslots</span></span>|<span data-ttu-id="0f143-118">Коллекция [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="0f143-118">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="0f143-119">Массив, содержащий значения периодов времени.</span><span class="sxs-lookup"><span data-stu-id="0f143-119">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
