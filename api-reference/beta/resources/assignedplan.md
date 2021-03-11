---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: jpettere
ms.openlocfilehash: ddb13f656eda6e17e037a7bcae06b33b41260f8f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721833"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="44c2e-103">Тип ресурса assignedPlan</span><span class="sxs-lookup"><span data-stu-id="44c2e-103">assignedPlan resource type</span></span>

<span data-ttu-id="44c2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44c2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44c2e-105">Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="44c2e-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="44c2e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="44c2e-106">Properties</span></span>

| <span data-ttu-id="44c2e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="44c2e-107">Property</span></span>     | <span data-ttu-id="44c2e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="44c2e-108">Type</span></span>   |<span data-ttu-id="44c2e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="44c2e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44c2e-110">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="44c2e-110">assignedDateTime</span></span>|<span data-ttu-id="44c2e-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44c2e-111">DateTimeOffset</span></span>|<span data-ttu-id="44c2e-112">дата и время, в которые был назначен план; например: 2013-01-02T19:32:30Z.</span><span class="sxs-lookup"><span data-stu-id="44c2e-112">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z.</span></span> <span data-ttu-id="44c2e-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="44c2e-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="44c2e-114">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="44c2e-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="44c2e-115">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="44c2e-115">capabilityStatus</span></span>|[<span data-ttu-id="44c2e-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="44c2e-116">capabilityStatus</span></span>](#capabilitystatus-values)|<span data-ttu-id="44c2e-117">Условие назначения возможностей.</span><span class="sxs-lookup"><span data-stu-id="44c2e-117">Condition of the capability assignment.</span></span> <span data-ttu-id="44c2e-118">Возможные значения `Enabled` , `Warning` `Suspended` , , `Deleted` `LockedOut` .</span><span class="sxs-lookup"><span data-stu-id="44c2e-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span>|
|<span data-ttu-id="44c2e-119">service</span><span class="sxs-lookup"><span data-stu-id="44c2e-119">service</span></span>|<span data-ttu-id="44c2e-120">String</span><span class="sxs-lookup"><span data-stu-id="44c2e-120">String</span></span>|<span data-ttu-id="44c2e-121">Имя службы, например "Exchange".</span><span class="sxs-lookup"><span data-stu-id="44c2e-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="44c2e-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="44c2e-122">servicePlanId</span></span>|<span data-ttu-id="44c2e-123">Guid</span><span class="sxs-lookup"><span data-stu-id="44c2e-123">Guid</span></span>|<span data-ttu-id="44c2e-124">Идентификатор GUID, определяющий план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="44c2e-124">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="44c2e-125">значения capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="44c2e-125">capabilityStatus values</span></span>

| <span data-ttu-id="44c2e-126">Member</span><span class="sxs-lookup"><span data-stu-id="44c2e-126">Member</span></span> | <span data-ttu-id="44c2e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="44c2e-127">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="44c2e-128">Включено</span><span class="sxs-lookup"><span data-stu-id="44c2e-128">Enabled</span></span> | <span data-ttu-id="44c2e-129">Доступно для нормального использования.</span><span class="sxs-lookup"><span data-stu-id="44c2e-129">Available for normal use.</span></span> |
| <span data-ttu-id="44c2e-130">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="44c2e-130">Warning</span></span> | <span data-ttu-id="44c2e-131">Доступно для нормального использования, но находится в льготном периоде.</span><span class="sxs-lookup"><span data-stu-id="44c2e-131">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="44c2e-132">Suspended</span><span class="sxs-lookup"><span data-stu-id="44c2e-132">Suspended</span></span> | <span data-ttu-id="44c2e-133">Недоступны, но все данные, связанные с этой возможностью, должны быть сохранены.</span><span class="sxs-lookup"><span data-stu-id="44c2e-133">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="44c2e-134">Deleted</span><span class="sxs-lookup"><span data-stu-id="44c2e-134">Deleted</span></span> | <span data-ttu-id="44c2e-135">Недоступные и любые данные, связанные с этой возможностью, могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="44c2e-135">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="44c2e-136">LockedOut</span><span class="sxs-lookup"><span data-stu-id="44c2e-136">LockedOut</span></span> | <span data-ttu-id="44c2e-137">Недоступно для всех администраторов и пользователей, но все данные, связанные с этой возможностью, должны быть сохранены.</span><span class="sxs-lookup"><span data-stu-id="44c2e-137">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44c2e-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44c2e-138">JSON representation</span></span>

<span data-ttu-id="44c2e-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44c2e-139">Here is a JSON representation of the resource</span></span>

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


