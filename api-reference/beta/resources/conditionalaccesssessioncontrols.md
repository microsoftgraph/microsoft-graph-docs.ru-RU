---
title: Тип ресурса conditionalAccessSessionControls
description: Представляет сложный тип элементов управления сеансом, которые применяются после регистрации.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: bf50399a26999c35730e2ce0c171c1be8777841d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134892"
---
# <a name="conditionalaccesssessioncontrols-resource-type"></a><span data-ttu-id="a8163-103">Тип ресурса conditionalAccessSessionControls</span><span class="sxs-lookup"><span data-stu-id="a8163-103">conditionalAccessSessionControls resource type</span></span>

<span data-ttu-id="a8163-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8163-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8163-105">Представляет элементы управления сеансом, которые применяются после регистрации.</span><span class="sxs-lookup"><span data-stu-id="a8163-105">Represents session controls that are enforced after sign-in.</span></span>
<span data-ttu-id="a8163-106">Все элементы управления сеансом наследуются [от conditionalAccessSessionControl.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="a8163-106">All the session controls inherit from [conditionalAccessSessionControl](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a8163-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8163-107">Properties</span></span>

| <span data-ttu-id="a8163-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8163-108">Property</span></span>     | <span data-ttu-id="a8163-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a8163-109">Type</span></span>        | <span data-ttu-id="a8163-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a8163-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8163-111">applicationEnforcedRestrictions</span><span class="sxs-lookup"><span data-stu-id="a8163-111">applicationEnforcedRestrictions</span></span>|[<span data-ttu-id="a8163-112">applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="a8163-112">applicationEnforcedRestrictionsSessionControl</span></span>](applicationenforcedrestrictionssessioncontrol.md)| <span data-ttu-id="a8163-113">Управление сеансом для применения ограничений приложений.</span><span class="sxs-lookup"><span data-stu-id="a8163-113">Session control to enforce application restrictions.</span></span> <span data-ttu-id="a8163-114">Этот контроль сеансов поддерживается только в Exchange Online и Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="a8163-114">Only Exchange Online and Sharepoint Online support this session control.</span></span> |
|<span data-ttu-id="a8163-115">cloudAppSecurity</span><span class="sxs-lookup"><span data-stu-id="a8163-115">cloudAppSecurity</span></span>|[<span data-ttu-id="a8163-116">cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="a8163-116">cloudAppSecuritySessionControl</span></span>](cloudappsecuritysessioncontrol.md)| <span data-ttu-id="a8163-117">Управление сеансом для применения безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="a8163-117">Session control to apply cloud app security.</span></span>|
|<span data-ttu-id="a8163-118">persistentBrowser</span><span class="sxs-lookup"><span data-stu-id="a8163-118">persistentBrowser</span></span>|[<span data-ttu-id="a8163-119">persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="a8163-119">persistentBrowserSessionControl</span></span>](persistentbrowsersessioncontrol.md)| <span data-ttu-id="a8163-120">Управление сеансом для определения того, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="a8163-120">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="a8163-121">Для правильной работы этого сеанса необходимо выбрать все приложения.</span><span class="sxs-lookup"><span data-stu-id="a8163-121">All apps should be selected for this session control to work correctly.</span></span> |
|<span data-ttu-id="a8163-122">signInFrequency</span><span class="sxs-lookup"><span data-stu-id="a8163-122">signInFrequency</span></span>|[<span data-ttu-id="a8163-123">signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="a8163-123">signInFrequencySessionControl</span></span>](signinfrequencysessioncontrol.md)| <span data-ttu-id="a8163-124">Управление сеансом для принудительной регистрации.</span><span class="sxs-lookup"><span data-stu-id="a8163-124">Session control to enforce signin frequency.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8163-125">Связи</span><span class="sxs-lookup"><span data-stu-id="a8163-125">Relationships</span></span>

<span data-ttu-id="a8163-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8163-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8163-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a8163-127">JSON representation</span></span>

<span data-ttu-id="a8163-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8163-128">The following is a JSON representation of the resource.</span></span>

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

