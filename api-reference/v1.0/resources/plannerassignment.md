---
title: Тип ресурса Планнерассигнмент
description: Ресурс **планнерассигнмент** представляет назначение задачи пользователю. Этот тип используется в открытом типе Планнерассигнментс.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f6346dd10101b6611ec46f01eb049c97774cea09
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035345"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="7648c-104">Тип ресурса Планнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="7648c-104">plannerAssignment resource type</span></span>

<span data-ttu-id="7648c-105">Ресурс **планнерассигнмент** представляет назначение задачи пользователю.</span><span class="sxs-lookup"><span data-stu-id="7648c-105">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="7648c-106">Этот тип используется в открытом типе [планнерассигнментс](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="7648c-106">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="7648c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7648c-107">Properties</span></span>
| <span data-ttu-id="7648c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7648c-108">Property</span></span>     | <span data-ttu-id="7648c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7648c-109">Type</span></span>   |<span data-ttu-id="7648c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7648c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7648c-111">Ассигнедби</span><span class="sxs-lookup"><span data-stu-id="7648c-111">assignedBy</span></span>|[<span data-ttu-id="7648c-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="7648c-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="7648c-113">Идентификатор пользователя, который выполнил назначение задачи, например, назначение.</span><span class="sxs-lookup"><span data-stu-id="7648c-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="7648c-114">Ассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="7648c-114">assignedDateTime</span></span>|<span data-ttu-id="7648c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7648c-115">DateTimeOffset</span></span>|<span data-ttu-id="7648c-116">Время назначения задачи.</span><span class="sxs-lookup"><span data-stu-id="7648c-116">The time at which the task was assigned.</span></span> <span data-ttu-id="7648c-117">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="7648c-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7648c-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7648c-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7648c-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="7648c-119">orderHint</span></span>|<span data-ttu-id="7648c-120">String</span><span class="sxs-lookup"><span data-stu-id="7648c-120">String</span></span>|<span data-ttu-id="7648c-121">Подсказка, используемая для упорядочивания уполномоченные в задаче.</span><span class="sxs-lookup"><span data-stu-id="7648c-121">Hint used to order assignees in a task.</span></span> <span data-ttu-id="7648c-122">Формат определяется, как описано [ниже](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="7648c-122">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7648c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7648c-123">JSON representation</span></span>
<span data-ttu-id="7648c-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7648c-124">Here is a JSON representation of the resource.</span></span>

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
