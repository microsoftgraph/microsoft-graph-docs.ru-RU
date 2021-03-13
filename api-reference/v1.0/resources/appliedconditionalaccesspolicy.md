---
title: тип ресурса appliedConditionalAccessPolicy
description: Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3aa114c23888ccc6852314e2274b8a89ca440344
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761530"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="3e4e1-103">тип ресурса appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="3e4e1-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="3e4e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e4e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e4e1-105">Указывает атрибуты, связанные с примененной политикой условного доступа или политиками, которые вызываются соответствующей активностью входов.</span><span class="sxs-lookup"><span data-stu-id="3e4e1-105">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="3e4e1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e4e1-106">Properties</span></span>

| <span data-ttu-id="3e4e1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e4e1-107">Property</span></span>   | <span data-ttu-id="3e4e1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3e4e1-108">Type</span></span> |<span data-ttu-id="3e4e1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3e4e1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e4e1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3e4e1-110">displayName</span></span>|<span data-ttu-id="3e4e1-111">String</span><span class="sxs-lookup"><span data-stu-id="3e4e1-111">String</span></span>|<span data-ttu-id="3e4e1-112">Ссылается на имя политики условного доступа (например: "Require MFA for Salesforce").</span><span class="sxs-lookup"><span data-stu-id="3e4e1-112">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="3e4e1-113">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="3e4e1-113">enforcedGrantControls</span></span>|<span data-ttu-id="3e4e1-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3e4e1-114">String collection</span></span>|<span data-ttu-id="3e4e1-115">Относится к средствам управления грантами, которые применяются в политике условного доступа (пример: "Требуется многофакторная проверка подлинности").</span><span class="sxs-lookup"><span data-stu-id="3e4e1-115">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="3e4e1-116">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="3e4e1-116">enforcedSessionControls</span></span>|<span data-ttu-id="3e4e1-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3e4e1-117">String collection</span></span>|<span data-ttu-id="3e4e1-118">Относится к средствам управления сеансами, которые применяются в политике условного доступа (пример: "Требуется принудительное управление приложениями").</span><span class="sxs-lookup"><span data-stu-id="3e4e1-118">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="3e4e1-119">id</span><span class="sxs-lookup"><span data-stu-id="3e4e1-119">id</span></span>|<span data-ttu-id="3e4e1-120">String</span><span class="sxs-lookup"><span data-stu-id="3e4e1-120">String</span></span>|<span data-ttu-id="3e4e1-121">Уникальный GUID политики условного доступа.</span><span class="sxs-lookup"><span data-stu-id="3e4e1-121">Unique GUID of the conditional access policy.</span></span>|
|<span data-ttu-id="3e4e1-122">result</span><span class="sxs-lookup"><span data-stu-id="3e4e1-122">result</span></span>|<span data-ttu-id="3e4e1-123">String</span><span class="sxs-lookup"><span data-stu-id="3e4e1-123">String</span></span>| <span data-ttu-id="3e4e1-124">Указывает результат срабатываемой политики ЦС.</span><span class="sxs-lookup"><span data-stu-id="3e4e1-124">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="3e4e1-125">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="3e4e1-125">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="3e4e1-126">`notApplied` - Политика не применяется, так как условия политики не были выполнены.</span><span class="sxs-lookup"><span data-stu-id="3e4e1-126">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="3e4e1-127">`notEnabled` - Это связано с политикой в состоянии отключения.</span><span class="sxs-lookup"><span data-stu-id="3e4e1-127">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e4e1-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e4e1-128">JSON representation</span></span>

<span data-ttu-id="3e4e1-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e4e1-129">Here is a JSON representation of the resource.</span></span>

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

