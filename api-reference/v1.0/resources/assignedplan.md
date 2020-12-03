---
title: Тип ресурса assignedPlan
description: Свойство **assignedPlans** объектов user и organization представляет собой коллекцию объектов **assignedPlan**.
localization_priority: Normal
author: krbain
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ea10e7894b91fd6bf23625c6c3c0097fbe9ed09
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563767"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="6dbbb-103">Тип ресурса assignedPlan</span><span class="sxs-lookup"><span data-stu-id="6dbbb-103">assignedPlan resource type</span></span>

<span data-ttu-id="6dbbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dbbb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6dbbb-105">Свойство **assignedPlans** объектов [user](user.md) и [organization](organization.md) представляет собой коллекцию объектов **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-105">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="6dbbb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6dbbb-106">Properties</span></span>

| <span data-ttu-id="6dbbb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6dbbb-107">Property</span></span>     | <span data-ttu-id="6dbbb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6dbbb-108">Type</span></span>   |<span data-ttu-id="6dbbb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6dbbb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dbbb-110">ассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="6dbbb-110">assignedDateTime</span></span>|<span data-ttu-id="6dbbb-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dbbb-111">DateTimeOffset</span></span>|<span data-ttu-id="6dbbb-p101">Дата и время назначения плана. Пример: 2013-01-02T19:32:30Z. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6dbbb-115">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="6dbbb-115">capabilityStatus</span></span>|[<span data-ttu-id="6dbbb-116">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="6dbbb-116">capabilityStatus</span></span>](#capabilitystatus-values)|<span data-ttu-id="6dbbb-117">Условие назначения возможности.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-117">Condition of the capability assignment.</span></span> <span data-ttu-id="6dbbb-118">Возможные значения:,,, `Enabled` `Warning` `Suspended` `Deleted` , `LockedOut` .</span><span class="sxs-lookup"><span data-stu-id="6dbbb-118">The possible values are `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span>|
|<span data-ttu-id="6dbbb-119">service</span><span class="sxs-lookup"><span data-stu-id="6dbbb-119">service</span></span>|<span data-ttu-id="6dbbb-120">String</span><span class="sxs-lookup"><span data-stu-id="6dbbb-120">String</span></span>|<span data-ttu-id="6dbbb-121">Имя службы, например "Exchange".</span><span class="sxs-lookup"><span data-stu-id="6dbbb-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="6dbbb-122">сервицепланид</span><span class="sxs-lookup"><span data-stu-id="6dbbb-122">servicePlanId</span></span>|<span data-ttu-id="6dbbb-123">Guid</span><span class="sxs-lookup"><span data-stu-id="6dbbb-123">Guid</span></span>|<span data-ttu-id="6dbbb-124">Идентификатор GUID, определяющий план обслуживания.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-124">A GUID that identifies the service plan.</span></span>|


### <a name="capabilitystatus-values"></a><span data-ttu-id="6dbbb-125">значения Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="6dbbb-125">capabilityStatus values</span></span>

| <span data-ttu-id="6dbbb-126">Member</span><span class="sxs-lookup"><span data-stu-id="6dbbb-126">Member</span></span> | <span data-ttu-id="6dbbb-127">Описание</span><span class="sxs-lookup"><span data-stu-id="6dbbb-127">Description</span></span>  |
|:---------------|:--------|
| <span data-ttu-id="6dbbb-128">Включено</span><span class="sxs-lookup"><span data-stu-id="6dbbb-128">Enabled</span></span> | <span data-ttu-id="6dbbb-129">Доступен для обычного использования.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-129">Available for normal use.</span></span> |
| <span data-ttu-id="6dbbb-130">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="6dbbb-130">Warning</span></span> | <span data-ttu-id="6dbbb-131">Доступен для нормального использования, но находится в периоде отсрочки.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-131">Available for normal use but is in a grace period.</span></span> |
| <span data-ttu-id="6dbbb-132">Suspended</span><span class="sxs-lookup"><span data-stu-id="6dbbb-132">Suspended</span></span> | <span data-ttu-id="6dbbb-133">Недоступно, но все данные, связанные с возможностью, должны быть сохранены.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-133">Unavailable but any data associated with the capability must be preserved.</span></span> |
| <span data-ttu-id="6dbbb-134">Deleted</span><span class="sxs-lookup"><span data-stu-id="6dbbb-134">Deleted</span></span> | <span data-ttu-id="6dbbb-135">Все данные, связанные с возможностью, недоступны и могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-135">Unavailable and any data associated with the capability may be deleted.</span></span> |
| <span data-ttu-id="6dbbb-136">Блокировка</span><span class="sxs-lookup"><span data-stu-id="6dbbb-136">LockedOut</span></span> | <span data-ttu-id="6dbbb-137">Недоступно для всех администраторов и пользователей, но все данные, связанные с этой возможностью, должны быть сохранены.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-137">Unavailable for all administrators and users but any data associated with the capability must be preserved.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6dbbb-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6dbbb-138">JSON representation</span></span>

<span data-ttu-id="6dbbb-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6dbbb-139">Here is a JSON representation of the resource</span></span>

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

