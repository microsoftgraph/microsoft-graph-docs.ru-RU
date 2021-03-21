---
title: тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, которые регулируются при применяемой политике.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 162943a5f2d51744ae37d6644f8a01eafb31c259
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961295"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="9b753-103">тип ресурса conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="9b753-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="9b753-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b753-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b753-105">Представляет тип условий, которые регулируются при применяемой политике.</span><span class="sxs-lookup"><span data-stu-id="9b753-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="9b753-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b753-106">Properties</span></span>

| <span data-ttu-id="9b753-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b753-107">Property</span></span>     | <span data-ttu-id="9b753-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9b753-108">Type</span></span>        | <span data-ttu-id="9b753-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9b753-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b753-110">приложения</span><span class="sxs-lookup"><span data-stu-id="9b753-110">applications</span></span>|[<span data-ttu-id="9b753-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="9b753-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="9b753-112">Приложения и действия пользователей, включенные и исключенные из политики.</span><span class="sxs-lookup"><span data-stu-id="9b753-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="9b753-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b753-113">Required.</span></span> |
|<span data-ttu-id="9b753-114">users</span><span class="sxs-lookup"><span data-stu-id="9b753-114">users</span></span>|[<span data-ttu-id="9b753-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="9b753-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="9b753-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="9b753-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="9b753-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b753-117">Required.</span></span> |
|<span data-ttu-id="9b753-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="9b753-118">clientAppTypes</span></span>|<span data-ttu-id="9b753-119">коллекция conditionalAccessClientApp</span><span class="sxs-lookup"><span data-stu-id="9b753-119">conditionalAccessClientApp collection</span></span>| <span data-ttu-id="9b753-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="9b753-120">Client application types included in the policy.</span></span> <span data-ttu-id="9b753-121">Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="9b753-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span> <span data-ttu-id="9b753-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b753-122">Required.</span></span>|
|<span data-ttu-id="9b753-123">deviceStates</span><span class="sxs-lookup"><span data-stu-id="9b753-123">deviceStates</span></span>|[<span data-ttu-id="9b753-124">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="9b753-124">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="9b753-125">Состояния устройств в политике.</span><span class="sxs-lookup"><span data-stu-id="9b753-125">Device states in the policy.</span></span> |
|<span data-ttu-id="9b753-126">устройства</span><span class="sxs-lookup"><span data-stu-id="9b753-126">devices</span></span>|[<span data-ttu-id="9b753-127">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="9b753-127">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="9b753-128">Устройства в политике.</span><span class="sxs-lookup"><span data-stu-id="9b753-128">Devices in the policy.</span></span> |
|<span data-ttu-id="9b753-129">locations</span><span class="sxs-lookup"><span data-stu-id="9b753-129">locations</span></span>|[<span data-ttu-id="9b753-130">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="9b753-130">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="9b753-131">Расположения, включенные и исключенные из политики.</span><span class="sxs-lookup"><span data-stu-id="9b753-131">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="9b753-132">платформы</span><span class="sxs-lookup"><span data-stu-id="9b753-132">platforms</span></span>|[<span data-ttu-id="9b753-133">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="9b753-133">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="9b753-134">Платформы, включенные и исключенные из политики.</span><span class="sxs-lookup"><span data-stu-id="9b753-134">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="9b753-135">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="9b753-135">signInRiskLevels</span></span>|<span data-ttu-id="9b753-136">коллекция riskLevel</span><span class="sxs-lookup"><span data-stu-id="9b753-136">riskLevel collection</span></span>| <span data-ttu-id="9b753-137">Уровни риска для входов, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="9b753-137">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="9b753-138">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9b753-138">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="9b753-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b753-139">Required.</span></span>|
|<span data-ttu-id="9b753-140">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="9b753-140">userRiskLevels</span></span>|<span data-ttu-id="9b753-141">коллекция riskLevel</span><span class="sxs-lookup"><span data-stu-id="9b753-141">riskLevel collection</span></span>| <span data-ttu-id="9b753-142">Уровни риска пользователей, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="9b753-142">User risk levels included in the policy.</span></span> <span data-ttu-id="9b753-143">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9b753-143">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="9b753-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b753-144">Required.</span></span>|

><span data-ttu-id="9b753-145">**Примечание:**</span><span class="sxs-lookup"><span data-stu-id="9b753-145">**Note:**</span></span>
>* <span data-ttu-id="9b753-146">**clientAppType** `modern` будет обесценить и заменить `mobileAppsAndDesktopClients` .</span><span class="sxs-lookup"><span data-stu-id="9b753-146">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> <br>
>* <span data-ttu-id="9b753-147">**clientAppType** `easUnsupported` будет обесцениться, в пользу которой будут включены поддерживаемые и неподдермываемые платформы `exchangeActiveSync` EAS.</span><span class="sxs-lookup"><span data-stu-id="9b753-147">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> <br>
>* <span data-ttu-id="9b753-148">Мы отстраняем состояние **deviceStates,** и оно может быть удалено в будущем.</span><span class="sxs-lookup"><span data-stu-id="9b753-148">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="9b753-149">В будущем используйте **условие устройств.**</span><span class="sxs-lookup"><span data-stu-id="9b753-149">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="9b753-150">Связи</span><span class="sxs-lookup"><span data-stu-id="9b753-150">Relationships</span></span>

<span data-ttu-id="9b753-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9b753-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b753-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9b753-152">JSON representation</span></span>

<span data-ttu-id="9b753-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b753-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
    "devices",
    "locations",
    "platforms",
    "signInRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


