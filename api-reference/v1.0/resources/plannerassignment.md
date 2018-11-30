---
title: Тип ресурса plannerAssignment
description: Ресурс **plannerAssignment** представляет назначения задачи для пользователя. Этот тип используется в plannerAssignments открытого типа.
ms.openlocfilehash: 4fe44f39428fc8940514e68443fef072bd6d0d55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025752"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="99164-104">Тип ресурса plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="99164-104">plannerAssignment resource type</span></span>

<span data-ttu-id="99164-p102">Ресурс **plannerAssignment** представляет назначение задачи пользователю. Этот тип используется в открытом типе [plannerAssignments](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="99164-p102">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="99164-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="99164-107">Properties</span></span>
| <span data-ttu-id="99164-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="99164-108">Property</span></span>     | <span data-ttu-id="99164-109">Тип</span><span class="sxs-lookup"><span data-stu-id="99164-109">Type</span></span>   |<span data-ttu-id="99164-110">Описание</span><span class="sxs-lookup"><span data-stu-id="99164-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99164-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="99164-111">assignedBy</span></span>|[<span data-ttu-id="99164-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="99164-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="99164-113">Удостоверение пользователя, назначившего задачу.</span><span class="sxs-lookup"><span data-stu-id="99164-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="99164-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="99164-114">assignedDateTime</span></span>|<span data-ttu-id="99164-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99164-115">DateTimeOffset</span></span>|<span data-ttu-id="99164-p103">Дата и время назначения задачи. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="99164-p103">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99164-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="99164-119">orderHint</span></span>|<span data-ttu-id="99164-120">String</span><span class="sxs-lookup"><span data-stu-id="99164-120">String</span></span>|<span data-ttu-id="99164-p104">Указание, которое позволяет упорядочить назначенных пользователей для задачи. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="99164-p104">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99164-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="99164-123">JSON representation</span></span>
<span data-ttu-id="99164-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99164-124">Here is a JSON representation of the resource.</span></span>

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