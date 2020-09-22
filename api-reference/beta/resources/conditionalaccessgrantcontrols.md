---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2bcb150239e6e6a8487caa3f49f7704fbd2550a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994283"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="e3112-103">Тип ресурса Кондитионалакцессгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="e3112-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="e3112-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3112-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3112-105">Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="e3112-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e3112-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3112-106">Properties</span></span>

| <span data-ttu-id="e3112-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3112-107">Property</span></span> | <span data-ttu-id="e3112-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e3112-108">Type</span></span> | <span data-ttu-id="e3112-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e3112-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e3112-110">operator</span><span class="sxs-lookup"><span data-stu-id="e3112-110">operator</span></span> | <span data-ttu-id="e3112-111">String</span><span class="sxs-lookup"><span data-stu-id="e3112-111">String</span></span> | <span data-ttu-id="e3112-112">Определяет связь элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="e3112-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="e3112-113">Возможные значения: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="e3112-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="e3112-114">буилтинконтролс</span><span class="sxs-lookup"><span data-stu-id="e3112-114">builtInControls</span></span> | <span data-ttu-id="e3112-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e3112-115">String collection</span></span> | <span data-ttu-id="e3112-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="e3112-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="e3112-117">Возможные значения: `block` ,,,,, `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` , `passwordChange` .</span><span class="sxs-lookup"><span data-stu-id="e3112-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="e3112-118">кустомаусентикатионфакторс</span><span class="sxs-lookup"><span data-stu-id="e3112-118">customAuthenticationFactors</span></span> | <span data-ttu-id="e3112-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e3112-119">String collection</span></span> | <span data-ttu-id="e3112-120">Список идентификаторов настраиваемых элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="e3112-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="e3112-121">Дополнительные сведения о настраиваемых элементах управления: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="e3112-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="e3112-122">термсофусе</span><span class="sxs-lookup"><span data-stu-id="e3112-122">termsOfUse</span></span> | <span data-ttu-id="e3112-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e3112-123">String collection</span></span> | <span data-ttu-id="e3112-124">Список [условий использования](agreement.md) идентификаторов, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="e3112-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="e3112-125">Особые рекомендации по использованию `passwordChange` в качестве элемента управления</span><span class="sxs-lookup"><span data-stu-id="e3112-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="e3112-126">При использовании `passwordChange` элемента управления учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="e3112-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="e3112-127">`passwordChange` должен сопровождаться `mfa` `AND` оператором.</span><span class="sxs-lookup"><span data-stu-id="e3112-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="e3112-128">Это сочетание гарантирует, что пароль будет обновлен безопасным способом.</span><span class="sxs-lookup"><span data-stu-id="e3112-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="e3112-129">`passwordChange` должен использоваться в политике, содержащей `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="e3112-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="e3112-130">Это предназначено для сценариев, в которых пользователям необходимо использовать пароль для безопасного изменения, чтобы сбросить риск для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e3112-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="e3112-131">Политика должна целевить `all` приложения и не исключать какие бы то ни было приложения.</span><span class="sxs-lookup"><span data-stu-id="e3112-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="e3112-132">Политика не может содержать другие условия.</span><span class="sxs-lookup"><span data-stu-id="e3112-132">The policy cannot contain any other condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="e3112-133">Связи</span><span class="sxs-lookup"><span data-stu-id="e3112-133">Relationships</span></span>

<span data-ttu-id="e3112-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e3112-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3112-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3112-135">JSON representation</span></span>

<span data-ttu-id="e3112-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3112-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


