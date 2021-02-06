---
title: Тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, управляющих применимой политикой.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e331a482fce3274463f742ceba6dc111437cd95
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137384"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="31261-103">Тип ресурса conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="31261-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="31261-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31261-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31261-105">Представляет тип условий, управляющих применимой политикой.</span><span class="sxs-lookup"><span data-stu-id="31261-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="31261-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="31261-106">Properties</span></span>

| <span data-ttu-id="31261-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="31261-107">Property</span></span>     | <span data-ttu-id="31261-108">Тип</span><span class="sxs-lookup"><span data-stu-id="31261-108">Type</span></span>        | <span data-ttu-id="31261-109">Описание</span><span class="sxs-lookup"><span data-stu-id="31261-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31261-110">applications</span><span class="sxs-lookup"><span data-stu-id="31261-110">applications</span></span>|[<span data-ttu-id="31261-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="31261-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="31261-112">Приложения и действия пользователей, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="31261-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="31261-113">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="31261-113">Required.</span></span> |
|<span data-ttu-id="31261-114">users</span><span class="sxs-lookup"><span data-stu-id="31261-114">users</span></span>|[<span data-ttu-id="31261-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="31261-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="31261-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="31261-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="31261-117">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="31261-117">Required.</span></span> |
|<span data-ttu-id="31261-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="31261-118">clientAppTypes</span></span>|<span data-ttu-id="31261-119">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="31261-119">String collection</span></span>| <span data-ttu-id="31261-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="31261-120">Client application types included in the policy.</span></span> <span data-ttu-id="31261-121">Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="31261-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="31261-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="31261-122">deviceStates</span></span>|[<span data-ttu-id="31261-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="31261-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="31261-124">Состояния устройств в политике.</span><span class="sxs-lookup"><span data-stu-id="31261-124">Device states in the policy.</span></span> |
|<span data-ttu-id="31261-125">устройства</span><span class="sxs-lookup"><span data-stu-id="31261-125">devices</span></span>|[<span data-ttu-id="31261-126">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="31261-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="31261-127">Устройства в политике.</span><span class="sxs-lookup"><span data-stu-id="31261-127">Devices in the policy.</span></span> |
|<span data-ttu-id="31261-128">locations</span><span class="sxs-lookup"><span data-stu-id="31261-128">locations</span></span>|[<span data-ttu-id="31261-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="31261-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="31261-130">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="31261-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="31261-131">платформы</span><span class="sxs-lookup"><span data-stu-id="31261-131">platforms</span></span>|[<span data-ttu-id="31261-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="31261-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="31261-133">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="31261-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="31261-134">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="31261-134">signInRiskLevels</span></span>|<span data-ttu-id="31261-135">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="31261-135">String collection</span></span>| <span data-ttu-id="31261-136">Уровни риска для входов, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="31261-136">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="31261-137">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="31261-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="31261-138">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="31261-138">userRiskLevels</span></span>|<span data-ttu-id="31261-139">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="31261-139">String collection</span></span>| <span data-ttu-id="31261-140">Уровни риска для пользователей, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="31261-140">User risk levels included in the policy.</span></span> <span data-ttu-id="31261-141">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="31261-141">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="31261-142">**Примечание:**</span><span class="sxs-lookup"><span data-stu-id="31261-142">**Note:**</span></span> 

><span data-ttu-id="31261-143">**clientAppType** `modern` будет неподготовлен и заменен `mobileAppsAndDesktopClients` .</span><span class="sxs-lookup"><span data-stu-id="31261-143">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> 

><span data-ttu-id="31261-144">**clientAppType** `easUnsupported` будет не поддерживаться, в том числе поддерживаемые и неподдершенные `exchangeActiveSync` платформы EAS.</span><span class="sxs-lookup"><span data-stu-id="31261-144">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> 

><span data-ttu-id="31261-145">Условие **deviceStates** является неподготовленным, и оно может быть удалено в будущем.</span><span class="sxs-lookup"><span data-stu-id="31261-145">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="31261-146">В будущем используйте **условие устройств.**</span><span class="sxs-lookup"><span data-stu-id="31261-146">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="31261-147">Связи</span><span class="sxs-lookup"><span data-stu-id="31261-147">Relationships</span></span>

<span data-ttu-id="31261-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="31261-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31261-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="31261-149">JSON representation</span></span>

<span data-ttu-id="31261-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31261-150">The following is a JSON representation of the resource.</span></span>

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


