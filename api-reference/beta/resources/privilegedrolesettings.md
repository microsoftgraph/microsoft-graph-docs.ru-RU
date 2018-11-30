---
title: Тип ресурса privilegedRoleSettings
description: Представляет параметры для привилегированной роли.
ms.openlocfilehash: 14b4919d653de80c97f06aff507c011162c3c0e4
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2018
ms.locfileid: "27082893"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="e446a-103">Тип ресурса privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e446a-103">privilegedRoleSettings resource type</span></span>

> <span data-ttu-id="e446a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e446a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e446a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e446a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e446a-106">Представляет параметры для привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-106">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="e446a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e446a-107">Methods</span></span>

| <span data-ttu-id="e446a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e446a-108">Method</span></span>           | <span data-ttu-id="e446a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e446a-109">Return Type</span></span>    |<span data-ttu-id="e446a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e446a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e446a-111">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e446a-111">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="e446a-112">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e446a-112">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="e446a-113">Чтение свойства и связи объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="e446a-113">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="e446a-114">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e446a-114">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="e446a-115">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e446a-115">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="e446a-116">Обновление объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="e446a-116">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="e446a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="e446a-117">Properties</span></span>
| <span data-ttu-id="e446a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="e446a-118">Property</span></span>     | <span data-ttu-id="e446a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e446a-119">Type</span></span>   |<span data-ttu-id="e446a-120">Description</span><span class="sxs-lookup"><span data-stu-id="e446a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e446a-121">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="e446a-121">elevationDuration</span></span>|<span data-ttu-id="e446a-122">duration</span><span class="sxs-lookup"><span data-stu-id="e446a-122">duration</span></span>|<span data-ttu-id="e446a-123">Длительность, при активации роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-123">The duration when the role is activated.</span></span>|
|<span data-ttu-id="e446a-124">id</span><span class="sxs-lookup"><span data-stu-id="e446a-124">id</span></span>|<span data-ttu-id="e446a-125">строка</span><span class="sxs-lookup"><span data-stu-id="e446a-125">string</span></span>| <span data-ttu-id="e446a-126">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-126">The unique identifier for the role settings.</span></span> <span data-ttu-id="e446a-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e446a-127">Read-only.</span></span>|
|<span data-ttu-id="e446a-128">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="e446a-128">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="e446a-129">boolean</span><span class="sxs-lookup"><span data-stu-id="e446a-129">boolean</span></span>|<span data-ttu-id="e446a-130">**значение true,** Если mfaOnElevation может быть настроен.</span><span class="sxs-lookup"><span data-stu-id="e446a-130">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="e446a-131">**значение false,** Если mfaOnElevation не настраивается.</span><span class="sxs-lookup"><span data-stu-id="e446a-131">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="e446a-132">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="e446a-132">lastGlobalAdmin</span></span>|<span data-ttu-id="e446a-133">boolean</span><span class="sxs-lookup"><span data-stu-id="e446a-133">boolean</span></span>|<span data-ttu-id="e446a-134">Для внутреннего использования используется только.</span><span class="sxs-lookup"><span data-stu-id="e446a-134">Internal used only.</span></span>|
|<span data-ttu-id="e446a-135">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="e446a-135">maxElavationDuration</span></span>|<span data-ttu-id="e446a-136">duration</span><span class="sxs-lookup"><span data-stu-id="e446a-136">duration</span></span>|<span data-ttu-id="e446a-137">Максимальной длительности для активации роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-137">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="e446a-138">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="e446a-138">mfaOnElevation</span></span>|<span data-ttu-id="e446a-139">boolean</span><span class="sxs-lookup"><span data-stu-id="e446a-139">boolean</span></span>|<span data-ttu-id="e446a-140">**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="e446a-140">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="e446a-141">**значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-141">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="e446a-142">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="e446a-142">minElevationDuration</span></span>|<span data-ttu-id="e446a-143">duration</span><span class="sxs-lookup"><span data-stu-id="e446a-143">duration</span></span>|<span data-ttu-id="e446a-144">Минимальная продолжительность активированные роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-144">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="e446a-145">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="e446a-145">notificationToUserOnElevation</span></span>|<span data-ttu-id="e446a-146">boolean</span><span class="sxs-lookup"><span data-stu-id="e446a-146">boolean</span></span>|<span data-ttu-id="e446a-147">**значение true,** Если отправить уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-147">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="e446a-148">**значение false,** Если не отправлять уведомления при активации роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-148">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="e446a-149">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="e446a-149">ticketingInfoOnElevation</span></span>|<span data-ttu-id="e446a-150">boolean</span><span class="sxs-lookup"><span data-stu-id="e446a-150">boolean</span></span>|<span data-ttu-id="e446a-151">**значение true,** Если отдела сведения требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-151">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="e446a-152">**значение false,** Если отдела сведения не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="e446a-152">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="e446a-153">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="e446a-153">approvalOnElevation</span></span>|<span data-ttu-id="e446a-154">boolean</span><span class="sxs-lookup"><span data-stu-id="e446a-154">boolean</span></span>|<span data-ttu-id="e446a-155">**значение true,** Если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="e446a-155">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="e446a-156">**значение false,** Если утверждение не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="e446a-156">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="e446a-157">approverIds</span><span class="sxs-lookup"><span data-stu-id="e446a-157">approverIds</span></span>|<span data-ttu-id="e446a-158">array</span><span class="sxs-lookup"><span data-stu-id="e446a-158">array</span></span>|<span data-ttu-id="e446a-159">Список идентификаторов утверждения, если требуется для активации утверждение.</span><span class="sxs-lookup"><span data-stu-id="e446a-159">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e446a-160">Связи</span><span class="sxs-lookup"><span data-stu-id="e446a-160">Relationships</span></span>
<span data-ttu-id="e446a-161">Нет</span><span class="sxs-lookup"><span data-stu-id="e446a-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e446a-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e446a-162">JSON representation</span></span>

<span data-ttu-id="e446a-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e446a-163">Here is a JSON representation of the resource.</span></span>

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
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->