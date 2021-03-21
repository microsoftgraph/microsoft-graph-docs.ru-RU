---
title: тип ресурса conditionalAccessSGrantControls
description: Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b2dba27c987351619a347a16d20b2a4b88646045
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961289"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="7dd5b-103">тип ресурса conditionalAccessSGrantControls</span><span class="sxs-lookup"><span data-stu-id="7dd5b-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="7dd5b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dd5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dd5b-105">Представляет элементы управления грантами, которые необходимо выполнить для выполнения политики.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="7dd5b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7dd5b-106">Properties</span></span>

| <span data-ttu-id="7dd5b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dd5b-107">Property</span></span> | <span data-ttu-id="7dd5b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7dd5b-108">Type</span></span> | <span data-ttu-id="7dd5b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd5b-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="7dd5b-110">operator</span><span class="sxs-lookup"><span data-stu-id="7dd5b-110">operator</span></span> | <span data-ttu-id="7dd5b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="7dd5b-111">String</span></span> | <span data-ttu-id="7dd5b-112">Определяет связь элементов управления грантами.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="7dd5b-113">Возможные значения: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="7dd5b-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="7dd5b-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="7dd5b-114">builtInControls</span></span> | <span data-ttu-id="7dd5b-115">коллекция conditionalAccessGrantControl</span><span class="sxs-lookup"><span data-stu-id="7dd5b-115">conditionalAccessGrantControl collection</span></span> | <span data-ttu-id="7dd5b-116">Список значений встроенных элементов управления, необходимых политике.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="7dd5b-117">Возможные значения: `block` , , , , , `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` `passwordChange` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="7dd5b-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="7dd5b-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="7dd5b-118">customAuthenticationFactors</span></span> | <span data-ttu-id="7dd5b-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7dd5b-119">String collection</span></span> | <span data-ttu-id="7dd5b-120">Список пользовательских ID-элементов элементов управления, необходимых политике.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="7dd5b-121">Дополнительные информацию о настраиваемом элементе управления здесь: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="7dd5b-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="7dd5b-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="7dd5b-122">termsOfUse</span></span> | <span data-ttu-id="7dd5b-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7dd5b-123">String collection</span></span> | <span data-ttu-id="7dd5b-124">Список [условий использования](agreement.md) ID, необходимых политике.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="7dd5b-125">Особые соображения при использовании `passwordChange` в качестве управления</span><span class="sxs-lookup"><span data-stu-id="7dd5b-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="7dd5b-126">При использовании управления рассмотрим `passwordChange` следующее:</span><span class="sxs-lookup"><span data-stu-id="7dd5b-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="7dd5b-127">`passwordChange` должны сопровождаться `mfa` с помощью `AND` оператора.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="7dd5b-128">Это сочетание гарантирует, что пароль будет обновляться безопасным способом.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="7dd5b-129">`passwordChange` необходимо использовать в политике, содержащей `userRiskLevels` .</span><span class="sxs-lookup"><span data-stu-id="7dd5b-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="7dd5b-130">Это предназначено для того, чтобы включить сценарии, в которых пользователи должны использовать безопасный пароль изменения для сброса риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="7dd5b-131">Политика должна быть ориентирована `all` на приложения, а не исключать любые приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="7dd5b-132">Политика не может содержать любое другое условие.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-132">The policy cannot contain any other condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="7dd5b-133">Связи</span><span class="sxs-lookup"><span data-stu-id="7dd5b-133">Relationships</span></span>

<span data-ttu-id="7dd5b-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dd5b-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7dd5b-135">JSON representation</span></span>

<span data-ttu-id="7dd5b-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dd5b-136">The following is a JSON representation of the resource.</span></span>

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


