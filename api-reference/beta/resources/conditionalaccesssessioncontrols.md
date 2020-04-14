---
title: Тип ресурса Кондитионалакцесссессионконтролс
description: Представляет сложный тип элементов управления сеанса, который принудительно применяется после входа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 13e1bc5b7f042634f1e4d2c9384c88fab5b96b29
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450820"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="df6a3-103">Тип ресурса Кондитионалакцесссессионконтролс</span><span class="sxs-lookup"><span data-stu-id="df6a3-103">conditionalAccessSessionControls resource type</span></span>

<span data-ttu-id="df6a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df6a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df6a3-105">Представляет элементы управления сеансом, которые применяются после входа.</span><span class="sxs-lookup"><span data-stu-id="df6a3-105">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="df6a3-106">Все элементы управления сеансом наследуются от [кондитионалакцесссессионконтрол](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="df6a3-106">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="df6a3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="df6a3-107">Properties</span></span>

| <span data-ttu-id="df6a3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="df6a3-108">Property</span></span>     | <span data-ttu-id="df6a3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="df6a3-109">Type</span></span>        | <span data-ttu-id="df6a3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="df6a3-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df6a3-111">аппликатионенфорцедрестриктионс</span><span class="sxs-lookup"><span data-stu-id="df6a3-111">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="df6a3-112">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="df6a3-112">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="df6a3-113">Управление сеансами для применения ограничений приложений.</span><span class="sxs-lookup"><span data-stu-id="df6a3-113">Session control to enforce application restrictions.</span></span> <span data-ttu-id="df6a3-114">Этот элемент управления сеансом поддерживают только Exchange Online и SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="df6a3-114">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="df6a3-115">клаудаппсекурити</span><span class="sxs-lookup"><span data-stu-id="df6a3-115">cloudAppSecurity</span></span>|[<span data-ttu-id="df6a3-116">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="df6a3-116">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="df6a3-117">Управление сеансами для применения Cloud App Security.</span><span class="sxs-lookup"><span data-stu-id="df6a3-117">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="df6a3-118">персистентбровсер</span><span class="sxs-lookup"><span data-stu-id="df6a3-118">persistentBrowser</span></span>|[<span data-ttu-id="df6a3-119">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="df6a3-119">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="df6a3-120">Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="df6a3-120">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="df6a3-121">Для правильной работы этого элемента управления сеансом необходимо выбрать все приложения.</span><span class="sxs-lookup"><span data-stu-id="df6a3-121">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="df6a3-122">сигнинфрекуенци</span><span class="sxs-lookup"><span data-stu-id="df6a3-122">signInFrequency</span></span>|[<span data-ttu-id="df6a3-123">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="df6a3-123">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="df6a3-124">Управление сеансами для применения частоты входа.</span><span class="sxs-lookup"><span data-stu-id="df6a3-124">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df6a3-125">Связи</span><span class="sxs-lookup"><span data-stu-id="df6a3-125">Relationships</span></span>

<span data-ttu-id="df6a3-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="df6a3-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df6a3-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="df6a3-127">JSON representation</span></span>

<span data-ttu-id="df6a3-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df6a3-128">The following is a JSON representation of the resource.</span></span>

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