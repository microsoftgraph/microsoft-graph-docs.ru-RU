---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 993201181a9256b54663ce279c914e3669f4dc91
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384681"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="b197f-103">Тип ресурса Кондитионалакцесскондитионсет</span><span class="sxs-lookup"><span data-stu-id="b197f-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="b197f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b197f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b197f-105">Представляет тип условий, определяющих, когда применяется политика.</span><span class="sxs-lookup"><span data-stu-id="b197f-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="b197f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b197f-106">Properties</span></span>

| <span data-ttu-id="b197f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b197f-107">Property</span></span>     | <span data-ttu-id="b197f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b197f-108">Type</span></span>        | <span data-ttu-id="b197f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b197f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b197f-110">заявлен</span><span class="sxs-lookup"><span data-stu-id="b197f-110">applications</span></span>|[<span data-ttu-id="b197f-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="b197f-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="b197f-112">Приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b197f-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="b197f-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b197f-113">Required.</span></span> |
|<span data-ttu-id="b197f-114">users</span><span class="sxs-lookup"><span data-stu-id="b197f-114">users</span></span>|[<span data-ttu-id="b197f-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="b197f-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="b197f-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b197f-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="b197f-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b197f-117">Required.</span></span> |
|<span data-ttu-id="b197f-118">клиентапптипес</span><span class="sxs-lookup"><span data-stu-id="b197f-118">clientAppTypes</span></span>|<span data-ttu-id="b197f-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b197f-119">String collection</span></span>| <span data-ttu-id="b197f-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="b197f-120">Client application types included in the policy.</span></span> <span data-ttu-id="b197f-121">Возможные значения: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="b197f-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="b197f-122">locations</span><span class="sxs-lookup"><span data-stu-id="b197f-122">locations</span></span>|[<span data-ttu-id="b197f-123">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="b197f-123">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="b197f-124">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b197f-124">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="b197f-125">Embedded</span><span class="sxs-lookup"><span data-stu-id="b197f-125">platforms</span></span>|[<span data-ttu-id="b197f-126">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="b197f-126">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="b197f-127">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="b197f-127">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="b197f-128">сигнинрисклевелс</span><span class="sxs-lookup"><span data-stu-id="b197f-128">signInRiskLevels</span></span>|<span data-ttu-id="b197f-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b197f-129">String collection</span></span>| <span data-ttu-id="b197f-130">Уровни риска, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="b197f-130">Risk levels included in the policy.</span></span> <span data-ttu-id="b197f-131">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="b197f-131">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b197f-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b197f-132">Relationships</span></span>

<span data-ttu-id="b197f-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b197f-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b197f-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b197f-134">JSON representation</span></span>

<span data-ttu-id="b197f-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b197f-135">The following is a JSON representation of the resource.</span></span>

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
