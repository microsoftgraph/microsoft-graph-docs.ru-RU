---
title: тип ресурса privilegedRoleSettings
description: Представляет параметры привилегированной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a1f20455ffcc818aa1b1edf784d6990d68b7556b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962570"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="8b74f-103">тип ресурса privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8b74f-103">privilegedRoleSettings resource type</span></span>

<span data-ttu-id="8b74f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b74f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b74f-105">Представляет параметры привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-105">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="8b74f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8b74f-106">Methods</span></span>

| <span data-ttu-id="8b74f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8b74f-107">Method</span></span>           | <span data-ttu-id="8b74f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8b74f-108">Return Type</span></span>    |<span data-ttu-id="8b74f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8b74f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b74f-110">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8b74f-110">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="8b74f-111">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8b74f-111">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="8b74f-112">Чтение свойств и связей объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="8b74f-112">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="8b74f-113">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8b74f-113">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="8b74f-114">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="8b74f-114">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="8b74f-115">Обновление объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="8b74f-115">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="8b74f-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b74f-116">Properties</span></span>
| <span data-ttu-id="8b74f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b74f-117">Property</span></span>     | <span data-ttu-id="8b74f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8b74f-118">Type</span></span>   |<span data-ttu-id="8b74f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8b74f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b74f-120">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="8b74f-120">elevationDuration</span></span>|<span data-ttu-id="8b74f-121">duration</span><span class="sxs-lookup"><span data-stu-id="8b74f-121">duration</span></span>|<span data-ttu-id="8b74f-122">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-122">The duration when the role is activated.</span></span>|
|<span data-ttu-id="8b74f-123">id</span><span class="sxs-lookup"><span data-stu-id="8b74f-123">id</span></span>|<span data-ttu-id="8b74f-124">string</span><span class="sxs-lookup"><span data-stu-id="8b74f-124">string</span></span>| <span data-ttu-id="8b74f-125">Уникальный идентификатор параметров ролей.</span><span class="sxs-lookup"><span data-stu-id="8b74f-125">The unique identifier for the role settings.</span></span> <span data-ttu-id="8b74f-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b74f-126">Read-only.</span></span>|
|<span data-ttu-id="8b74f-127">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="8b74f-127">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="8b74f-128">boolean</span><span class="sxs-lookup"><span data-stu-id="8b74f-128">boolean</span></span>|<span data-ttu-id="8b74f-129">`true` если **mfaOnElevation** настраивается.</span><span class="sxs-lookup"><span data-stu-id="8b74f-129">`true` if **mfaOnElevation** is configurable.</span></span> <span data-ttu-id="8b74f-130">`false` если **mfaOnElevation** не настраивается.</span><span class="sxs-lookup"><span data-stu-id="8b74f-130">`false` if **mfaOnElevation** is not configurable.</span></span>|
|<span data-ttu-id="8b74f-131">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="8b74f-131">lastGlobalAdmin</span></span>|<span data-ttu-id="8b74f-132">boolean</span><span class="sxs-lookup"><span data-stu-id="8b74f-132">boolean</span></span>|<span data-ttu-id="8b74f-133">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="8b74f-133">Internal used only.</span></span>|
|<span data-ttu-id="8b74f-134">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="8b74f-134">maxElavationDuration</span></span>|<span data-ttu-id="8b74f-135">duration</span><span class="sxs-lookup"><span data-stu-id="8b74f-135">duration</span></span>|<span data-ttu-id="8b74f-136">Максимальная продолжительность для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-136">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="8b74f-137">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="8b74f-137">mfaOnElevation</span></span>|<span data-ttu-id="8b74f-138">boolean</span><span class="sxs-lookup"><span data-stu-id="8b74f-138">boolean</span></span>|<span data-ttu-id="8b74f-139">`true` если для активации роли требуется MFA.</span><span class="sxs-lookup"><span data-stu-id="8b74f-139">`true` if MFA is required to activate the role.</span></span> <span data-ttu-id="8b74f-140">`false` если MFA не требуется активировать роль.</span><span class="sxs-lookup"><span data-stu-id="8b74f-140">`false` if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="8b74f-141">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="8b74f-141">minElevationDuration</span></span>|<span data-ttu-id="8b74f-142">duration</span><span class="sxs-lookup"><span data-stu-id="8b74f-142">duration</span></span>|<span data-ttu-id="8b74f-143">Минимальная продолжительность для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-143">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="8b74f-144">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="8b74f-144">notificationToUserOnElevation</span></span>|<span data-ttu-id="8b74f-145">boolean</span><span class="sxs-lookup"><span data-stu-id="8b74f-145">boolean</span></span>|<span data-ttu-id="8b74f-146">`true` при отправке уведомления конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-146">`true` if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="8b74f-147">`false` если не отправлять уведомления при активации роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-147">`false` if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="8b74f-148">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="8b74f-148">ticketingInfoOnElevation</span></span>|<span data-ttu-id="8b74f-149">boolean</span><span class="sxs-lookup"><span data-stu-id="8b74f-149">boolean</span></span>|<span data-ttu-id="8b74f-150">`true` если при активации роли требуется информация о билетах.</span><span class="sxs-lookup"><span data-stu-id="8b74f-150">`true` if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="8b74f-151">`false` если сведения о билетах не требуются при активации роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-151">`false` if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="8b74f-152">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="8b74f-152">approvalOnElevation</span></span>|<span data-ttu-id="8b74f-153">boolean</span><span class="sxs-lookup"><span data-stu-id="8b74f-153">boolean</span></span>|<span data-ttu-id="8b74f-154">`true` если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-154">`true` if the approval is required when activate the role.</span></span> <span data-ttu-id="8b74f-155">`false` если утверждение не требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="8b74f-155">`false` if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="8b74f-156">approverIds</span><span class="sxs-lookup"><span data-stu-id="8b74f-156">approverIds</span></span>| <span data-ttu-id="8b74f-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8b74f-157">string collection</span></span> |<span data-ttu-id="8b74f-158">Список ids утверждения, если требуется утверждение для активации.</span><span class="sxs-lookup"><span data-stu-id="8b74f-158">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b74f-159">Связи</span><span class="sxs-lookup"><span data-stu-id="8b74f-159">Relationships</span></span>
<span data-ttu-id="8b74f-160">Нет</span><span class="sxs-lookup"><span data-stu-id="8b74f-160">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8b74f-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b74f-161">JSON representation</span></span>

<span data-ttu-id="8b74f-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b74f-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


