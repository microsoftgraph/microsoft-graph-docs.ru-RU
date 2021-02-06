---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: krbain
ms.openlocfilehash: 7cb9aeeca6ad1838ede8395ab270cf10f84faa5f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130923"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="543d4-103">Тип ресурса assignedPlan</span><span class="sxs-lookup"><span data-stu-id="543d4-103">assignedPlan resource type</span></span>

<span data-ttu-id="543d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="543d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="543d4-105">Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="543d4-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="543d4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="543d4-106">Properties</span></span>

| <span data-ttu-id="543d4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="543d4-107">Property</span></span>     | <span data-ttu-id="543d4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="543d4-108">Type</span></span>   |<span data-ttu-id="543d4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="543d4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="543d4-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="543d4-110">assignedDateTime</span></span>|<span data-ttu-id="543d4-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="543d4-111">DateTimeOffset</span></span>|<span data-ttu-id="543d4-p101">Дата и время назначения плана. Пример: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="543d4-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="543d4-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="543d4-115">capabilityStatus</span></span>|[<span data-ttu-id="543d4-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="543d4-116">capabilityStatus</span></span>](#capabilitystatus-values)|<span data-ttu-id="543d4-117">Условие назначения возможности.</span><span class="sxs-lookup"><span data-stu-id="543d4-117">Condition of the capability assignment.</span></span> <span data-ttu-id="543d4-118">Возможные значения: `Enabled` `Warning` , , , `Suspended` `Deleted` `LockedOut` .</span><span class="sxs-lookup"><span data-stu-id="543d4-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span>|
|<span data-ttu-id="543d4-119">service</span><span class="sxs-lookup"><span data-stu-id="543d4-119">service</span></span>|<span data-ttu-id="543d4-120">String</span><span class="sxs-lookup"><span data-stu-id="543d4-120">String</span></span>|<span data-ttu-id="543d4-121">Имя службы, например "Exchange".</span><span class="sxs-lookup"><span data-stu-id="543d4-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="543d4-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="543d4-122">servicePlanId</span></span>|<span data-ttu-id="543d4-123">Guid</span><span class="sxs-lookup"><span data-stu-id="543d4-123">Guid</span></span>|<span data-ttu-id="543d4-124">Идентификатор GUID, определяющий план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="543d4-124">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="543d4-125">значения capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="543d4-125">capabilityStatus values</span></span>

| <span data-ttu-id="543d4-126">Member</span><span class="sxs-lookup"><span data-stu-id="543d4-126">Member</span></span> | <span data-ttu-id="543d4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="543d4-127">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="543d4-128">Включен</span><span class="sxs-lookup"><span data-stu-id="543d4-128">Enabled</span></span> | <span data-ttu-id="543d4-129">Доступно для обычного использования.</span><span class="sxs-lookup"><span data-stu-id="543d4-129">Available for normal use.</span></span> |
| <span data-ttu-id="543d4-130">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="543d4-130">Warning</span></span> | <span data-ttu-id="543d4-131">Доступно для обычного использования, но находится в льготном периоде.</span><span class="sxs-lookup"><span data-stu-id="543d4-131">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="543d4-132">Suspended</span><span class="sxs-lookup"><span data-stu-id="543d4-132">Suspended</span></span> | <span data-ttu-id="543d4-133">Недоступно, но все данные, связанные с возможностью, должны быть сохранены.</span><span class="sxs-lookup"><span data-stu-id="543d4-133">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="543d4-134">Deleted</span><span class="sxs-lookup"><span data-stu-id="543d4-134">Deleted</span></span> | <span data-ttu-id="543d4-135">Недоступны и любые данные, связанные с возможностью, могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="543d4-135">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="543d4-136">LockedOut</span><span class="sxs-lookup"><span data-stu-id="543d4-136">LockedOut</span></span> | <span data-ttu-id="543d4-137">Недоступно для всех администраторов и пользователей, но все данные, связанные с возможностью, должны быть сохранены.</span><span class="sxs-lookup"><span data-stu-id="543d4-137">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="543d4-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="543d4-138">JSON representation</span></span>

<span data-ttu-id="543d4-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="543d4-139">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->


