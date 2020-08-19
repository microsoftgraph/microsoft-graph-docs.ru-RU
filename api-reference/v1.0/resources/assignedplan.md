---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e4a184a45f1ec385a47fab0e51918949119523b9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808391"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="7e34e-103">Тип ресурса assignedPlan</span><span class="sxs-lookup"><span data-stu-id="7e34e-103">assignedPlan resource type</span></span>

<span data-ttu-id="7e34e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e34e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e34e-105">Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="7e34e-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="7e34e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e34e-106">Properties</span></span>
| <span data-ttu-id="7e34e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e34e-107">Property</span></span>     | <span data-ttu-id="7e34e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7e34e-108">Type</span></span>   |<span data-ttu-id="7e34e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7e34e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e34e-110">ассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="7e34e-110">assignedDateTime</span></span>|<span data-ttu-id="7e34e-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e34e-111">DateTimeOffset</span></span>|<span data-ttu-id="7e34e-p101">Дата и время назначения плана. Пример: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7e34e-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7e34e-115">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="7e34e-115">capabilityStatus</span></span>|<span data-ttu-id="7e34e-116">String</span><span class="sxs-lookup"><span data-stu-id="7e34e-116">String</span></span>|<span data-ttu-id="7e34e-117">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="7e34e-117">For example, “Enabled”.</span></span>|
|<span data-ttu-id="7e34e-118">service</span><span class="sxs-lookup"><span data-stu-id="7e34e-118">service</span></span>|<span data-ttu-id="7e34e-119">String</span><span class="sxs-lookup"><span data-stu-id="7e34e-119">String</span></span>|<span data-ttu-id="7e34e-120">Имя службы, например "Exchange".</span><span class="sxs-lookup"><span data-stu-id="7e34e-120">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="7e34e-121">сервицепланид</span><span class="sxs-lookup"><span data-stu-id="7e34e-121">servicePlanId</span></span>|<span data-ttu-id="7e34e-122">Guid</span><span class="sxs-lookup"><span data-stu-id="7e34e-122">Guid</span></span>|<span data-ttu-id="7e34e-123">Идентификатор GUID, определяющий план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="7e34e-123">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e34e-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7e34e-124">JSON representation</span></span>

<span data-ttu-id="7e34e-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e34e-125">Here is a JSON representation of the resource</span></span>

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
