---
title: тип ресурса unifiedRoleManagementPolicyApprovalRule
description: Единое правило утверждения, связанное с политикой управления ролью, указывает правило unifiedRoleManagementPolicyApprovalRule. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0a23087bada876a76658e616add68e404635461f
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299701"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a><span data-ttu-id="0db5a-104">тип ресурса unifiedRoleManagementPolicyApprovalRule</span><span class="sxs-lookup"><span data-stu-id="0db5a-104">unifiedRoleManagementPolicyApprovalRule resource type</span></span>

<span data-ttu-id="0db5a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0db5a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0db5a-106">Единое правило утверждения, связанное с политикой управления ролью, указывает правило unifiedRoleManagementPolicyApprovalRule.</span><span class="sxs-lookup"><span data-stu-id="0db5a-106">A unifiedRoleManagementPolicyApprovalRule specifies the approval rule associated with a role management policy.</span></span> <span data-ttu-id="0db5a-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="0db5a-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="0db5a-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="0db5a-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0db5a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0db5a-109">Properties</span></span>
|<span data-ttu-id="0db5a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0db5a-110">Property</span></span>|<span data-ttu-id="0db5a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0db5a-111">Type</span></span>|<span data-ttu-id="0db5a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0db5a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db5a-113">id</span><span class="sxs-lookup"><span data-stu-id="0db5a-113">id</span></span>|<span data-ttu-id="0db5a-114">Строка</span><span class="sxs-lookup"><span data-stu-id="0db5a-114">String</span></span>|<span data-ttu-id="0db5a-115">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="0db5a-115">Unique identifier for the rule.</span></span> <span data-ttu-id="0db5a-116">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="0db5a-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="0db5a-117">setting</span><span class="sxs-lookup"><span data-stu-id="0db5a-117">setting</span></span>|[<span data-ttu-id="0db5a-118">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="0db5a-118">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="0db5a-119">Параметр утверждения правила.</span><span class="sxs-lookup"><span data-stu-id="0db5a-119">The approval setting for the rule.</span></span>|
|<span data-ttu-id="0db5a-120">target</span><span class="sxs-lookup"><span data-stu-id="0db5a-120">target</span></span>|[<span data-ttu-id="0db5a-121">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="0db5a-121">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="0db5a-122">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="0db5a-122">The target for the rule rule.</span></span> <span data-ttu-id="0db5a-123">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="0db5a-123">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0db5a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="0db5a-124">Relationships</span></span>
<span data-ttu-id="0db5a-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0db5a-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0db5a-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0db5a-126">JSON representation</span></span>
<span data-ttu-id="0db5a-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0db5a-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "setting": {
    "@odata.type": "microsoft.graph.approvalSettings"
  }
}
```

