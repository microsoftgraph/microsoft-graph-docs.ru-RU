---
title: Тип ресурса conditionalAccessConditionSet
description: Представляет тип условий, управляющих применимой политикой.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ff7159c09b0afcaf223a5840584d531e99be2da6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132136"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="25d0d-103">Тип ресурса conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="25d0d-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="25d0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25d0d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="25d0d-105">Представляет тип условий, управляющих применимой политикой.</span><span class="sxs-lookup"><span data-stu-id="25d0d-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="25d0d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="25d0d-106">Properties</span></span>

| <span data-ttu-id="25d0d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="25d0d-107">Property</span></span>     | <span data-ttu-id="25d0d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="25d0d-108">Type</span></span>        | <span data-ttu-id="25d0d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25d0d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="25d0d-110">applications</span><span class="sxs-lookup"><span data-stu-id="25d0d-110">applications</span></span>|[<span data-ttu-id="25d0d-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="25d0d-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="25d0d-112">Приложения и действия пользователей, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="25d0d-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="25d0d-113">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="25d0d-113">Required.</span></span> |
|<span data-ttu-id="25d0d-114">users</span><span class="sxs-lookup"><span data-stu-id="25d0d-114">users</span></span>|[<span data-ttu-id="25d0d-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="25d0d-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="25d0d-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="25d0d-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="25d0d-117">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="25d0d-117">Required.</span></span> |
|<span data-ttu-id="25d0d-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="25d0d-118">clientAppTypes</span></span>|<span data-ttu-id="25d0d-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="25d0d-119">String collection</span></span>| <span data-ttu-id="25d0d-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="25d0d-120">Client application types included in the policy.</span></span> <span data-ttu-id="25d0d-121">Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="25d0d-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="25d0d-122">locations</span><span class="sxs-lookup"><span data-stu-id="25d0d-122">locations</span></span>|[<span data-ttu-id="25d0d-123">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="25d0d-123">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="25d0d-124">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="25d0d-124">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="25d0d-125">платформы</span><span class="sxs-lookup"><span data-stu-id="25d0d-125">platforms</span></span>|[<span data-ttu-id="25d0d-126">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="25d0d-126">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="25d0d-127">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="25d0d-127">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="25d0d-128">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="25d0d-128">signInRiskLevels</span></span>|<span data-ttu-id="25d0d-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="25d0d-129">String collection</span></span>| <span data-ttu-id="25d0d-130">Уровни риска для входов, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="25d0d-130">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="25d0d-131">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="25d0d-131">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="25d0d-132">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="25d0d-132">userRiskLevels</span></span>|<span data-ttu-id="25d0d-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="25d0d-133">String collection</span></span>| <span data-ttu-id="25d0d-134">Уровни риска для пользователей, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="25d0d-134">User risk levels included in the policy.</span></span> <span data-ttu-id="25d0d-135">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="25d0d-135">Possible values are: `low`, `medium`, `high`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25d0d-136">Связи</span><span class="sxs-lookup"><span data-stu-id="25d0d-136">Relationships</span></span>

<span data-ttu-id="25d0d-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25d0d-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25d0d-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25d0d-138">JSON representation</span></span>

<span data-ttu-id="25d0d-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25d0d-139">The following is a JSON representation of the resource.</span></span>

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

