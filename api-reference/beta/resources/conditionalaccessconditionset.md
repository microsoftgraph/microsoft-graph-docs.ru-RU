---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5db4c6367834733a4a5fbbb6c7a8d6b08393160
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805679"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="564b1-103">Тип ресурса Кондитионалакцесскондитионсет</span><span class="sxs-lookup"><span data-stu-id="564b1-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="564b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="564b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="564b1-105">Представляет тип условий, определяющих, когда применяется политика.</span><span class="sxs-lookup"><span data-stu-id="564b1-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="564b1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="564b1-106">Properties</span></span>

| <span data-ttu-id="564b1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="564b1-107">Property</span></span>     | <span data-ttu-id="564b1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="564b1-108">Type</span></span>        | <span data-ttu-id="564b1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="564b1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="564b1-110">заявлен</span><span class="sxs-lookup"><span data-stu-id="564b1-110">applications</span></span>|[<span data-ttu-id="564b1-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="564b1-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="564b1-112">Приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="564b1-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="564b1-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="564b1-113">Required.</span></span> |
|<span data-ttu-id="564b1-114">users</span><span class="sxs-lookup"><span data-stu-id="564b1-114">users</span></span>|[<span data-ttu-id="564b1-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="564b1-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="564b1-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="564b1-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="564b1-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="564b1-117">Required.</span></span> |
|<span data-ttu-id="564b1-118">клиентапптипес</span><span class="sxs-lookup"><span data-stu-id="564b1-118">clientAppTypes</span></span>|<span data-ttu-id="564b1-119">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="564b1-119">String collection</span></span>| <span data-ttu-id="564b1-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="564b1-120">Client application types included in the policy.</span></span> <span data-ttu-id="564b1-121">Возможные значения: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="564b1-121">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="564b1-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="564b1-122">deviceStates</span></span>|[<span data-ttu-id="564b1-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="564b1-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="564b1-124">Состояния устройств в политике.</span><span class="sxs-lookup"><span data-stu-id="564b1-124">Device states in the policy.</span></span> |
|<span data-ttu-id="564b1-125">драйверов</span><span class="sxs-lookup"><span data-stu-id="564b1-125">devices</span></span>|[<span data-ttu-id="564b1-126">кондитионалакцессдевицес</span><span class="sxs-lookup"><span data-stu-id="564b1-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="564b1-127">Устройства в политике.</span><span class="sxs-lookup"><span data-stu-id="564b1-127">Devices in the policy.</span></span> |
|<span data-ttu-id="564b1-128">locations</span><span class="sxs-lookup"><span data-stu-id="564b1-128">locations</span></span>|[<span data-ttu-id="564b1-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="564b1-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="564b1-130">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="564b1-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="564b1-131">Embedded</span><span class="sxs-lookup"><span data-stu-id="564b1-131">platforms</span></span>|[<span data-ttu-id="564b1-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="564b1-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="564b1-133">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="564b1-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="564b1-134">сигнинрисклевелс</span><span class="sxs-lookup"><span data-stu-id="564b1-134">signInRiskLevels</span></span>|<span data-ttu-id="564b1-135">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="564b1-135">String collection</span></span>| <span data-ttu-id="564b1-136">Уровни риска, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="564b1-136">Risk levels included in the policy.</span></span> <span data-ttu-id="564b1-137">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="564b1-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="564b1-138">**Примечание:** Мы рекомендуем использовать условие **девицестатес** , и оно может быть удалено в будущем.</span><span class="sxs-lookup"><span data-stu-id="564b1-138">**Note:** We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="564b1-139">Перемотка вперед, используйте состояние **Devices** .</span><span class="sxs-lookup"><span data-stu-id="564b1-139">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="564b1-140">Связи</span><span class="sxs-lookup"><span data-stu-id="564b1-140">Relationships</span></span>

<span data-ttu-id="564b1-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="564b1-141">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="564b1-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="564b1-142">JSON representation</span></span>

<span data-ttu-id="564b1-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="564b1-143">The following is a JSON representation of the resource.</span></span>

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
