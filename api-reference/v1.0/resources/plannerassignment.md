---
title: Тип ресурса Планнерассигнмент
description: Ресурс **планнерассигнмент** представляет назначение задачи пользователю. Этот тип используется в открытом типе Планнерассигнментс.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5ae09a6c528e0311c542283ea5929ffba88ba029
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447145"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="9801d-104">Тип ресурса Планнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="9801d-104">plannerAssignment resource type</span></span>

<span data-ttu-id="9801d-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9801d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9801d-106">Ресурс **планнерассигнмент** представляет назначение задачи пользователю.</span><span class="sxs-lookup"><span data-stu-id="9801d-106">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="9801d-107">Этот тип используется в открытом типе [планнерассигнментс](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="9801d-107">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="9801d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9801d-108">Properties</span></span>
| <span data-ttu-id="9801d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9801d-109">Property</span></span>     | <span data-ttu-id="9801d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9801d-110">Type</span></span>   |<span data-ttu-id="9801d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9801d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9801d-112">ассигнедби</span><span class="sxs-lookup"><span data-stu-id="9801d-112">assignedBy</span></span>|[<span data-ttu-id="9801d-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="9801d-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="9801d-114">Идентификатор пользователя, который выполнил назначение задачи, например, назначение.</span><span class="sxs-lookup"><span data-stu-id="9801d-114">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="9801d-115">ассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="9801d-115">assignedDateTime</span></span>|<span data-ttu-id="9801d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9801d-116">DateTimeOffset</span></span>|<span data-ttu-id="9801d-117">Время назначения задачи.</span><span class="sxs-lookup"><span data-stu-id="9801d-117">The time at which the task was assigned.</span></span> <span data-ttu-id="9801d-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9801d-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9801d-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9801d-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9801d-120">orderHint</span><span class="sxs-lookup"><span data-stu-id="9801d-120">orderHint</span></span>|<span data-ttu-id="9801d-121">String</span><span class="sxs-lookup"><span data-stu-id="9801d-121">String</span></span>|<span data-ttu-id="9801d-122">Подсказка, используемая для упорядочивания уполномоченные в задаче.</span><span class="sxs-lookup"><span data-stu-id="9801d-122">Hint used to order assignees in a task.</span></span> <span data-ttu-id="9801d-123">Формат определяется, как описано [ниже](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="9801d-123">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9801d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9801d-124">JSON representation</span></span>
<span data-ttu-id="9801d-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9801d-125">Here is a JSON representation of the resource.</span></span>

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
