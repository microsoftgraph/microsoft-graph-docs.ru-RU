---
title: Тип ресурса conditionalAccessGrantControls
description: Представляет элементы управления предоставлением, которые должны быть выполнены для прохода политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0b93508db666fc1673f1c8154ef638762a872f3
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013669"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="b3ddb-103">Тип ресурса conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="b3ddb-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="b3ddb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3ddb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3ddb-105">Представляет элементы управления предоставлением, которые должны быть выполнены для прохода политики.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b3ddb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3ddb-106">Properties</span></span>

| <span data-ttu-id="b3ddb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3ddb-107">Property</span></span> | <span data-ttu-id="b3ddb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b3ddb-108">Type</span></span> | <span data-ttu-id="b3ddb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b3ddb-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="b3ddb-110">operator</span><span class="sxs-lookup"><span data-stu-id="b3ddb-110">operator</span></span> | <span data-ttu-id="b3ddb-111">String</span><span class="sxs-lookup"><span data-stu-id="b3ddb-111">String</span></span> | <span data-ttu-id="b3ddb-112">Определяет отношение элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="b3ddb-113">Возможные значения: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="b3ddb-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="b3ddb-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="b3ddb-114">builtInControls</span></span> | <span data-ttu-id="b3ddb-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3ddb-115">String collection</span></span> | <span data-ttu-id="b3ddb-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="b3ddb-117">Возможные значения: `block` , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` . `passwordChange`</span><span class="sxs-lookup"><span data-stu-id="b3ddb-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="b3ddb-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="b3ddb-118">customAuthenticationFactors</span></span> | <span data-ttu-id="b3ddb-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3ddb-119">String collection</span></span> | <span data-ttu-id="b3ddb-120">Список пользовательских ИД элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="b3ddb-121">Дополнительные сведения см. в [настраиваемом элементе управления.](/azure/active-directory/conditional-access/controls)</span><span class="sxs-lookup"><span data-stu-id="b3ddb-121">For more information, see [Custom controls](/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="b3ddb-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="b3ddb-122">termsOfUse</span></span> | <span data-ttu-id="b3ddb-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3ddb-123">String collection</span></span> | <span data-ttu-id="b3ddb-124">Список [условий использования,](/graph/api/resources/agreement) необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-124">List of [terms of use](/graph/api/resources/agreement) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="b3ddb-125">Особые соображения при использовании `passwordChange` в качестве управления</span><span class="sxs-lookup"><span data-stu-id="b3ddb-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="b3ddb-126">При использовании этого управления учитывайте `passwordChange` следующее:</span><span class="sxs-lookup"><span data-stu-id="b3ddb-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="b3ddb-127">`passwordChange` должен сопровождаться `mfa` с помощью `AND` оператора.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="b3ddb-128">Это сочетание гарантирует безопасное обновление пароля.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="b3ddb-129">`passwordChange` должен использоваться в политике, содержащей `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="b3ddb-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="b3ddb-130">Это позволяет пользователям использовать безопасный пароль для сброса рисков пользователей.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="b3ddb-131">Политика должна быть нацелена `all` на приложения и не исключать их.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="b3ddb-132">Политика не может содержать другие условия, кроме `users` . `applications` `userRiskLevels`</span><span class="sxs-lookup"><span data-stu-id="b3ddb-132">The policy cannot contain any other condition except `users`, `applications` and `userRiskLevels`.</span></span>

## <a name="relationships"></a><span data-ttu-id="b3ddb-133">Связи</span><span class="sxs-lookup"><span data-stu-id="b3ddb-133">Relationships</span></span>

<span data-ttu-id="b3ddb-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3ddb-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b3ddb-135">JSON representation</span></span>

<span data-ttu-id="b3ddb-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3ddb-136">The following is a JSON representation of the resource.</span></span>

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