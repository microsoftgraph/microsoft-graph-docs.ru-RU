---
title: Тип ресурса Кондитионалакцесскондитионсет
description: Представляет тип условий, определяющих, когда применяется политика.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aaec4b4cfcca6cc42ef7f4376982ef207ab1c767
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413511"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="dd12c-103">Тип ресурса Кондитионалакцесскондитионсет</span><span class="sxs-lookup"><span data-stu-id="dd12c-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="dd12c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd12c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd12c-105">Представляет тип условий, определяющих, когда применяется политика.</span><span class="sxs-lookup"><span data-stu-id="dd12c-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="dd12c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd12c-106">Properties</span></span>

| <span data-ttu-id="dd12c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd12c-107">Property</span></span>     | <span data-ttu-id="dd12c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dd12c-108">Type</span></span>        | <span data-ttu-id="dd12c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dd12c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd12c-110">заявлен</span><span class="sxs-lookup"><span data-stu-id="dd12c-110">applications</span></span>|[<span data-ttu-id="dd12c-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="dd12c-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="dd12c-112">Приложения и действия пользователя, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="dd12c-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="dd12c-113">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dd12c-113">Required.</span></span> |
|<span data-ttu-id="dd12c-114">users</span><span class="sxs-lookup"><span data-stu-id="dd12c-114">users</span></span>|[<span data-ttu-id="dd12c-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="dd12c-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="dd12c-116">Пользователи, группы и роли, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="dd12c-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="dd12c-117">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dd12c-117">Required.</span></span> |
|<span data-ttu-id="dd12c-118">клиентапптипес</span><span class="sxs-lookup"><span data-stu-id="dd12c-118">clientAppTypes</span></span>|<span data-ttu-id="dd12c-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dd12c-119">String collection</span></span>| <span data-ttu-id="dd12c-120">Типы клиентских приложений, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="dd12c-120">Client application types included in the policy.</span></span> <span data-ttu-id="dd12c-121">Возможные значения: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="dd12c-121">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="dd12c-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="dd12c-122">deviceStates</span></span>|[<span data-ttu-id="dd12c-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="dd12c-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="dd12c-124">Состояния устройств в политике.</span><span class="sxs-lookup"><span data-stu-id="dd12c-124">Device states in the policy.</span></span> |
|<span data-ttu-id="dd12c-125">locations</span><span class="sxs-lookup"><span data-stu-id="dd12c-125">locations</span></span>|[<span data-ttu-id="dd12c-126">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="dd12c-126">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="dd12c-127">Расположения, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="dd12c-127">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="dd12c-128">Embedded</span><span class="sxs-lookup"><span data-stu-id="dd12c-128">platforms</span></span>|[<span data-ttu-id="dd12c-129">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="dd12c-129">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="dd12c-130">Платформы, включенные в политику и исключенные из нее.</span><span class="sxs-lookup"><span data-stu-id="dd12c-130">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="dd12c-131">сигнинрисклевелс</span><span class="sxs-lookup"><span data-stu-id="dd12c-131">signInRiskLevels</span></span>|<span data-ttu-id="dd12c-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dd12c-132">String collection</span></span>| <span data-ttu-id="dd12c-133">Уровни риска, включенные в политику.</span><span class="sxs-lookup"><span data-stu-id="dd12c-133">Risk levels included in the policy.</span></span> <span data-ttu-id="dd12c-134">Возможные значения: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="dd12c-134">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd12c-135">Связи</span><span class="sxs-lookup"><span data-stu-id="dd12c-135">Relationships</span></span>

<span data-ttu-id="dd12c-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dd12c-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd12c-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dd12c-137">JSON representation</span></span>

<span data-ttu-id="dd12c-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd12c-138">The following is a JSON representation of the resource.</span></span>

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