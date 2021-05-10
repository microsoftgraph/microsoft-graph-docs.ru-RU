---
title: тип ресурса unifiedRoleManagementPolicyExpirationRule
description: В единойroleManagementPolicyExpirationRule указывается правило включить, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 610ecd2e861ac672d0b211e313132caa6946d8ff
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299694"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a><span data-ttu-id="18aa1-104">тип ресурса unifiedRoleManagementPolicyExpirationRule</span><span class="sxs-lookup"><span data-stu-id="18aa1-104">unifiedRoleManagementPolicyExpirationRule resource type</span></span>

<span data-ttu-id="18aa1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18aa1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18aa1-106">В единойroleManagementPolicyExpirationRule указывается правило включить, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="18aa1-106">A unifiedRoleManagementPolicyExpirationRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="18aa1-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="18aa1-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="18aa1-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="18aa1-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="18aa1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="18aa1-109">Properties</span></span>
|<span data-ttu-id="18aa1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="18aa1-110">Property</span></span>|<span data-ttu-id="18aa1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="18aa1-111">Type</span></span>|<span data-ttu-id="18aa1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="18aa1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18aa1-113">id</span><span class="sxs-lookup"><span data-stu-id="18aa1-113">id</span></span>|<span data-ttu-id="18aa1-114">Строка</span><span class="sxs-lookup"><span data-stu-id="18aa1-114">String</span></span>|<span data-ttu-id="18aa1-115">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="18aa1-115">Unique identifier for the rule.</span></span> <span data-ttu-id="18aa1-116">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="18aa1-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="18aa1-117">isExpirationRequired</span><span class="sxs-lookup"><span data-stu-id="18aa1-117">isExpirationRequired</span></span>|<span data-ttu-id="18aa1-118">Логический</span><span class="sxs-lookup"><span data-stu-id="18aa1-118">Boolean</span></span>|<span data-ttu-id="18aa1-119">Указывает, требуется ли истечение срока действия для получения права или назначения.</span><span class="sxs-lookup"><span data-stu-id="18aa1-119">Indicates if expiration is required for eligibility or assignment.</span></span>|
|<span data-ttu-id="18aa1-120">maximumDuration</span><span class="sxs-lookup"><span data-stu-id="18aa1-120">maximumDuration</span></span>|<span data-ttu-id="18aa1-121">Длительность</span><span class="sxs-lookup"><span data-stu-id="18aa1-121">Duration</span></span>|<span data-ttu-id="18aa1-122">Максимальная продолжительность, разрешенная для получения права или назначения, которая не является постоянной.</span><span class="sxs-lookup"><span data-stu-id="18aa1-122">The maximum duration allowed for eligiblity or assignment which is not permanent.</span></span>|
|<span data-ttu-id="18aa1-123">target</span><span class="sxs-lookup"><span data-stu-id="18aa1-123">target</span></span>|[<span data-ttu-id="18aa1-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="18aa1-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="18aa1-125">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="18aa1-125">The target for the rule.</span></span> <span data-ttu-id="18aa1-126">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="18aa1-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="18aa1-127">Связи</span><span class="sxs-lookup"><span data-stu-id="18aa1-127">Relationships</span></span>
<span data-ttu-id="18aa1-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="18aa1-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18aa1-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="18aa1-129">JSON representation</span></span>
<span data-ttu-id="18aa1-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18aa1-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isExpirationRequired": "Boolean",
  "maximumDuration": "String (duration)"
}
```

