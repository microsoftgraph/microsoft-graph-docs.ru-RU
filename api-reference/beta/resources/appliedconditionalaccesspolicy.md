---
title: тип ресурса appliedConditionalAccessPolicy
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ffb91b315772d017ce039237e353df68daa47bfc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952317"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="8a275-103">тип ресурса appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="8a275-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="8a275-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a275-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a275-105">Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.</span><span class="sxs-lookup"><span data-stu-id="8a275-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="8a275-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a275-106">Properties</span></span>

| <span data-ttu-id="8a275-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a275-107">Property</span></span>   | <span data-ttu-id="8a275-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8a275-108">Type</span></span> |<span data-ttu-id="8a275-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a275-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a275-110">условия, удовлетворяемые</span><span class="sxs-lookup"><span data-stu-id="8a275-110">conditionsSatisfied</span></span>|<span data-ttu-id="8a275-111">conditionalAccessConditions</span><span class="sxs-lookup"><span data-stu-id="8a275-111">conditionalAccessConditions</span></span>|<span data-ttu-id="8a275-112">Относится к условиям политики условного доступа, которые удовлетворены.</span><span class="sxs-lookup"><span data-stu-id="8a275-112">Refers to the conditional access policy conditions that are satisfied.</span></span> <span data-ttu-id="8a275-113">Возможные значения: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span><span class="sxs-lookup"><span data-stu-id="8a275-113">Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span></span>|
|<span data-ttu-id="8a275-114">conditionsNotSatisfied</span><span class="sxs-lookup"><span data-stu-id="8a275-114">conditionsNotSatisfied</span></span>|<span data-ttu-id="8a275-115">conditionalAccessConditions</span><span class="sxs-lookup"><span data-stu-id="8a275-115">conditionalAccessConditions</span></span>|<span data-ttu-id="8a275-116">Относится к условиям политики условного доступа, которые не удовлетворены.</span><span class="sxs-lookup"><span data-stu-id="8a275-116">Refers to the conditional access policy conditions that are not satisfied.</span></span> <span data-ttu-id="8a275-117">Возможные значения: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span><span class="sxs-lookup"><span data-stu-id="8a275-117">Possible values are: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.</span></span>|
|<span data-ttu-id="8a275-118">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="8a275-118">enforcedGrantControls</span></span>|<span data-ttu-id="8a275-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8a275-119">String collection</span></span>|<span data-ttu-id="8a275-120">Относится к средствам управления грантами, которые применяются в политике условного доступа (пример: "Требуется многофакторная проверка подлинности").</span><span class="sxs-lookup"><span data-stu-id="8a275-120">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="8a275-121">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="8a275-121">enforcedSessionControls</span></span>|<span data-ttu-id="8a275-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8a275-122">String collection</span></span>|<span data-ttu-id="8a275-123">Относится к средствам управления сеансами, которые применяются в политике условного доступа (пример: "Требуется принудительное управление приложениями").</span><span class="sxs-lookup"><span data-stu-id="8a275-123">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="8a275-124">id</span><span class="sxs-lookup"><span data-stu-id="8a275-124">id</span></span>|<span data-ttu-id="8a275-125">Строка</span><span class="sxs-lookup"><span data-stu-id="8a275-125">String</span></span>|<span data-ttu-id="8a275-126">Идентификатор политики условного доступа.</span><span class="sxs-lookup"><span data-stu-id="8a275-126">Identifier of the conditional access policy.</span></span>|
|<span data-ttu-id="8a275-127">result</span><span class="sxs-lookup"><span data-stu-id="8a275-127">result</span></span>|<span data-ttu-id="8a275-128">appliedConditionalAccessPolicyResult</span><span class="sxs-lookup"><span data-stu-id="8a275-128">appliedConditionalAccessPolicyResult</span></span>| <span data-ttu-id="8a275-129">Указывает результат срабатываемой политики ЦС.</span><span class="sxs-lookup"><span data-stu-id="8a275-129">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="8a275-130">Возможные значения: , , (Политика не применяется, так как условия политики не были выполнены), (Это связано с политикой в состоянии `success` `failure` `notApplied` `notEnabled` отключена), `unknown` , , , `unknownFutureValue` `reportOnlySuccess` `reportOnlyFailure` , `reportOnlyNotApplied``reportOnlyInterrupted`</span><span class="sxs-lookup"><span data-stu-id="8a275-130">Possible values are: `success`, `failure`, `notApplied` (Policy isn't applied because policy conditions were not met),`notEnabled` (This is due to the policy in disabled state), `unknown`, `unknownFutureValue`, `reportOnlySuccess`, `reportOnlyFailure`, `reportOnlyNotApplied`, `reportOnlyInterrupted`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a275-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a275-131">JSON representation</span></span>

<span data-ttu-id="8a275-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a275-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
