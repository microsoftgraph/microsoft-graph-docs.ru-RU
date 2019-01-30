---
title: Тип ресурса privilegedRoleSettings
description: Представляет параметры для привилегированной роли.
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642781"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="6fe20-103">Тип ресурса privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6fe20-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fe20-104">Представляет параметры для привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="6fe20-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6fe20-105">Methods</span></span>

| <span data-ttu-id="6fe20-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6fe20-106">Method</span></span>           | <span data-ttu-id="6fe20-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6fe20-107">Return Type</span></span>    |<span data-ttu-id="6fe20-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6fe20-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6fe20-109">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6fe20-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="6fe20-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6fe20-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="6fe20-111">Чтение свойства и связи объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="6fe20-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="6fe20-112">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6fe20-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="6fe20-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6fe20-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="6fe20-114">Обновление объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="6fe20-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="6fe20-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fe20-115">Properties</span></span>
| <span data-ttu-id="6fe20-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fe20-116">Property</span></span>     | <span data-ttu-id="6fe20-117">Тип</span><span class="sxs-lookup"><span data-stu-id="6fe20-117">Type</span></span>   |<span data-ttu-id="6fe20-118">Описание</span><span class="sxs-lookup"><span data-stu-id="6fe20-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fe20-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="6fe20-119">elevationDuration</span></span>|<span data-ttu-id="6fe20-120">duration</span><span class="sxs-lookup"><span data-stu-id="6fe20-120">duration</span></span>|<span data-ttu-id="6fe20-121">Длительность, при активации роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="6fe20-122">id</span><span class="sxs-lookup"><span data-stu-id="6fe20-122">id</span></span>|<span data-ttu-id="6fe20-123">строка</span><span class="sxs-lookup"><span data-stu-id="6fe20-123">string</span></span>| <span data-ttu-id="6fe20-124">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="6fe20-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6fe20-125">Read-only.</span></span>|
|<span data-ttu-id="6fe20-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="6fe20-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="6fe20-127">boolean</span><span class="sxs-lookup"><span data-stu-id="6fe20-127">boolean</span></span>|<span data-ttu-id="6fe20-128">**значение true,** Если mfaOnElevation может быть настроен.</span><span class="sxs-lookup"><span data-stu-id="6fe20-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="6fe20-129">**значение false,** Если mfaOnElevation не настраивается.</span><span class="sxs-lookup"><span data-stu-id="6fe20-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="6fe20-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="6fe20-130">lastGlobalAdmin</span></span>|<span data-ttu-id="6fe20-131">boolean</span><span class="sxs-lookup"><span data-stu-id="6fe20-131">boolean</span></span>|<span data-ttu-id="6fe20-132">Для внутреннего использования используется только.</span><span class="sxs-lookup"><span data-stu-id="6fe20-132">Internal used only.</span></span>|
|<span data-ttu-id="6fe20-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="6fe20-133">maxElavationDuration</span></span>|<span data-ttu-id="6fe20-134">duration</span><span class="sxs-lookup"><span data-stu-id="6fe20-134">duration</span></span>|<span data-ttu-id="6fe20-135">Максимальной длительности для активации роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="6fe20-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="6fe20-136">mfaOnElevation</span></span>|<span data-ttu-id="6fe20-137">boolean</span><span class="sxs-lookup"><span data-stu-id="6fe20-137">boolean</span></span>|<span data-ttu-id="6fe20-138">**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="6fe20-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="6fe20-139">**значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="6fe20-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="6fe20-140">minElevationDuration</span></span>|<span data-ttu-id="6fe20-141">duration</span><span class="sxs-lookup"><span data-stu-id="6fe20-141">duration</span></span>|<span data-ttu-id="6fe20-142">Минимальная продолжительность активированные роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="6fe20-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="6fe20-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="6fe20-144">boolean</span><span class="sxs-lookup"><span data-stu-id="6fe20-144">boolean</span></span>|<span data-ttu-id="6fe20-145">**значение true,** Если отправить уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="6fe20-146">**значение false,** Если не отправлять уведомления при активации роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="6fe20-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="6fe20-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="6fe20-148">boolean</span><span class="sxs-lookup"><span data-stu-id="6fe20-148">boolean</span></span>|<span data-ttu-id="6fe20-149">**значение true,** Если отдела сведения требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="6fe20-150">**значение false,** Если отдела сведения не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="6fe20-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="6fe20-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="6fe20-151">approvalOnElevation</span></span>|<span data-ttu-id="6fe20-152">boolean</span><span class="sxs-lookup"><span data-stu-id="6fe20-152">boolean</span></span>|<span data-ttu-id="6fe20-153">**значение true,** Если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="6fe20-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="6fe20-154">**значение false,** Если утверждение не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="6fe20-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="6fe20-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="6fe20-155">approverIds</span></span>|<span data-ttu-id="6fe20-156">array</span><span class="sxs-lookup"><span data-stu-id="6fe20-156">array</span></span>|<span data-ttu-id="6fe20-157">Список идентификаторов утверждения, если требуется для активации утверждение.</span><span class="sxs-lookup"><span data-stu-id="6fe20-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fe20-158">Связи</span><span class="sxs-lookup"><span data-stu-id="6fe20-158">Relationships</span></span>
<span data-ttu-id="6fe20-159">Нет</span><span class="sxs-lookup"><span data-stu-id="6fe20-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6fe20-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fe20-160">JSON representation</span></span>

<span data-ttu-id="6fe20-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fe20-161">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
