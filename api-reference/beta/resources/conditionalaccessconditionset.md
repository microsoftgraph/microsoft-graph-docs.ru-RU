---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e81e8b2748a7dc3b6a9ca028472c1f6ab153b0e
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638514"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="60846-103">Тип ресурса Кондитионалакцесскондитионсет</span><span class="sxs-lookup"><span data-stu-id="60846-103">conditionalAccessConditionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60846-104">Представляет тип условий, определяющих, когда применяется политика.</span><span class="sxs-lookup"><span data-stu-id="60846-104">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="60846-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="60846-105">Properties</span></span>

| <span data-ttu-id="60846-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="60846-106">Property</span></span>     | <span data-ttu-id="60846-107">Тип</span><span class="sxs-lookup"><span data-stu-id="60846-107">Type</span></span>        | <span data-ttu-id="60846-108">Описание</span><span class="sxs-lookup"><span data-stu-id="60846-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="60846-109">заявлен</span><span class="sxs-lookup"><span data-stu-id="60846-109">applications</span></span>|[<span data-ttu-id="60846-110">кондитионалакцессаппликатионс</span><span class="sxs-lookup"><span data-stu-id="60846-110">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="60846-111">Приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="60846-111">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="60846-112">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="60846-112">Required.</span></span> |
|<span data-ttu-id="60846-113">users</span><span class="sxs-lookup"><span data-stu-id="60846-113">users</span></span>|[<span data-ttu-id="60846-114">кондитионалакцессусерс</span><span class="sxs-lookup"><span data-stu-id="60846-114">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="60846-115">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="60846-115">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="60846-116">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="60846-116">Required.</span></span> |
|<span data-ttu-id="60846-117">клиентапптипес</span><span class="sxs-lookup"><span data-stu-id="60846-117">clientAppTypes</span></span>|<span data-ttu-id="60846-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="60846-118">String collection</span></span>| <span data-ttu-id="60846-119">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="60846-119">Client application types included in the policy.</span></span> <span data-ttu-id="60846-120">Возможные значения: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="60846-120">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="60846-121">deviceStates</span><span class="sxs-lookup"><span data-stu-id="60846-121">deviceStates</span></span>|[<span data-ttu-id="60846-122">кондитионалакцессдевицестатес</span><span class="sxs-lookup"><span data-stu-id="60846-122">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="60846-123">Состояния устройств в политике.</span><span class="sxs-lookup"><span data-stu-id="60846-123">Device states in the policy.</span></span> |
|<span data-ttu-id="60846-124">locations</span><span class="sxs-lookup"><span data-stu-id="60846-124">locations</span></span>|[<span data-ttu-id="60846-125">кондитионалакцесслокатионс</span><span class="sxs-lookup"><span data-stu-id="60846-125">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="60846-126">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="60846-126">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="60846-127">Embedded</span><span class="sxs-lookup"><span data-stu-id="60846-127">platforms</span></span>|[<span data-ttu-id="60846-128">кондитионалакцессплатформс</span><span class="sxs-lookup"><span data-stu-id="60846-128">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="60846-129">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="60846-129">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="60846-130">сигнинрисклевелс</span><span class="sxs-lookup"><span data-stu-id="60846-130">signInRiskLevels</span></span>|<span data-ttu-id="60846-131">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="60846-131">String collection</span></span>| <span data-ttu-id="60846-132">Уровни риска, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="60846-132">Risk levels included in the policy.</span></span> <span data-ttu-id="60846-133">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="60846-133">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60846-134">Связи</span><span class="sxs-lookup"><span data-stu-id="60846-134">Relationships</span></span>

<span data-ttu-id="60846-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="60846-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60846-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="60846-136">JSON representation</span></span>

<span data-ttu-id="60846-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60846-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
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