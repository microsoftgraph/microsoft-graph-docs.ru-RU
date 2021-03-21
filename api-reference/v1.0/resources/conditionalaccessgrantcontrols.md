---
title: тип ресурса conditionalAccessSGrantControls
description: Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 67795b93f99f7075b28657c32a94085968c981be
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962492"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="46a0c-103">тип ресурса conditionalAccessSGrantControls</span><span class="sxs-lookup"><span data-stu-id="46a0c-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="46a0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46a0c-105">Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.</span><span class="sxs-lookup"><span data-stu-id="46a0c-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="46a0c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="46a0c-106">Properties</span></span>

| <span data-ttu-id="46a0c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="46a0c-107">Property</span></span> | <span data-ttu-id="46a0c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="46a0c-108">Type</span></span> | <span data-ttu-id="46a0c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="46a0c-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="46a0c-110">operator</span><span class="sxs-lookup"><span data-stu-id="46a0c-110">operator</span></span> | <span data-ttu-id="46a0c-111">String</span><span class="sxs-lookup"><span data-stu-id="46a0c-111">String</span></span> | <span data-ttu-id="46a0c-112">Определяет связь элементов управления грантами.</span><span class="sxs-lookup"><span data-stu-id="46a0c-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="46a0c-113">Возможные значения: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="46a0c-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="46a0c-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="46a0c-114">builtInControls</span></span> | <span data-ttu-id="46a0c-115">коллекция conditionalAccessGrantControl</span><span class="sxs-lookup"><span data-stu-id="46a0c-115">conditionalAccessGrantControl collection</span></span> | <span data-ttu-id="46a0c-116">Список значений встроенных элементов управления, необходимых политике.</span><span class="sxs-lookup"><span data-stu-id="46a0c-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="46a0c-117">Возможные значения: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="46a0c-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="46a0c-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="46a0c-118">customAuthenticationFactors</span></span> | <span data-ttu-id="46a0c-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="46a0c-119">String collection</span></span> | <span data-ttu-id="46a0c-120">Список пользовательских ID-элементов элементов управления, необходимых политике.</span><span class="sxs-lookup"><span data-stu-id="46a0c-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="46a0c-121">Дополнительные сведения см. в [специальном элементе управления.](/azure/active-directory/conditional-access/controls)</span><span class="sxs-lookup"><span data-stu-id="46a0c-121">For more information, see [Custom controls](/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="46a0c-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="46a0c-122">termsOfUse</span></span> | <span data-ttu-id="46a0c-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="46a0c-123">String collection</span></span> | <span data-ttu-id="46a0c-124">Список [условий использования](/graph/api/resources/agreement) ID, необходимых политике.</span><span class="sxs-lookup"><span data-stu-id="46a0c-124">List of [terms of use](/graph/api/resources/agreement) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="46a0c-125">Особые соображения при использовании `passwordChange` в качестве управления</span><span class="sxs-lookup"><span data-stu-id="46a0c-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="46a0c-126">При использовании управления рассмотрим `passwordChange` следующее:</span><span class="sxs-lookup"><span data-stu-id="46a0c-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="46a0c-127">`passwordChange` должны сопровождаться `mfa` с помощью `AND` оператора.</span><span class="sxs-lookup"><span data-stu-id="46a0c-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="46a0c-128">Это сочетание гарантирует, что пароль будет обновляться безопасным способом.</span><span class="sxs-lookup"><span data-stu-id="46a0c-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="46a0c-129">`passwordChange` необходимо использовать в политике, содержащей `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="46a0c-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="46a0c-130">Это предназначено для того, чтобы включить сценарии, в которых пользователи должны использовать безопасный пароль изменения для сброса риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="46a0c-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="46a0c-131">Политика должна быть ориентирована `all` на приложения, а не исключать любые приложения.</span><span class="sxs-lookup"><span data-stu-id="46a0c-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="46a0c-132">Политика не может содержать любое другое условие, кроме `users` `applications` , и `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="46a0c-132">The policy cannot contain any other condition except `users`, `applications` and `userRiskLevels`.</span></span>

## <a name="relationships"></a><span data-ttu-id="46a0c-133">Связи</span><span class="sxs-lookup"><span data-stu-id="46a0c-133">Relationships</span></span>

<span data-ttu-id="46a0c-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="46a0c-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46a0c-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="46a0c-135">JSON representation</span></span>

<span data-ttu-id="46a0c-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46a0c-136">The following is a JSON representation of the resource.</span></span>

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
