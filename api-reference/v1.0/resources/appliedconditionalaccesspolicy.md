---
title: тип ресурса appliedConditionalAccessPolicy
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e69125d4119e7d2083189f459ad7c86816ddcd8e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952559"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="07592-103">тип ресурса appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="07592-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="07592-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07592-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07592-105">Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.</span><span class="sxs-lookup"><span data-stu-id="07592-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="07592-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="07592-106">Properties</span></span>

| <span data-ttu-id="07592-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="07592-107">Property</span></span>   | <span data-ttu-id="07592-108">Тип</span><span class="sxs-lookup"><span data-stu-id="07592-108">Type</span></span> |<span data-ttu-id="07592-109">Описание</span><span class="sxs-lookup"><span data-stu-id="07592-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07592-110">displayName</span><span class="sxs-lookup"><span data-stu-id="07592-110">displayName</span></span>|<span data-ttu-id="07592-111">String</span><span class="sxs-lookup"><span data-stu-id="07592-111">String</span></span>|<span data-ttu-id="07592-112">Ссылается на имя политики условного доступа (например: "Require MFA for Salesforce").</span><span class="sxs-lookup"><span data-stu-id="07592-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="07592-113">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="07592-113">enforcedGrantControls</span></span>|<span data-ttu-id="07592-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="07592-114">String collection</span></span>|<span data-ttu-id="07592-115">Относится к средствам управления грантами, которые применяются в политике условного доступа (пример: "Требуется многофакторная проверка подлинности").</span><span class="sxs-lookup"><span data-stu-id="07592-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="07592-116">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="07592-116">enforcedSessionControls</span></span>|<span data-ttu-id="07592-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="07592-117">String collection</span></span>|<span data-ttu-id="07592-118">Относится к средствам управления сеансами, которые применяются в политике условного доступа (пример: "Требуется принудительное управление приложениями").</span><span class="sxs-lookup"><span data-stu-id="07592-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="07592-119">id</span><span class="sxs-lookup"><span data-stu-id="07592-119">id</span></span>|<span data-ttu-id="07592-120">String</span><span class="sxs-lookup"><span data-stu-id="07592-120">String</span></span>|<span data-ttu-id="07592-121">Идентификатор политики условного доступа.</span><span class="sxs-lookup"><span data-stu-id="07592-121">An identifier of the conditional access policy.</span></span>|
|<span data-ttu-id="07592-122">result</span><span class="sxs-lookup"><span data-stu-id="07592-122">result</span></span>|<span data-ttu-id="07592-123">appliedConditionalAccessPolicyResult</span><span class="sxs-lookup"><span data-stu-id="07592-123">appliedConditionalAccessPolicyResult</span></span>| <span data-ttu-id="07592-124">Указывает результат срабатываемой политики ЦС.</span><span class="sxs-lookup"><span data-stu-id="07592-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="07592-125">Возможные значения: , ( Политика не применяется, так как условия политики не были выполнены), (Это связано с политикой в состоянии `success` `failure` `notApplied` `notEnabled` отключения), `unknown` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="07592-125">Possible values are: `success`, `failure`, `notApplied` (Policy isn't applied because policy conditions were not met),`notEnabled` (This is due to the policy in disabled state), `unknown`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07592-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07592-126">JSON representation</span></span>

<span data-ttu-id="07592-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07592-127">Here is a JSON representation of the resource.</span></span>

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

