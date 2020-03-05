---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dee80ebdacfda6c0b633f1aec1dd085d80eb22e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507564"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="b3b9c-103">Тип ресурса Кондитионалакцесскондитионсет</span><span class="sxs-lookup"><span data-stu-id="b3b9c-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="b3b9c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b3b9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3b9c-105">Представляет тип условий, определяющих, когда применяется политика.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="b3b9c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3b9c-106">Properties</span></span>

| <span data-ttu-id="b3b9c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3b9c-107">Property</span></span>     | <span data-ttu-id="b3b9c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b3b9c-108">Type</span></span>        | <span data-ttu-id="b3b9c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b3b9c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3b9c-110">заявлен</span><span class="sxs-lookup"><span data-stu-id="b3b9c-110">applications</span></span>|[<span data-ttu-id="b3b9c-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="b3b9c-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="b3b9c-112">Приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="b3b9c-113">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-113">Required.</span></span> |
|<span data-ttu-id="b3b9c-114">users</span><span class="sxs-lookup"><span data-stu-id="b3b9c-114">users</span></span>|[<span data-ttu-id="b3b9c-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="b3b9c-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="b3b9c-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="b3b9c-117">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-117">Required.</span></span> |
|<span data-ttu-id="b3b9c-118">клиентапптипес</span><span class="sxs-lookup"><span data-stu-id="b3b9c-118">clientAppTypes</span></span>|<span data-ttu-id="b3b9c-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3b9c-119">String collection</span></span>| <span data-ttu-id="b3b9c-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-120">Client application types included in the policy.</span></span> <span data-ttu-id="b3b9c-121">Возможные значения: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-121">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="b3b9c-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="b3b9c-122">deviceStates</span></span>|[<span data-ttu-id="b3b9c-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="b3b9c-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="b3b9c-124">Состояния устройств в политике.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-124">Device states in the policy.</span></span> |
|<span data-ttu-id="b3b9c-125">locations</span><span class="sxs-lookup"><span data-stu-id="b3b9c-125">locations</span></span>|[<span data-ttu-id="b3b9c-126">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="b3b9c-126">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="b3b9c-127">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-127">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="b3b9c-128">Embedded</span><span class="sxs-lookup"><span data-stu-id="b3b9c-128">platforms</span></span>|[<span data-ttu-id="b3b9c-129">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="b3b9c-129">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="b3b9c-130">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-130">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="b3b9c-131">сигнинрисклевелс</span><span class="sxs-lookup"><span data-stu-id="b3b9c-131">signInRiskLevels</span></span>|<span data-ttu-id="b3b9c-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3b9c-132">String collection</span></span>| <span data-ttu-id="b3b9c-133">Уровни риска, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-133">Risk levels included in the policy.</span></span> <span data-ttu-id="b3b9c-134">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-134">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3b9c-135">Связи</span><span class="sxs-lookup"><span data-stu-id="b3b9c-135">Relationships</span></span>

<span data-ttu-id="b3b9c-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3b9c-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b3b9c-137">JSON representation</span></span>

<span data-ttu-id="b3b9c-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3b9c-138">The following is a JSON representation of the resource.</span></span>

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