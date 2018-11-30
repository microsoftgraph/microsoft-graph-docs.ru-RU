---
title: Тип ресурса plannerAssignment
description: Ресурс **plannerAssignment** представляет назначения задачи для пользователя. Этот тип используется в plannerAssignments открытого типа.
ms.openlocfilehash: 1efe7c3f2d3229bcce1d2c35e375cc636dadc51f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080916"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="111d8-104">Тип ресурса plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="111d8-104">plannerAssignment resource type</span></span>

> <span data-ttu-id="111d8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="111d8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="111d8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="111d8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="111d8-p103">Ресурс **plannerAssignment** представляет назначение задачи пользователю. Этот тип используется в открытом типе [plannerAssignments](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="111d8-p103">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="111d8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="111d8-109">Properties</span></span>
| <span data-ttu-id="111d8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="111d8-110">Property</span></span>     | <span data-ttu-id="111d8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="111d8-111">Type</span></span>   |<span data-ttu-id="111d8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="111d8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="111d8-113">assignedBy</span><span class="sxs-lookup"><span data-stu-id="111d8-113">assignedBy</span></span>|[<span data-ttu-id="111d8-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="111d8-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="111d8-115">Удостоверение пользователя, назначившего задачу.</span><span class="sxs-lookup"><span data-stu-id="111d8-115">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="111d8-116">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="111d8-116">assignedDateTime</span></span>|<span data-ttu-id="111d8-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="111d8-117">DateTimeOffset</span></span>|<span data-ttu-id="111d8-p104">Дата и время назначения задачи. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="111d8-p104">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="111d8-121">orderHint</span><span class="sxs-lookup"><span data-stu-id="111d8-121">orderHint</span></span>|<span data-ttu-id="111d8-122">String</span><span class="sxs-lookup"><span data-stu-id="111d8-122">String</span></span>|<span data-ttu-id="111d8-p105">Указание, которое позволяет упорядочить назначенных пользователей для задачи. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="111d8-p105">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="111d8-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="111d8-125">JSON representation</span></span>
<span data-ttu-id="111d8-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="111d8-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->