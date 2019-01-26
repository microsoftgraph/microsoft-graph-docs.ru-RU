---
title: Тип ресурса privilegedRoleSettings
description: Представляет параметры для привилегированной роли.
localization_priority: Normal
ms.openlocfilehash: 673327e3c83a4111eb469ca48550836433dbdf0a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577153"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="9cb0a-103">Тип ресурса privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9cb0a-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cb0a-104">Представляет параметры для привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="9cb0a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9cb0a-105">Methods</span></span>

| <span data-ttu-id="9cb0a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="9cb0a-106">Method</span></span>           | <span data-ttu-id="9cb0a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9cb0a-107">Return Type</span></span>    |<span data-ttu-id="9cb0a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9cb0a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9cb0a-109">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9cb0a-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="9cb0a-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9cb0a-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="9cb0a-111">Чтение свойства и связи объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="9cb0a-112">Обновление privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9cb0a-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="9cb0a-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9cb0a-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="9cb0a-114">Обновление объекта privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="9cb0a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cb0a-115">Properties</span></span>
| <span data-ttu-id="9cb0a-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cb0a-116">Property</span></span>     | <span data-ttu-id="9cb0a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="9cb0a-117">Type</span></span>   |<span data-ttu-id="9cb0a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="9cb0a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cb0a-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="9cb0a-119">elevationDuration</span></span>| <span data-ttu-id="9cb0a-120">String (метка времени)</span><span class="sxs-lookup"><span data-stu-id="9cb0a-120">String (timestamp)</span></span> |<span data-ttu-id="9cb0a-121">Длительность, при активации роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="9cb0a-122">id</span><span class="sxs-lookup"><span data-stu-id="9cb0a-122">id</span></span>| <span data-ttu-id="9cb0a-123">String (идентификатор)</span><span class="sxs-lookup"><span data-stu-id="9cb0a-123">string (identifier)</span></span>| <span data-ttu-id="9cb0a-124">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="9cb0a-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-125">Read-only.</span></span>|
|<span data-ttu-id="9cb0a-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="9cb0a-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="9cb0a-127">boolean</span><span class="sxs-lookup"><span data-stu-id="9cb0a-127">boolean</span></span>|<span data-ttu-id="9cb0a-128">**значение true,** Если mfaOnElevation может быть настроен.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="9cb0a-129">**значение false,** Если mfaOnElevation не настраивается.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="9cb0a-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="9cb0a-130">lastGlobalAdmin</span></span>|<span data-ttu-id="9cb0a-131">boolean</span><span class="sxs-lookup"><span data-stu-id="9cb0a-131">boolean</span></span>|<span data-ttu-id="9cb0a-132">Для внутреннего использования используется только.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-132">Internal used only.</span></span>|
|<span data-ttu-id="9cb0a-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="9cb0a-133">maxElavationDuration</span></span>| <span data-ttu-id="9cb0a-134">String (идентификатор)</span><span class="sxs-lookup"><span data-stu-id="9cb0a-134">string (identifier)</span></span>| |<span data-ttu-id="9cb0a-135">Максимальной длительности для активации роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="9cb0a-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="9cb0a-136">mfaOnElevation</span></span>|<span data-ttu-id="9cb0a-137">boolean</span><span class="sxs-lookup"><span data-stu-id="9cb0a-137">boolean</span></span>|<span data-ttu-id="9cb0a-138">**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="9cb0a-139">**значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="9cb0a-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="9cb0a-140">minElevationDuration</span></span>|<span data-ttu-id="9cb0a-141">String (идентификатор)</span><span class="sxs-lookup"><span data-stu-id="9cb0a-141">string (identifier)</span></span>||<span data-ttu-id="9cb0a-142">Минимальная продолжительность активированные роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="9cb0a-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="9cb0a-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="9cb0a-144">boolean</span><span class="sxs-lookup"><span data-stu-id="9cb0a-144">boolean</span></span>|<span data-ttu-id="9cb0a-145">**значение true,** Если отправить уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="9cb0a-146">**значение false,** Если не отправлять уведомления при активации роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="9cb0a-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="9cb0a-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="9cb0a-148">boolean</span><span class="sxs-lookup"><span data-stu-id="9cb0a-148">boolean</span></span>|<span data-ttu-id="9cb0a-149">**значение true,** Если отдела сведения требуется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="9cb0a-150">**значение false,** Если отдела сведения не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="9cb0a-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="9cb0a-151">approvalOnElevation</span></span>|<span data-ttu-id="9cb0a-152">boolean</span><span class="sxs-lookup"><span data-stu-id="9cb0a-152">boolean</span></span>|<span data-ttu-id="9cb0a-153">**значение true,** Если требуется утверждение при активации роли.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="9cb0a-154">**значение false,** Если утверждение не является обязательным, когда активировать роль.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="9cb0a-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="9cb0a-155">approverIds</span></span>| <span data-ttu-id="9cb0a-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9cb0a-156">String collection</span></span> |<span data-ttu-id="9cb0a-157">Список идентификаторов утверждения, если требуется для активации утверждение.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cb0a-158">Связи</span><span class="sxs-lookup"><span data-stu-id="9cb0a-158">Relationships</span></span>
<span data-ttu-id="9cb0a-159">Нет</span><span class="sxs-lookup"><span data-stu-id="9cb0a-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9cb0a-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cb0a-160">JSON representation</span></span>

<span data-ttu-id="9cb0a-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cb0a-161">Here is a JSON representation of the resource.</span></span>

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
  "approverIds": [ "String (identifier)" ]
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
