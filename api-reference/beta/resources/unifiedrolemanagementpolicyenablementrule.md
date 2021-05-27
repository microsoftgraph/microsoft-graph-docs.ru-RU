---
title: тип ресурса unifiedRoleManagementPolicyEnablementRule
description: В единойroleManagementPolicyEnablementRule указывается правило включить, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bf3ef8e25026c72aab36a9c2fb6241f5bef950da
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680684"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a><span data-ttu-id="51520-104">тип ресурса unifiedRoleManagementPolicyEnablementRule</span><span class="sxs-lookup"><span data-stu-id="51520-104">unifiedRoleManagementPolicyEnablementRule resource type</span></span>

<span data-ttu-id="51520-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51520-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51520-106">В единойroleManagementPolicyEnablementRule указывается правило включить, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="51520-106">A unifiedRoleManagementPolicyEnablementRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="51520-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="51520-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="51520-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="51520-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="51520-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="51520-109">Properties</span></span>
|<span data-ttu-id="51520-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="51520-110">Property</span></span>|<span data-ttu-id="51520-111">Тип</span><span class="sxs-lookup"><span data-stu-id="51520-111">Type</span></span>|<span data-ttu-id="51520-112">Описание</span><span class="sxs-lookup"><span data-stu-id="51520-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51520-113">enabledRules</span><span class="sxs-lookup"><span data-stu-id="51520-113">enabledRules</span></span>|<span data-ttu-id="51520-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="51520-114">String collection</span></span>|<span data-ttu-id="51520-115">Правила, которые включены.</span><span class="sxs-lookup"><span data-stu-id="51520-115">The rules which are enabled.</span></span> <span data-ttu-id="51520-116">Допустимые значения : MultifactorAuthentication, Justification, Ticketing.</span><span class="sxs-lookup"><span data-stu-id="51520-116">Allowed values are MultifactorAuthentication, Justification, Ticketing.</span></span>|
|<span data-ttu-id="51520-117">id</span><span class="sxs-lookup"><span data-stu-id="51520-117">id</span></span>|<span data-ttu-id="51520-118">String</span><span class="sxs-lookup"><span data-stu-id="51520-118">String</span></span>|<span data-ttu-id="51520-119">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="51520-119">Unique identifier for the rule.</span></span> <span data-ttu-id="51520-120">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="51520-120">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="51520-121">target</span><span class="sxs-lookup"><span data-stu-id="51520-121">target</span></span>|[<span data-ttu-id="51520-122">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="51520-122">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="51520-123">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="51520-123">The target for the rule.</span></span> <span data-ttu-id="51520-124">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="51520-124">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="51520-125">Связи</span><span class="sxs-lookup"><span data-stu-id="51520-125">Relationships</span></span>
<span data-ttu-id="51520-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="51520-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51520-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="51520-127">JSON representation</span></span>
<span data-ttu-id="51520-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51520-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "enabledRules": [
    "String"
  ]
}
```

