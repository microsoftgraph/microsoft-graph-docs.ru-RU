---
title: Тип ресурса Кондитионалакцесссессионконтролс
description: Представляет сложный тип элементов управления сеанса, который принудительно применяется после входа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 317120eb7c4138d955bf8a35030375180d5a1631
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638549"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="b6853-103">Тип ресурса Кондитионалакцесссессионконтролс</span><span class="sxs-lookup"><span data-stu-id="b6853-103">conditionalAccessSessionControls resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6853-104">Представляет элементы управления сеансом, которые применяются после входа.</span><span class="sxs-lookup"><span data-stu-id="b6853-104">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="b6853-105">Все элементы управления сеансом наследуются от [кондитионалакцесссессионконтрол](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="b6853-105">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b6853-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6853-106">Properties</span></span>

| <span data-ttu-id="b6853-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6853-107">Property</span></span>     | <span data-ttu-id="b6853-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b6853-108">Type</span></span>        | <span data-ttu-id="b6853-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b6853-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6853-110">аппликатионенфорцедрестриктионс</span><span class="sxs-lookup"><span data-stu-id="b6853-110">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="b6853-111">аппликатионенфорцедрестриктионссессионконтрол</span><span class="sxs-lookup"><span data-stu-id="b6853-111">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="b6853-112">Управление сеансами для применения ограничений приложений.</span><span class="sxs-lookup"><span data-stu-id="b6853-112">Session control to enforce application restrictions.</span></span> <span data-ttu-id="b6853-113">Этот элемент управления сеансом поддерживают только Exchange Online и SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b6853-113">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="b6853-114">клаудаппсекурити</span><span class="sxs-lookup"><span data-stu-id="b6853-114">cloudAppSecurity</span></span>|[<span data-ttu-id="b6853-115">клаудаппсекуритисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="b6853-115">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="b6853-116">Управление сеансами для применения Cloud App Security.</span><span class="sxs-lookup"><span data-stu-id="b6853-116">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="b6853-117">персистентбровсер</span><span class="sxs-lookup"><span data-stu-id="b6853-117">persistentBrowser</span></span>|[<span data-ttu-id="b6853-118">персистентбровсерсессионконтрол</span><span class="sxs-lookup"><span data-stu-id="b6853-118">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="b6853-119">Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="b6853-119">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="b6853-120">Для правильной работы этого элемента управления сеансом необходимо выбрать все приложения.</span><span class="sxs-lookup"><span data-stu-id="b6853-120">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="b6853-121">сигнинфрекуенци</span><span class="sxs-lookup"><span data-stu-id="b6853-121">signInFrequency</span></span>|[<span data-ttu-id="b6853-122">сигнинфрекуенцисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="b6853-122">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="b6853-123">Управление сеансами для применения частоты входа.</span><span class="sxs-lookup"><span data-stu-id="b6853-123">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6853-124">Связи</span><span class="sxs-lookup"><span data-stu-id="b6853-124">Relationships</span></span>

<span data-ttu-id="b6853-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b6853-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6853-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b6853-126">JSON representation</span></span>

<span data-ttu-id="b6853-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6853-127">The following is a JSON representation of the resource.</span></span>

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