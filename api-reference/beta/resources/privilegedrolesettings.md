---
title: Тип ресурса Привилежедролесеттингс
description: Представляет параметры привилегированной роли.
localization_priority: Normal
ms.openlocfilehash: 6500d5a51fcedce97d71c1c4022c7d941de27b83
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344232"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="27bdd-103">Тип ресурса Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="27bdd-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27bdd-104">Представляет параметры привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="27bdd-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="27bdd-105">Методы</span><span class="sxs-lookup"><span data-stu-id="27bdd-105">Methods</span></span>

| <span data-ttu-id="27bdd-106">Метод</span><span class="sxs-lookup"><span data-stu-id="27bdd-106">Method</span></span>           | <span data-ttu-id="27bdd-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27bdd-107">Return Type</span></span>    |<span data-ttu-id="27bdd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27bdd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27bdd-109">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="27bdd-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="27bdd-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="27bdd-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="27bdd-111">Чтение свойств и связей объекта Привилежедролесеттингс.</span><span class="sxs-lookup"><span data-stu-id="27bdd-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="27bdd-112">Обновление Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="27bdd-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="27bdd-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="27bdd-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="27bdd-114">Обновление объекта Привилежедролесеттингс.</span><span class="sxs-lookup"><span data-stu-id="27bdd-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="27bdd-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="27bdd-115">Properties</span></span>
| <span data-ttu-id="27bdd-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="27bdd-116">Property</span></span>     | <span data-ttu-id="27bdd-117">Тип</span><span class="sxs-lookup"><span data-stu-id="27bdd-117">Type</span></span>   |<span data-ttu-id="27bdd-118">Описание</span><span class="sxs-lookup"><span data-stu-id="27bdd-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27bdd-119">Елеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="27bdd-119">elevationDuration</span></span>|<span data-ttu-id="27bdd-120">duration</span><span class="sxs-lookup"><span data-stu-id="27bdd-120">duration</span></span>|<span data-ttu-id="27bdd-121">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="27bdd-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="27bdd-122">id</span><span class="sxs-lookup"><span data-stu-id="27bdd-122">id</span></span>|<span data-ttu-id="27bdd-123">string</span><span class="sxs-lookup"><span data-stu-id="27bdd-123">string</span></span>| <span data-ttu-id="27bdd-124">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="27bdd-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="27bdd-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27bdd-125">Read-only.</span></span>|
|<span data-ttu-id="27bdd-126">Исмфаонелеватионконфигурабле</span><span class="sxs-lookup"><span data-stu-id="27bdd-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="27bdd-127">boolean</span><span class="sxs-lookup"><span data-stu-id="27bdd-127">boolean</span></span>|<span data-ttu-id="27bdd-128">**значение true** , если мфаонелеватион является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="27bdd-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="27bdd-129">**false** , если мфаонелеватион не является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="27bdd-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="27bdd-130">Ластглобаладмин</span><span class="sxs-lookup"><span data-stu-id="27bdd-130">lastGlobalAdmin</span></span>|<span data-ttu-id="27bdd-131">boolean</span><span class="sxs-lookup"><span data-stu-id="27bdd-131">boolean</span></span>|<span data-ttu-id="27bdd-132">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="27bdd-132">Internal used only.</span></span>|
|<span data-ttu-id="27bdd-133">Макселаватиондуратион</span><span class="sxs-lookup"><span data-stu-id="27bdd-133">maxElavationDuration</span></span>|<span data-ttu-id="27bdd-134">duration</span><span class="sxs-lookup"><span data-stu-id="27bdd-134">duration</span></span>|<span data-ttu-id="27bdd-135">Максимальный срок для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="27bdd-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="27bdd-136">Мфаонелеватион</span><span class="sxs-lookup"><span data-stu-id="27bdd-136">mfaOnElevation</span></span>|<span data-ttu-id="27bdd-137">boolean</span><span class="sxs-lookup"><span data-stu-id="27bdd-137">boolean</span></span>|<span data-ttu-id="27bdd-138">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="27bdd-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="27bdd-139">**false** , если MFA не требуется для активации роли.</span><span class="sxs-lookup"><span data-stu-id="27bdd-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="27bdd-140">Минелеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="27bdd-140">minElevationDuration</span></span>|<span data-ttu-id="27bdd-141">duration</span><span class="sxs-lookup"><span data-stu-id="27bdd-141">duration</span></span>|<span data-ttu-id="27bdd-142">Минимальная длительность для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="27bdd-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="27bdd-143">Нотификатионтаусеронелеватион</span><span class="sxs-lookup"><span data-stu-id="27bdd-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="27bdd-144">boolean</span><span class="sxs-lookup"><span data-stu-id="27bdd-144">boolean</span></span>|<span data-ttu-id="27bdd-145">**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="27bdd-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="27bdd-146">**значение false** , если уведомление не отправляется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="27bdd-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="27bdd-147">Тиккетингинфунелеватион</span><span class="sxs-lookup"><span data-stu-id="27bdd-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="27bdd-148">boolean</span><span class="sxs-lookup"><span data-stu-id="27bdd-148">boolean</span></span>|<span data-ttu-id="27bdd-149">**имеет значение true** , если при активации роли требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="27bdd-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="27bdd-150">**false** , если при активации роли не требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="27bdd-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="27bdd-151">Аппровалонелеватион</span><span class="sxs-lookup"><span data-stu-id="27bdd-151">approvalOnElevation</span></span>|<span data-ttu-id="27bdd-152">boolean</span><span class="sxs-lookup"><span data-stu-id="27bdd-152">boolean</span></span>|<span data-ttu-id="27bdd-153">**имеет значение true** , если при активации роли необходимо выполнить утверждение.</span><span class="sxs-lookup"><span data-stu-id="27bdd-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="27bdd-154">**false** , если при активации роли не нужно утверждать.</span><span class="sxs-lookup"><span data-stu-id="27bdd-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="27bdd-155">Аппроверидс</span><span class="sxs-lookup"><span data-stu-id="27bdd-155">approverIds</span></span>| <span data-ttu-id="27bdd-156">string collection</span><span class="sxs-lookup"><span data-stu-id="27bdd-156">string collection</span></span> |<span data-ttu-id="27bdd-157">Список идентификаторов утверждения, если для активации необходимо утверждение.</span><span class="sxs-lookup"><span data-stu-id="27bdd-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27bdd-158">Связи</span><span class="sxs-lookup"><span data-stu-id="27bdd-158">Relationships</span></span>
<span data-ttu-id="27bdd-159">Нет</span><span class="sxs-lookup"><span data-stu-id="27bdd-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="27bdd-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27bdd-160">JSON representation</span></span>

<span data-ttu-id="27bdd-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27bdd-161">Here is a JSON representation of the resource.</span></span>

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
