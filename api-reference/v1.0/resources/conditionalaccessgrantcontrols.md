---
title: Тип ресурса conditionalAccessGrantControls
description: Представляет элементы управления предоставлением, которые должны быть выполнены для прохода политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 99b6d6dc3bd15ea84c4a8507981acd9c8ac2eb6f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130790"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="187ce-103">Тип ресурса conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="187ce-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="187ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="187ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="187ce-105">Представляет элементы управления предоставлением, которые должны быть выполнены для прохода политики.</span><span class="sxs-lookup"><span data-stu-id="187ce-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="187ce-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="187ce-106">Properties</span></span>

| <span data-ttu-id="187ce-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="187ce-107">Property</span></span> | <span data-ttu-id="187ce-108">Тип</span><span class="sxs-lookup"><span data-stu-id="187ce-108">Type</span></span> | <span data-ttu-id="187ce-109">Описание</span><span class="sxs-lookup"><span data-stu-id="187ce-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="187ce-110">operator</span><span class="sxs-lookup"><span data-stu-id="187ce-110">operator</span></span> | <span data-ttu-id="187ce-111">String</span><span class="sxs-lookup"><span data-stu-id="187ce-111">String</span></span> | <span data-ttu-id="187ce-112">Определяет отношение элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="187ce-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="187ce-113">Возможные значения: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="187ce-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="187ce-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="187ce-114">builtInControls</span></span> | <span data-ttu-id="187ce-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="187ce-115">String collection</span></span> | <span data-ttu-id="187ce-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="187ce-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="187ce-117">Возможные значения: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` .</span><span class="sxs-lookup"><span data-stu-id="187ce-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="187ce-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="187ce-118">customAuthenticationFactors</span></span> | <span data-ttu-id="187ce-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="187ce-119">String collection</span></span> | <span data-ttu-id="187ce-120">Список пользовательских ИД элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="187ce-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="187ce-121">Дополнительные сведения см. в [настраиваемом элементе управления.](/azure/active-directory/conditional-access/controls)</span><span class="sxs-lookup"><span data-stu-id="187ce-121">For more information, see [Custom controls](/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="187ce-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="187ce-122">termsOfUse</span></span> | <span data-ttu-id="187ce-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="187ce-123">String collection</span></span> | <span data-ttu-id="187ce-124">Список [условий использования,](/graph/api/resources/agreement) необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="187ce-124">List of [terms of use](/graph/api/resources/agreement) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="187ce-125">Особые соображения при использовании `passwordChange` в качестве управления</span><span class="sxs-lookup"><span data-stu-id="187ce-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="187ce-126">При использовании этого управления учитывайте `passwordChange` следующее:</span><span class="sxs-lookup"><span data-stu-id="187ce-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="187ce-127">`passwordChange` должен сопровождаться `mfa` с помощью `AND` оператора.</span><span class="sxs-lookup"><span data-stu-id="187ce-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="187ce-128">Это сочетание гарантирует безопасное обновление пароля.</span><span class="sxs-lookup"><span data-stu-id="187ce-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="187ce-129">`passwordChange` должен использоваться в политике, содержащей `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="187ce-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="187ce-130">Это позволяет пользователям использовать безопасный пароль для сброса рисков пользователей.</span><span class="sxs-lookup"><span data-stu-id="187ce-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="187ce-131">Политика должна быть нацелена `all` на приложения и не исключать их.</span><span class="sxs-lookup"><span data-stu-id="187ce-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="187ce-132">Политика не может содержать другие условия, кроме `users` . `applications` `userRiskLevels`</span><span class="sxs-lookup"><span data-stu-id="187ce-132">The policy cannot contain any other condition except `users`, `applications` and `userRiskLevels`.</span></span>

## <a name="relationships"></a><span data-ttu-id="187ce-133">Связи</span><span class="sxs-lookup"><span data-stu-id="187ce-133">Relationships</span></span>

<span data-ttu-id="187ce-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="187ce-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="187ce-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="187ce-135">JSON representation</span></span>

<span data-ttu-id="187ce-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="187ce-136">The following is a JSON representation of the resource.</span></span>

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
