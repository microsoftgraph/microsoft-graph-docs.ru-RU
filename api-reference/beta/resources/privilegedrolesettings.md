---
title: Тип ресурса privilegedRoleSettings
description: Представляет параметры привилегированной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: efc04b9b65719cbd5952dffb545d371172ab95eb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137636"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="77b58-103">Тип ресурса privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="77b58-103">privilegedRoleSettings resource type</span></span>

<span data-ttu-id="77b58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77b58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77b58-105">Представляет параметры привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-105">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="77b58-106">Методы</span><span class="sxs-lookup"><span data-stu-id="77b58-106">Methods</span></span>

| <span data-ttu-id="77b58-107">Метод</span><span class="sxs-lookup"><span data-stu-id="77b58-107">Method</span></span>           | <span data-ttu-id="77b58-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77b58-108">Return Type</span></span>    |<span data-ttu-id="77b58-109">Описание</span><span class="sxs-lookup"><span data-stu-id="77b58-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77b58-110">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="77b58-110">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="77b58-111">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="77b58-111">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="77b58-112">Чтение свойств и связей объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="77b58-112">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="77b58-113">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="77b58-113">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="77b58-114">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="77b58-114">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="77b58-115">Обновление объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="77b58-115">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="77b58-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="77b58-116">Properties</span></span>
| <span data-ttu-id="77b58-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="77b58-117">Property</span></span>     | <span data-ttu-id="77b58-118">Тип</span><span class="sxs-lookup"><span data-stu-id="77b58-118">Type</span></span>   |<span data-ttu-id="77b58-119">Описание</span><span class="sxs-lookup"><span data-stu-id="77b58-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77b58-120">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="77b58-120">elevationDuration</span></span>|<span data-ttu-id="77b58-121">duration</span><span class="sxs-lookup"><span data-stu-id="77b58-121">duration</span></span>|<span data-ttu-id="77b58-122">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-122">The duration when the role is activated.</span></span>|
|<span data-ttu-id="77b58-123">id</span><span class="sxs-lookup"><span data-stu-id="77b58-123">id</span></span>|<span data-ttu-id="77b58-124">string</span><span class="sxs-lookup"><span data-stu-id="77b58-124">string</span></span>| <span data-ttu-id="77b58-125">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-125">The unique identifier for the role settings.</span></span> <span data-ttu-id="77b58-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77b58-126">Read-only.</span></span>|
|<span data-ttu-id="77b58-127">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="77b58-127">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="77b58-128">boolean</span><span class="sxs-lookup"><span data-stu-id="77b58-128">boolean</span></span>|<span data-ttu-id="77b58-129">**true,** если mfaOnElevation настраивается.</span><span class="sxs-lookup"><span data-stu-id="77b58-129">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="77b58-130">**false,** если mfaOnElevation не настраивается.</span><span class="sxs-lookup"><span data-stu-id="77b58-130">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="77b58-131">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="77b58-131">lastGlobalAdmin</span></span>|<span data-ttu-id="77b58-132">boolean</span><span class="sxs-lookup"><span data-stu-id="77b58-132">boolean</span></span>|<span data-ttu-id="77b58-133">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="77b58-133">Internal used only.</span></span>|
|<span data-ttu-id="77b58-134">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="77b58-134">maxElavationDuration</span></span>|<span data-ttu-id="77b58-135">duration</span><span class="sxs-lookup"><span data-stu-id="77b58-135">duration</span></span>|<span data-ttu-id="77b58-136">Максимальная длительность активированной роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-136">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="77b58-137">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="77b58-137">mfaOnElevation</span></span>|<span data-ttu-id="77b58-138">boolean</span><span class="sxs-lookup"><span data-stu-id="77b58-138">boolean</span></span>|<span data-ttu-id="77b58-139">**имеет значение true,** если для активации роли требуется многофаксная активация.</span><span class="sxs-lookup"><span data-stu-id="77b58-139">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="77b58-140">**false,** если MFA не требуется для активации роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-140">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="77b58-141">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="77b58-141">minElevationDuration</span></span>|<span data-ttu-id="77b58-142">duration</span><span class="sxs-lookup"><span data-stu-id="77b58-142">duration</span></span>|<span data-ttu-id="77b58-143">Минимальная длительность активированной роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-143">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="77b58-144">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="77b58-144">notificationToUserOnElevation</span></span>|<span data-ttu-id="77b58-145">boolean</span><span class="sxs-lookup"><span data-stu-id="77b58-145">boolean</span></span>|<span data-ttu-id="77b58-146">имеет значение **true,** если при активации роли пользователю отправляется уведомление.</span><span class="sxs-lookup"><span data-stu-id="77b58-146">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="77b58-147">**false,** если не отправлять уведомление при активации роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-147">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="77b58-148">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="77b58-148">ticketingInfoOnElevation</span></span>|<span data-ttu-id="77b58-149">boolean</span><span class="sxs-lookup"><span data-stu-id="77b58-149">boolean</span></span>|<span data-ttu-id="77b58-150">имеет значение **true,** если при активации роли требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="77b58-150">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="77b58-151">**false,** если сведения о билетах не требуются при активации роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-151">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="77b58-152">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="77b58-152">approvalOnElevation</span></span>|<span data-ttu-id="77b58-153">boolean</span><span class="sxs-lookup"><span data-stu-id="77b58-153">boolean</span></span>|<span data-ttu-id="77b58-154">имеет значение **true,** если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-154">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="77b58-155">**false,** если утверждение не требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="77b58-155">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="77b58-156">approverIds</span><span class="sxs-lookup"><span data-stu-id="77b58-156">approverIds</span></span>| <span data-ttu-id="77b58-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="77b58-157">string collection</span></span> |<span data-ttu-id="77b58-158">Список ид утверждения, если для активации требуется утверждение.</span><span class="sxs-lookup"><span data-stu-id="77b58-158">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77b58-159">Связи</span><span class="sxs-lookup"><span data-stu-id="77b58-159">Relationships</span></span>
<span data-ttu-id="77b58-160">Нет</span><span class="sxs-lookup"><span data-stu-id="77b58-160">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="77b58-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77b58-161">JSON representation</span></span>

<span data-ttu-id="77b58-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77b58-162">Here is a JSON representation of the resource.</span></span>

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


