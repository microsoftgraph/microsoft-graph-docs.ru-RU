---
title: тип ресурса unifiedRoleManagementPolicyApprovalRule
description: Единое правило утверждения, связанное с политикой управления ролью, указывает правило unifiedRoleManagementPolicyApprovalRule. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 41d9cac01f48d8dcdd59513718053611b023a3a8
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680705"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a><span data-ttu-id="40ee2-104">тип ресурса unifiedRoleManagementPolicyApprovalRule</span><span class="sxs-lookup"><span data-stu-id="40ee2-104">unifiedRoleManagementPolicyApprovalRule resource type</span></span>

<span data-ttu-id="40ee2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ee2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40ee2-106">Единое правило утверждения, связанное с политикой управления ролью, указывает правило unifiedRoleManagementPolicyApprovalRule.</span><span class="sxs-lookup"><span data-stu-id="40ee2-106">A unifiedRoleManagementPolicyApprovalRule specifies the approval rule associated with a role management policy.</span></span> <span data-ttu-id="40ee2-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="40ee2-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="40ee2-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="40ee2-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="40ee2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="40ee2-109">Properties</span></span>
|<span data-ttu-id="40ee2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="40ee2-110">Property</span></span>|<span data-ttu-id="40ee2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="40ee2-111">Type</span></span>|<span data-ttu-id="40ee2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="40ee2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40ee2-113">id</span><span class="sxs-lookup"><span data-stu-id="40ee2-113">id</span></span>|<span data-ttu-id="40ee2-114">String</span><span class="sxs-lookup"><span data-stu-id="40ee2-114">String</span></span>|<span data-ttu-id="40ee2-115">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="40ee2-115">Unique identifier for the rule.</span></span> <span data-ttu-id="40ee2-116">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="40ee2-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="40ee2-117">setting</span><span class="sxs-lookup"><span data-stu-id="40ee2-117">setting</span></span>|[<span data-ttu-id="40ee2-118">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="40ee2-118">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="40ee2-119">Параметр утверждения правила.</span><span class="sxs-lookup"><span data-stu-id="40ee2-119">The approval setting for the rule.</span></span>|
|<span data-ttu-id="40ee2-120">target</span><span class="sxs-lookup"><span data-stu-id="40ee2-120">target</span></span>|[<span data-ttu-id="40ee2-121">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="40ee2-121">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="40ee2-122">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="40ee2-122">The target for the rule rule.</span></span> <span data-ttu-id="40ee2-123">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="40ee2-123">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="40ee2-124">Связи</span><span class="sxs-lookup"><span data-stu-id="40ee2-124">Relationships</span></span>
<span data-ttu-id="40ee2-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="40ee2-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="40ee2-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="40ee2-126">JSON representation</span></span>
<span data-ttu-id="40ee2-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40ee2-127">The following is a JSON representation of the resource.</span></span>
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

