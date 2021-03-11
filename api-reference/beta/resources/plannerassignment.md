---
title: Тип ресурса plannerAssignment
description: Ресурс **plannerAssignment** представляет назначение задачи пользователю. Этот тип используется в планировщиках открытого типаAssignments.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d9e608b027200566fc957b3c267e56b599d7b0cb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721175"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="b96a1-104">Тип ресурса plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="b96a1-104">plannerAssignment resource type</span></span>

<span data-ttu-id="b96a1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b96a1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b96a1-106">Ресурс **plannerAssignment** представляет назначение задачи пользователю.</span><span class="sxs-lookup"><span data-stu-id="b96a1-106">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="b96a1-107">Этот тип используется в планировщиках открытого [типаAssignments.](plannerassignments.md)</span><span class="sxs-lookup"><span data-stu-id="b96a1-107">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="b96a1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b96a1-108">Properties</span></span>
| <span data-ttu-id="b96a1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b96a1-109">Property</span></span>     | <span data-ttu-id="b96a1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b96a1-110">Type</span></span>   |<span data-ttu-id="b96a1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b96a1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b96a1-112">assignedBy</span><span class="sxs-lookup"><span data-stu-id="b96a1-112">assignedBy</span></span>|[<span data-ttu-id="b96a1-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="b96a1-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="b96a1-114">Удостоверение пользователя, который выполнил назначение задачи, то есть назначителя.</span><span class="sxs-lookup"><span data-stu-id="b96a1-114">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="b96a1-115">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="b96a1-115">assignedDateTime</span></span>|<span data-ttu-id="b96a1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b96a1-116">DateTimeOffset</span></span>|<span data-ttu-id="b96a1-117">Время, в которое была назначена задача.</span><span class="sxs-lookup"><span data-stu-id="b96a1-117">The time at which the task was assigned.</span></span> <span data-ttu-id="b96a1-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b96a1-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b96a1-119">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b96a1-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b96a1-120">orderHint</span><span class="sxs-lookup"><span data-stu-id="b96a1-120">orderHint</span></span>|<span data-ttu-id="b96a1-121">String</span><span class="sxs-lookup"><span data-stu-id="b96a1-121">String</span></span>|<span data-ttu-id="b96a1-122">Подсказка, используемая для заказа назначаемой задачи.</span><span class="sxs-lookup"><span data-stu-id="b96a1-122">Hint used to order assignees in a task.</span></span> <span data-ttu-id="b96a1-123">Формат определяется как описанный [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="b96a1-123">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b96a1-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b96a1-124">JSON representation</span></span>
<span data-ttu-id="b96a1-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b96a1-125">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


