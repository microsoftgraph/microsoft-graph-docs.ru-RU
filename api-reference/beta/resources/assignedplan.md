---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов **user** и organization представляет собой коллекцию объектов assignedPlan.
localization_priority: Normal
ms.openlocfilehash: 3e06894fa71f81993b94d174d6cde8a54126fd62
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525138"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="6fef9-103">Тип ресурса assignedPlan</span><span class="sxs-lookup"><span data-stu-id="6fef9-103">assignedPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fef9-104">Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="6fef9-104">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="6fef9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fef9-105">Properties</span></span>
| <span data-ttu-id="6fef9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fef9-106">Property</span></span>     | <span data-ttu-id="6fef9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6fef9-107">Type</span></span>   |<span data-ttu-id="6fef9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6fef9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fef9-109">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fef9-109">assignedDateTime</span></span>|<span data-ttu-id="6fef9-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fef9-110">DateTimeOffset</span></span>|<span data-ttu-id="6fef9-p101">Дата и время назначения плана. Пример: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6fef9-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6fef9-114">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="6fef9-114">capabilityStatus</span></span>|<span data-ttu-id="6fef9-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6fef9-115">String</span></span>|<span data-ttu-id="6fef9-116">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="6fef9-116">For example, “Enabled”.</span></span>|
|<span data-ttu-id="6fef9-117">service</span><span class="sxs-lookup"><span data-stu-id="6fef9-117">service</span></span>|<span data-ttu-id="6fef9-118">String</span><span class="sxs-lookup"><span data-stu-id="6fef9-118">String</span></span>|<span data-ttu-id="6fef9-119">Имя службы, например "Exchange".</span><span class="sxs-lookup"><span data-stu-id="6fef9-119">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="6fef9-120">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="6fef9-120">servicePlanId</span></span>|<span data-ttu-id="6fef9-121">Guid</span><span class="sxs-lookup"><span data-stu-id="6fef9-121">Guid</span></span>|<span data-ttu-id="6fef9-122">Идентификатор GUID, определяющий план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="6fef9-122">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fef9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fef9-123">JSON representation</span></span>

<span data-ttu-id="6fef9-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fef9-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/assignedplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
