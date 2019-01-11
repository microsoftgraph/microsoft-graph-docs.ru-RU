---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
localization_priority: Normal
ms.openlocfilehash: d1f3df6a88ab688206d26db6fc0afe1e1d4a4f60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852999"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="fa47c-103">Тип ресурса assignedPlan</span><span class="sxs-lookup"><span data-stu-id="fa47c-103">assignedPlan resource type</span></span>

<span data-ttu-id="fa47c-104">Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="fa47c-104">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="fa47c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa47c-105">Properties</span></span>
| <span data-ttu-id="fa47c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa47c-106">Property</span></span>     | <span data-ttu-id="fa47c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fa47c-107">Type</span></span>   |<span data-ttu-id="fa47c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fa47c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa47c-109">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa47c-109">assignedDateTime</span></span>|<span data-ttu-id="fa47c-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa47c-110">DateTimeOffset</span></span>|<span data-ttu-id="fa47c-p101">Дата и время назначения плана. Пример: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fa47c-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fa47c-114">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="fa47c-114">capabilityStatus</span></span>|<span data-ttu-id="fa47c-115">String</span><span class="sxs-lookup"><span data-stu-id="fa47c-115">String</span></span>|<span data-ttu-id="fa47c-116">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="fa47c-116">For example, “Enabled”.</span></span>|
|<span data-ttu-id="fa47c-117">service</span><span class="sxs-lookup"><span data-stu-id="fa47c-117">service</span></span>|<span data-ttu-id="fa47c-118">String</span><span class="sxs-lookup"><span data-stu-id="fa47c-118">String</span></span>|<span data-ttu-id="fa47c-119">Имя службы, например "Exchange".</span><span class="sxs-lookup"><span data-stu-id="fa47c-119">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="fa47c-120">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="fa47c-120">servicePlanId</span></span>|<span data-ttu-id="fa47c-121">Guid</span><span class="sxs-lookup"><span data-stu-id="fa47c-121">Guid</span></span>|<span data-ttu-id="fa47c-122">Идентификатор GUID, определяющий план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="fa47c-122">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa47c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa47c-123">JSON representation</span></span>

<span data-ttu-id="fa47c-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa47c-124">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
