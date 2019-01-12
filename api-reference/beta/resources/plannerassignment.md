---
title: Тип ресурса plannerAssignment
description: Ресурс **plannerAssignment** представляет назначения задачи для пользователя. Этот тип используется в plannerAssignments открытого типа.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5eaeb00abf7446db1085a7c0d0916b0a7b5b2434
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963964"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="99ff7-104">Тип ресурса plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="99ff7-104">plannerAssignment resource type</span></span>

> <span data-ttu-id="99ff7-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99ff7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99ff7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99ff7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99ff7-p103">Ресурс **plannerAssignment** представляет назначение задачи пользователю. Этот тип используется в открытом типе [plannerAssignments](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="99ff7-p103">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="99ff7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="99ff7-109">Properties</span></span>
| <span data-ttu-id="99ff7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="99ff7-110">Property</span></span>     | <span data-ttu-id="99ff7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="99ff7-111">Type</span></span>   |<span data-ttu-id="99ff7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="99ff7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99ff7-113">assignedBy</span><span class="sxs-lookup"><span data-stu-id="99ff7-113">assignedBy</span></span>|[<span data-ttu-id="99ff7-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="99ff7-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="99ff7-115">Удостоверение пользователя, назначившего задачу.</span><span class="sxs-lookup"><span data-stu-id="99ff7-115">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="99ff7-116">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="99ff7-116">assignedDateTime</span></span>|<span data-ttu-id="99ff7-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99ff7-117">DateTimeOffset</span></span>|<span data-ttu-id="99ff7-p104">Дата и время назначения задачи. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="99ff7-p104">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99ff7-121">orderHint</span><span class="sxs-lookup"><span data-stu-id="99ff7-121">orderHint</span></span>|<span data-ttu-id="99ff7-122">String</span><span class="sxs-lookup"><span data-stu-id="99ff7-122">String</span></span>|<span data-ttu-id="99ff7-p105">Указание, которое позволяет упорядочить назначенных пользователей для задачи. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="99ff7-p105">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99ff7-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="99ff7-125">JSON representation</span></span>
<span data-ttu-id="99ff7-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99ff7-126">Here is a JSON representation of the resource.</span></span>

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
