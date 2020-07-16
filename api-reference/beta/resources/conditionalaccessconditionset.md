---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 763fe78508a61461f824e618867abe96c1afd348
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122604"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="09d02-103">Тип ресурса Кондитионалакцесскондитионсет</span><span class="sxs-lookup"><span data-stu-id="09d02-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="09d02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09d02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09d02-105">Представляет тип условий, определяющих, когда применяется политика.</span><span class="sxs-lookup"><span data-stu-id="09d02-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="09d02-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="09d02-106">Properties</span></span>

| <span data-ttu-id="09d02-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="09d02-107">Property</span></span>     | <span data-ttu-id="09d02-108">Тип</span><span class="sxs-lookup"><span data-stu-id="09d02-108">Type</span></span>        | <span data-ttu-id="09d02-109">Описание</span><span class="sxs-lookup"><span data-stu-id="09d02-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09d02-110">заявлен</span><span class="sxs-lookup"><span data-stu-id="09d02-110">applications</span></span>|[<span data-ttu-id="09d02-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="09d02-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="09d02-112">Приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="09d02-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="09d02-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09d02-113">Required.</span></span> |
|<span data-ttu-id="09d02-114">users</span><span class="sxs-lookup"><span data-stu-id="09d02-114">users</span></span>|[<span data-ttu-id="09d02-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="09d02-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="09d02-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="09d02-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="09d02-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09d02-117">Required.</span></span> |
|<span data-ttu-id="09d02-118">клиентапптипес</span><span class="sxs-lookup"><span data-stu-id="09d02-118">clientAppTypes</span></span>|<span data-ttu-id="09d02-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="09d02-119">String collection</span></span>| <span data-ttu-id="09d02-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="09d02-120">Client application types included in the policy.</span></span> <span data-ttu-id="09d02-121">Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="09d02-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="09d02-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="09d02-122">deviceStates</span></span>|[<span data-ttu-id="09d02-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="09d02-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="09d02-124">Состояния устройств в политике.</span><span class="sxs-lookup"><span data-stu-id="09d02-124">Device states in the policy.</span></span> |
|<span data-ttu-id="09d02-125">драйверов</span><span class="sxs-lookup"><span data-stu-id="09d02-125">devices</span></span>|[<span data-ttu-id="09d02-126">кондитионалакцессдевицес</span><span class="sxs-lookup"><span data-stu-id="09d02-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="09d02-127">Устройства в политике.</span><span class="sxs-lookup"><span data-stu-id="09d02-127">Devices in the policy.</span></span> |
|<span data-ttu-id="09d02-128">locations</span><span class="sxs-lookup"><span data-stu-id="09d02-128">locations</span></span>|[<span data-ttu-id="09d02-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="09d02-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="09d02-130">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="09d02-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="09d02-131">Embedded</span><span class="sxs-lookup"><span data-stu-id="09d02-131">platforms</span></span>|[<span data-ttu-id="09d02-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="09d02-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="09d02-133">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="09d02-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="09d02-134">сигнинрисклевелс</span><span class="sxs-lookup"><span data-stu-id="09d02-134">signInRiskLevels</span></span>|<span data-ttu-id="09d02-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="09d02-135">String collection</span></span>| <span data-ttu-id="09d02-136">Уровни риска входа, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="09d02-136">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="09d02-137">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="09d02-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="09d02-138">усеррисклевелс</span><span class="sxs-lookup"><span data-stu-id="09d02-138">userRiskLevels</span></span>|<span data-ttu-id="09d02-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="09d02-139">String collection</span></span>| <span data-ttu-id="09d02-140">Уровни риска пользователей, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="09d02-140">User risk levels included in the policy.</span></span> <span data-ttu-id="09d02-141">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="09d02-141">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="09d02-142">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="09d02-142">**Note:**</span></span> 

><span data-ttu-id="09d02-143">**клиентапптипе** `modern` считается устаревшим и заменяется на `mobileAppsAndDesktopClients` .</span><span class="sxs-lookup"><span data-stu-id="09d02-143">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> 

><span data-ttu-id="09d02-144">**клиентапптипе** `easUnsupported` считается нерекомендуемым, в том `exchangeActiveSync` числе поддерживаемых и неподдерживаемых платформах EAS.</span><span class="sxs-lookup"><span data-stu-id="09d02-144">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> 

><span data-ttu-id="09d02-145">Мы рекомендуем использовать условие **девицестатес** , и оно может быть удалено в будущем.</span><span class="sxs-lookup"><span data-stu-id="09d02-145">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="09d02-146">Перемотка вперед, используйте состояние **Devices** .</span><span class="sxs-lookup"><span data-stu-id="09d02-146">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="09d02-147">Связи</span><span class="sxs-lookup"><span data-stu-id="09d02-147">Relationships</span></span>

<span data-ttu-id="09d02-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="09d02-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09d02-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="09d02-149">JSON representation</span></span>

<span data-ttu-id="09d02-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09d02-150">The following is a JSON representation of the resource.</span></span>

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
