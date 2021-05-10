---
title: тип ресурса unifiedRoleManagementPolicyEnablementRule
description: В единойroleManagementPolicyEnablementRule указывается правило включить, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e2cb5770f2fdd50aaf5e82d7c1f8fba505a47151
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299695"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a><span data-ttu-id="2db3e-104">тип ресурса unifiedRoleManagementPolicyEnablementRule</span><span class="sxs-lookup"><span data-stu-id="2db3e-104">unifiedRoleManagementPolicyEnablementRule resource type</span></span>

<span data-ttu-id="2db3e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2db3e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2db3e-106">В единойroleManagementPolicyEnablementRule указывается правило включить, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="2db3e-106">A unifiedRoleManagementPolicyEnablementRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="2db3e-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="2db3e-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="2db3e-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="2db3e-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2db3e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2db3e-109">Properties</span></span>
|<span data-ttu-id="2db3e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2db3e-110">Property</span></span>|<span data-ttu-id="2db3e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2db3e-111">Type</span></span>|<span data-ttu-id="2db3e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2db3e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2db3e-113">enabledRules</span><span class="sxs-lookup"><span data-stu-id="2db3e-113">enabledRules</span></span>|<span data-ttu-id="2db3e-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="2db3e-114">String collection</span></span>|<span data-ttu-id="2db3e-115">Правила, которые включены.</span><span class="sxs-lookup"><span data-stu-id="2db3e-115">The rules which are enabled.</span></span> <span data-ttu-id="2db3e-116">Допустимые значения : MultifactorAuthentication, Justification, Ticketing.</span><span class="sxs-lookup"><span data-stu-id="2db3e-116">Allowed values are MultifactorAuthentication, Justification, Ticketing.</span></span>|
|<span data-ttu-id="2db3e-117">id</span><span class="sxs-lookup"><span data-stu-id="2db3e-117">id</span></span>|<span data-ttu-id="2db3e-118">Строка</span><span class="sxs-lookup"><span data-stu-id="2db3e-118">String</span></span>|<span data-ttu-id="2db3e-119">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="2db3e-119">Unique identifier for the rule.</span></span> <span data-ttu-id="2db3e-120">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="2db3e-120">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="2db3e-121">target</span><span class="sxs-lookup"><span data-stu-id="2db3e-121">target</span></span>|[<span data-ttu-id="2db3e-122">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="2db3e-122">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="2db3e-123">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="2db3e-123">The target for the rule.</span></span> <span data-ttu-id="2db3e-124">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="2db3e-124">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2db3e-125">Связи</span><span class="sxs-lookup"><span data-stu-id="2db3e-125">Relationships</span></span>
<span data-ttu-id="2db3e-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2db3e-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2db3e-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2db3e-127">JSON representation</span></span>
<span data-ttu-id="2db3e-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2db3e-128">The following is a JSON representation of the resource.</span></span>
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

