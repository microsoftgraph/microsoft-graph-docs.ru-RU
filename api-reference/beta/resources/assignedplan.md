---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
ms.openlocfilehash: 0df1540819b569b62607bf0e56c1c8f53d2749da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075098"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="6e27f-103">Тип ресурса assignedPlan</span><span class="sxs-lookup"><span data-stu-id="6e27f-103">assignedPlan resource type</span></span>

> <span data-ttu-id="6e27f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e27f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e27f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e27f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e27f-106">Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="6e27f-106">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="6e27f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e27f-107">Properties</span></span>
| <span data-ttu-id="6e27f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e27f-108">Property</span></span>     | <span data-ttu-id="6e27f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e27f-109">Type</span></span>   |<span data-ttu-id="6e27f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e27f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e27f-111">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e27f-111">assignedDateTime</span></span>|<span data-ttu-id="6e27f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e27f-112">DateTimeOffset</span></span>|<span data-ttu-id="6e27f-p102">Дата и время назначения плана. Пример: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6e27f-p102">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6e27f-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="6e27f-116">capabilityStatus</span></span>|<span data-ttu-id="6e27f-117">String</span><span class="sxs-lookup"><span data-stu-id="6e27f-117">String</span></span>|<span data-ttu-id="6e27f-118">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="6e27f-118">For example, “Enabled”.</span></span>|
|<span data-ttu-id="6e27f-119">service</span><span class="sxs-lookup"><span data-stu-id="6e27f-119">service</span></span>|<span data-ttu-id="6e27f-120">String</span><span class="sxs-lookup"><span data-stu-id="6e27f-120">String</span></span>|<span data-ttu-id="6e27f-121">Имя службы, например "Exchange".</span><span class="sxs-lookup"><span data-stu-id="6e27f-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="6e27f-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="6e27f-122">servicePlanId</span></span>|<span data-ttu-id="6e27f-123">Guid</span><span class="sxs-lookup"><span data-stu-id="6e27f-123">Guid</span></span>|<span data-ttu-id="6e27f-124">Идентификатор GUID, определяющий план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="6e27f-124">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e27f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e27f-125">JSON representation</span></span>

<span data-ttu-id="6e27f-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e27f-126">Here is a JSON representation of the resource</span></span>

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
