---
title: Тип ресурса Кондитионалакцесссессионконтролс
description: Представляет сложный тип элементов управления сеанса, который принудительно применяется после входа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e76c17838b9257a4274c51ac161a1c36d512fe3f
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916748"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="d6701-103">Тип ресурса Кондитионалакцесссессионконтролс</span><span class="sxs-lookup"><span data-stu-id="d6701-103">conditionalAccessSessionControls resource type</span></span>

<span data-ttu-id="d6701-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6701-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6701-105">Представляет элементы управления сеансом, которые применяются после входа.</span><span class="sxs-lookup"><span data-stu-id="d6701-105">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="d6701-106">Все элементы управления сеансом наследуются от [кондитионалакцесссессионконтрол](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="d6701-106">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d6701-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6701-107">Properties</span></span>

| <span data-ttu-id="d6701-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6701-108">Property</span></span>     | <span data-ttu-id="d6701-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d6701-109">Type</span></span>        | <span data-ttu-id="d6701-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d6701-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d6701-111">аппликатионенфорцедрестриктионс</span><span class="sxs-lookup"><span data-stu-id="d6701-111">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="d6701-112">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="d6701-112">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="d6701-113">Управление сеансами для применения ограничений приложений.</span><span class="sxs-lookup"><span data-stu-id="d6701-113">Session control to enforce application restrictions.</span></span> <span data-ttu-id="d6701-114">Этот элемент управления сеансом поддерживают только Exchange Online и SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d6701-114">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="d6701-115">клаудаппсекурити</span><span class="sxs-lookup"><span data-stu-id="d6701-115">cloudAppSecurity</span></span>|[<span data-ttu-id="d6701-116">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="d6701-116">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="d6701-117">Управление сеансами для применения Cloud App Security.</span><span class="sxs-lookup"><span data-stu-id="d6701-117">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="d6701-118">персистентбровсер</span><span class="sxs-lookup"><span data-stu-id="d6701-118">persistentBrowser</span></span>|[<span data-ttu-id="d6701-119">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="d6701-119">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="d6701-120">Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="d6701-120">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="d6701-121">Для правильной работы этого элемента управления сеансом необходимо выбрать все приложения.</span><span class="sxs-lookup"><span data-stu-id="d6701-121">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="d6701-122">сигнинфрекуенци</span><span class="sxs-lookup"><span data-stu-id="d6701-122">signInFrequency</span></span>|[<span data-ttu-id="d6701-123">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="d6701-123">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="d6701-124">Управление сеансами для применения частоты входа.</span><span class="sxs-lookup"><span data-stu-id="d6701-124">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6701-125">Связи</span><span class="sxs-lookup"><span data-stu-id="d6701-125">Relationships</span></span>

<span data-ttu-id="d6701-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d6701-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6701-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d6701-127">JSON representation</span></span>

<span data-ttu-id="d6701-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6701-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "applicationEnforcedRestrictions",
    "persistentBrowser",
    "cloudAppSecurity",
    "signInFrequency"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControls",
  "baseType": null
}-->

```json
{
  "applicationEnforcedRestrictions": {"@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl"},
  "cloudAppSecurity": {"@odata.type": "microsoft.graph.cloudAppSecuritySessionControl"},
  "persistentBrowser": {"@odata.type": "microsoft.graph.persistentBrowserSessionControl"},
  "signInFrequency": {"@odata.type": "microsoft.graph.signInFrequencySessionControl"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessSessionControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->