---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9b9e4149f05825e6698703457aeb4b7709382a7
ms.sourcegitcommit: 5d4bf35774eba6de21f4252b46f7e9d8f64a517f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/08/2020
ms.locfileid: "44168560"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="94af7-103">Тип ресурса Кондитионалакцесскондитионсет</span><span class="sxs-lookup"><span data-stu-id="94af7-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="94af7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94af7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94af7-105">Представляет тип условий, определяющих, когда применяется политика.</span><span class="sxs-lookup"><span data-stu-id="94af7-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="94af7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="94af7-106">Properties</span></span>

| <span data-ttu-id="94af7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="94af7-107">Property</span></span>     | <span data-ttu-id="94af7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="94af7-108">Type</span></span>        | <span data-ttu-id="94af7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="94af7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94af7-110">заявлен</span><span class="sxs-lookup"><span data-stu-id="94af7-110">applications</span></span>|[<span data-ttu-id="94af7-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="94af7-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="94af7-112">Приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="94af7-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="94af7-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94af7-113">Required.</span></span> |
|<span data-ttu-id="94af7-114">users</span><span class="sxs-lookup"><span data-stu-id="94af7-114">users</span></span>|[<span data-ttu-id="94af7-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="94af7-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="94af7-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="94af7-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="94af7-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94af7-117">Required.</span></span> |
|<span data-ttu-id="94af7-118">клиентапптипес</span><span class="sxs-lookup"><span data-stu-id="94af7-118">clientAppTypes</span></span>|<span data-ttu-id="94af7-119">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="94af7-119">String collection</span></span>| <span data-ttu-id="94af7-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="94af7-120">Client application types included in the policy.</span></span> <span data-ttu-id="94af7-121">Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="94af7-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="94af7-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="94af7-122">deviceStates</span></span>|[<span data-ttu-id="94af7-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="94af7-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="94af7-124">Состояния устройств в политике.</span><span class="sxs-lookup"><span data-stu-id="94af7-124">Device states in the policy.</span></span> |
|<span data-ttu-id="94af7-125">драйверов</span><span class="sxs-lookup"><span data-stu-id="94af7-125">devices</span></span>|[<span data-ttu-id="94af7-126">кондитионалакцессдевицес</span><span class="sxs-lookup"><span data-stu-id="94af7-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="94af7-127">Устройства в политике.</span><span class="sxs-lookup"><span data-stu-id="94af7-127">Devices in the policy.</span></span> |
|<span data-ttu-id="94af7-128">locations</span><span class="sxs-lookup"><span data-stu-id="94af7-128">locations</span></span>|[<span data-ttu-id="94af7-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="94af7-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="94af7-130">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="94af7-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="94af7-131">Embedded</span><span class="sxs-lookup"><span data-stu-id="94af7-131">platforms</span></span>|[<span data-ttu-id="94af7-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="94af7-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="94af7-133">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="94af7-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="94af7-134">сигнинрисклевелс</span><span class="sxs-lookup"><span data-stu-id="94af7-134">signInRiskLevels</span></span>|<span data-ttu-id="94af7-135">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="94af7-135">String collection</span></span>| <span data-ttu-id="94af7-136">Уровни риска, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="94af7-136">Risk levels included in the policy.</span></span> <span data-ttu-id="94af7-137">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="94af7-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="94af7-138">**Примечание.**</span><span class="sxs-lookup"><span data-stu-id="94af7-138">**Note:**</span></span> 

><span data-ttu-id="94af7-139">**клиентапптипе** `modern` считается устаревшим и заменяется на `mobileAppsAndDesktopClients`.</span><span class="sxs-lookup"><span data-stu-id="94af7-139">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> 

><span data-ttu-id="94af7-140">**клиентапптипе** `easUnsupported` считается нерекомендуемым, в `exchangeActiveSync` том числе поддерживаемых EAS и неподдерживаемых платформ.</span><span class="sxs-lookup"><span data-stu-id="94af7-140">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> 

><span data-ttu-id="94af7-141">Мы рекомендуем использовать условие **девицестатес** , и оно может быть удалено в будущем.</span><span class="sxs-lookup"><span data-stu-id="94af7-141">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="94af7-142">Перемотка вперед, используйте состояние **Devices** .</span><span class="sxs-lookup"><span data-stu-id="94af7-142">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="94af7-143">Связи</span><span class="sxs-lookup"><span data-stu-id="94af7-143">Relationships</span></span>

<span data-ttu-id="94af7-144">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="94af7-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94af7-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="94af7-145">JSON representation</span></span>

<span data-ttu-id="94af7-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94af7-146">The following is a JSON representation of the resource.</span></span>

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
