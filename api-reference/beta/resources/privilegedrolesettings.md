---
title: Тип ресурса Привилежедролесеттингс
description: Представляет параметры привилегированной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c072f75095267910d128396c3848b2decca4728c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521497"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="feee5-103">Тип ресурса Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="feee5-103">privilegedRoleSettings resource type</span></span>

<span data-ttu-id="feee5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feee5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feee5-105">Представляет параметры привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="feee5-105">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="feee5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="feee5-106">Methods</span></span>

| <span data-ttu-id="feee5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="feee5-107">Method</span></span>           | <span data-ttu-id="feee5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="feee5-108">Return Type</span></span>    |<span data-ttu-id="feee5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="feee5-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="feee5-110">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="feee5-110">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="feee5-111">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="feee5-111">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="feee5-112">Чтение свойств и связей объекта Привилежедролесеттингс.</span><span class="sxs-lookup"><span data-stu-id="feee5-112">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="feee5-113">Обновление Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="feee5-113">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="feee5-114">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="feee5-114">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="feee5-115">Обновление объекта Привилежедролесеттингс.</span><span class="sxs-lookup"><span data-stu-id="feee5-115">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="feee5-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="feee5-116">Properties</span></span>
| <span data-ttu-id="feee5-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="feee5-117">Property</span></span>     | <span data-ttu-id="feee5-118">Тип</span><span class="sxs-lookup"><span data-stu-id="feee5-118">Type</span></span>   |<span data-ttu-id="feee5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="feee5-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="feee5-120">елеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="feee5-120">elevationDuration</span></span>|<span data-ttu-id="feee5-121">duration</span><span class="sxs-lookup"><span data-stu-id="feee5-121">duration</span></span>|<span data-ttu-id="feee5-122">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="feee5-122">The duration when the role is activated.</span></span>|
|<span data-ttu-id="feee5-123">id</span><span class="sxs-lookup"><span data-stu-id="feee5-123">id</span></span>|<span data-ttu-id="feee5-124">string</span><span class="sxs-lookup"><span data-stu-id="feee5-124">string</span></span>| <span data-ttu-id="feee5-125">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="feee5-125">The unique identifier for the role settings.</span></span> <span data-ttu-id="feee5-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="feee5-126">Read-only.</span></span>|
|<span data-ttu-id="feee5-127">исмфаонелеватионконфигурабле</span><span class="sxs-lookup"><span data-stu-id="feee5-127">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="feee5-128">boolean</span><span class="sxs-lookup"><span data-stu-id="feee5-128">boolean</span></span>|<span data-ttu-id="feee5-129">**значение true** , если мфаонелеватион является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="feee5-129">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="feee5-130">**false** , если мфаонелеватион не является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="feee5-130">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="feee5-131">ластглобаладмин</span><span class="sxs-lookup"><span data-stu-id="feee5-131">lastGlobalAdmin</span></span>|<span data-ttu-id="feee5-132">boolean</span><span class="sxs-lookup"><span data-stu-id="feee5-132">boolean</span></span>|<span data-ttu-id="feee5-133">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="feee5-133">Internal used only.</span></span>|
|<span data-ttu-id="feee5-134">макселаватиондуратион</span><span class="sxs-lookup"><span data-stu-id="feee5-134">maxElavationDuration</span></span>|<span data-ttu-id="feee5-135">duration</span><span class="sxs-lookup"><span data-stu-id="feee5-135">duration</span></span>|<span data-ttu-id="feee5-136">Максимальный срок для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="feee5-136">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="feee5-137">мфаонелеватион</span><span class="sxs-lookup"><span data-stu-id="feee5-137">mfaOnElevation</span></span>|<span data-ttu-id="feee5-138">boolean</span><span class="sxs-lookup"><span data-stu-id="feee5-138">boolean</span></span>|<span data-ttu-id="feee5-139">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="feee5-139">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="feee5-140">**false** , если MFA не требуется для активации роли.</span><span class="sxs-lookup"><span data-stu-id="feee5-140">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="feee5-141">минелеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="feee5-141">minElevationDuration</span></span>|<span data-ttu-id="feee5-142">duration</span><span class="sxs-lookup"><span data-stu-id="feee5-142">duration</span></span>|<span data-ttu-id="feee5-143">Минимальная длительность для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="feee5-143">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="feee5-144">нотификатионтаусеронелеватион</span><span class="sxs-lookup"><span data-stu-id="feee5-144">notificationToUserOnElevation</span></span>|<span data-ttu-id="feee5-145">boolean</span><span class="sxs-lookup"><span data-stu-id="feee5-145">boolean</span></span>|<span data-ttu-id="feee5-146">**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="feee5-146">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="feee5-147">**значение false** , если уведомление не отправляется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="feee5-147">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="feee5-148">тиккетингинфунелеватион</span><span class="sxs-lookup"><span data-stu-id="feee5-148">ticketingInfoOnElevation</span></span>|<span data-ttu-id="feee5-149">boolean</span><span class="sxs-lookup"><span data-stu-id="feee5-149">boolean</span></span>|<span data-ttu-id="feee5-150">**имеет значение true** , если при активации роли требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="feee5-150">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="feee5-151">**false** , если при активации роли не требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="feee5-151">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="feee5-152">аппровалонелеватион</span><span class="sxs-lookup"><span data-stu-id="feee5-152">approvalOnElevation</span></span>|<span data-ttu-id="feee5-153">boolean</span><span class="sxs-lookup"><span data-stu-id="feee5-153">boolean</span></span>|<span data-ttu-id="feee5-154">**имеет значение true** , если при активации роли необходимо выполнить утверждение.</span><span class="sxs-lookup"><span data-stu-id="feee5-154">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="feee5-155">**false** , если при активации роли не нужно утверждать.</span><span class="sxs-lookup"><span data-stu-id="feee5-155">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="feee5-156">аппроверидс</span><span class="sxs-lookup"><span data-stu-id="feee5-156">approverIds</span></span>| <span data-ttu-id="feee5-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="feee5-157">string collection</span></span> |<span data-ttu-id="feee5-158">Список идентификаторов утверждения, если для активации необходимо утверждение.</span><span class="sxs-lookup"><span data-stu-id="feee5-158">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="feee5-159">Связи</span><span class="sxs-lookup"><span data-stu-id="feee5-159">Relationships</span></span>
<span data-ttu-id="feee5-160">Нет</span><span class="sxs-lookup"><span data-stu-id="feee5-160">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="feee5-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="feee5-161">JSON representation</span></span>

<span data-ttu-id="feee5-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feee5-162">Here is a JSON representation of the resource.</span></span>

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
