---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1fd96fb7bfa54ff059afa83b7ea922737dc90809
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018930"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="1e921-103">Тип ресурса Кондитионалакцесскондитионсет</span><span class="sxs-lookup"><span data-stu-id="1e921-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="1e921-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e921-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e921-105">Представляет тип условий, определяющих, когда применяется политика.</span><span class="sxs-lookup"><span data-stu-id="1e921-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="1e921-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e921-106">Properties</span></span>

| <span data-ttu-id="1e921-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e921-107">Property</span></span>     | <span data-ttu-id="1e921-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1e921-108">Type</span></span>        | <span data-ttu-id="1e921-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e921-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e921-110">заявлен</span><span class="sxs-lookup"><span data-stu-id="1e921-110">applications</span></span>|[<span data-ttu-id="1e921-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="1e921-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="1e921-112">Приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="1e921-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="1e921-113">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1e921-113">Required.</span></span> |
|<span data-ttu-id="1e921-114">users</span><span class="sxs-lookup"><span data-stu-id="1e921-114">users</span></span>|[<span data-ttu-id="1e921-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="1e921-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="1e921-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="1e921-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="1e921-117">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1e921-117">Required.</span></span> |
|<span data-ttu-id="1e921-118">клиентапптипес</span><span class="sxs-lookup"><span data-stu-id="1e921-118">clientAppTypes</span></span>|<span data-ttu-id="1e921-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1e921-119">String collection</span></span>| <span data-ttu-id="1e921-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="1e921-120">Client application types included in the policy.</span></span> <span data-ttu-id="1e921-121">Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="1e921-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="1e921-122">locations</span><span class="sxs-lookup"><span data-stu-id="1e921-122">locations</span></span>|[<span data-ttu-id="1e921-123">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="1e921-123">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="1e921-124">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="1e921-124">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="1e921-125">Embedded</span><span class="sxs-lookup"><span data-stu-id="1e921-125">platforms</span></span>|[<span data-ttu-id="1e921-126">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="1e921-126">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="1e921-127">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="1e921-127">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="1e921-128">сигнинрисклевелс</span><span class="sxs-lookup"><span data-stu-id="1e921-128">signInRiskLevels</span></span>|<span data-ttu-id="1e921-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1e921-129">String collection</span></span>| <span data-ttu-id="1e921-130">Уровни риска, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="1e921-130">Risk levels included in the policy.</span></span> <span data-ttu-id="1e921-131">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="1e921-131">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e921-132">Связи</span><span class="sxs-lookup"><span data-stu-id="1e921-132">Relationships</span></span>

<span data-ttu-id="1e921-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1e921-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e921-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e921-134">JSON representation</span></span>

<span data-ttu-id="1e921-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e921-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
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
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
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

