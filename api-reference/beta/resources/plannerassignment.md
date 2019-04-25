---
title: Тип ресурса Планнерассигнмент
description: Ресурс **планнерассигнмент** представляет назначение задачи пользователю. Этот тип используется в открытом типе Планнерассигнментс.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 054cd42eedd27a7fe11abc2e5578a56da667e05d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541362"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="b9321-104">Тип ресурса Планнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="b9321-104">plannerAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9321-105">Ресурс **планнерассигнмент** представляет назначение задачи пользователю.</span><span class="sxs-lookup"><span data-stu-id="b9321-105">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="b9321-106">Этот тип используется в открытом типе [планнерассигнментс](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="b9321-106">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="b9321-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9321-107">Properties</span></span>
| <span data-ttu-id="b9321-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9321-108">Property</span></span>     | <span data-ttu-id="b9321-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9321-109">Type</span></span>   |<span data-ttu-id="b9321-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9321-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9321-111">Ассигнедби</span><span class="sxs-lookup"><span data-stu-id="b9321-111">assignedBy</span></span>|[<span data-ttu-id="b9321-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="b9321-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="b9321-113">Идентификатор пользователя, который выполнил назначение задачи, например, назначение.</span><span class="sxs-lookup"><span data-stu-id="b9321-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="b9321-114">Ассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="b9321-114">assignedDateTime</span></span>|<span data-ttu-id="b9321-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9321-115">DateTimeOffset</span></span>|<span data-ttu-id="b9321-116">Время назначения задачи.</span><span class="sxs-lookup"><span data-stu-id="b9321-116">The time at which the task was assigned.</span></span> <span data-ttu-id="b9321-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b9321-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9321-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b9321-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b9321-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="b9321-119">orderHint</span></span>|<span data-ttu-id="b9321-120">String</span><span class="sxs-lookup"><span data-stu-id="b9321-120">String</span></span>|<span data-ttu-id="b9321-121">ПодСказка, используемая для упорядочивания уполномоченные в задаче.</span><span class="sxs-lookup"><span data-stu-id="b9321-121">Hint used to order assignees in a task.</span></span> <span data-ttu-id="b9321-122">Формат определяется, как описано [ниже](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="b9321-122">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9321-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9321-123">JSON representation</span></span>
<span data-ttu-id="b9321-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9321-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
