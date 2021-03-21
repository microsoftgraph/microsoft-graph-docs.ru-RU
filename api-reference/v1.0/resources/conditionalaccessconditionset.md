---
title: тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, которые регулируются при применяемой политике.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3d448b2d54fbc94c63588712f06492ce7d38a33a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962499"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="5d966-103">тип ресурса conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="5d966-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="5d966-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d966-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d966-105">Представляет тип условий, которые регулируются при применяемой политике.</span><span class="sxs-lookup"><span data-stu-id="5d966-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="5d966-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d966-106">Properties</span></span>

| <span data-ttu-id="5d966-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d966-107">Property</span></span>     | <span data-ttu-id="5d966-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5d966-108">Type</span></span>        | <span data-ttu-id="5d966-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5d966-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d966-110">приложения</span><span class="sxs-lookup"><span data-stu-id="5d966-110">applications</span></span>|[<span data-ttu-id="5d966-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="5d966-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="5d966-112">Приложения и действия пользователей, включенные и исключенные из политики.</span><span class="sxs-lookup"><span data-stu-id="5d966-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="5d966-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d966-113">Required.</span></span> |
|<span data-ttu-id="5d966-114">users</span><span class="sxs-lookup"><span data-stu-id="5d966-114">users</span></span>|[<span data-ttu-id="5d966-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="5d966-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="5d966-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="5d966-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="5d966-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d966-117">Required.</span></span> |
|<span data-ttu-id="5d966-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="5d966-118">clientAppTypes</span></span>|<span data-ttu-id="5d966-119">коллекция conditionalAccessClientApp</span><span class="sxs-lookup"><span data-stu-id="5d966-119">conditionalAccessClientApp collection</span></span>| <span data-ttu-id="5d966-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="5d966-120">Client application types included in the policy.</span></span> <span data-ttu-id="5d966-121">Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="5d966-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span> <span data-ttu-id="5d966-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d966-122">Required.</span></span>|
|<span data-ttu-id="5d966-123">locations</span><span class="sxs-lookup"><span data-stu-id="5d966-123">locations</span></span>|[<span data-ttu-id="5d966-124">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="5d966-124">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="5d966-125">Расположения, включенные и исключенные из политики.</span><span class="sxs-lookup"><span data-stu-id="5d966-125">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="5d966-126">платформы</span><span class="sxs-lookup"><span data-stu-id="5d966-126">platforms</span></span>|[<span data-ttu-id="5d966-127">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="5d966-127">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="5d966-128">Платформы, включенные и исключенные из политики.</span><span class="sxs-lookup"><span data-stu-id="5d966-128">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="5d966-129">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="5d966-129">signInRiskLevels</span></span>|<span data-ttu-id="5d966-130">коллекция riskLevel</span><span class="sxs-lookup"><span data-stu-id="5d966-130">riskLevel collection</span></span>| <span data-ttu-id="5d966-131">Уровни риска для входов, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="5d966-131">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="5d966-132">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5d966-132">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="5d966-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d966-133">Required.</span></span>|
|<span data-ttu-id="5d966-134">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="5d966-134">userRiskLevels</span></span>|<span data-ttu-id="5d966-135">коллекция riskLevel</span><span class="sxs-lookup"><span data-stu-id="5d966-135">riskLevel collection</span></span>| <span data-ttu-id="5d966-136">Уровни риска пользователей, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="5d966-136">User risk levels included in the policy.</span></span> <span data-ttu-id="5d966-137">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5d966-137">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="5d966-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d966-138">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d966-139">Связи</span><span class="sxs-lookup"><span data-stu-id="5d966-139">Relationships</span></span>

<span data-ttu-id="5d966-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5d966-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d966-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5d966-141">JSON representation</span></span>

<span data-ttu-id="5d966-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d966-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "locations",
    "platforms",
    "signInRiskLevels",
    "userRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"],
  "userRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

