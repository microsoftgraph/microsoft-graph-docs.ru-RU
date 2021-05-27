---
title: тип ресурса unifiedRoleManagementPolicyExpirationRule
description: В единойroleManagementPolicyExpirationRule указывается правило включить, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e41a59ee25ef3d00b72c279c9e47308cbae6735a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680677"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a><span data-ttu-id="f0061-104">тип ресурса unifiedRoleManagementPolicyExpirationRule</span><span class="sxs-lookup"><span data-stu-id="f0061-104">unifiedRoleManagementPolicyExpirationRule resource type</span></span>

<span data-ttu-id="f0061-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0061-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0061-106">В единойroleManagementPolicyExpirationRule указывается правило включить, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="f0061-106">A unifiedRoleManagementPolicyExpirationRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="f0061-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="f0061-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="f0061-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="f0061-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f0061-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0061-109">Properties</span></span>
|<span data-ttu-id="f0061-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0061-110">Property</span></span>|<span data-ttu-id="f0061-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f0061-111">Type</span></span>|<span data-ttu-id="f0061-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f0061-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0061-113">id</span><span class="sxs-lookup"><span data-stu-id="f0061-113">id</span></span>|<span data-ttu-id="f0061-114">String</span><span class="sxs-lookup"><span data-stu-id="f0061-114">String</span></span>|<span data-ttu-id="f0061-115">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="f0061-115">Unique identifier for the rule.</span></span> <span data-ttu-id="f0061-116">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="f0061-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="f0061-117">isExpirationRequired</span><span class="sxs-lookup"><span data-stu-id="f0061-117">isExpirationRequired</span></span>|<span data-ttu-id="f0061-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0061-118">Boolean</span></span>|<span data-ttu-id="f0061-119">Указывает, требуется ли истечение срока действия для получения права или назначения.</span><span class="sxs-lookup"><span data-stu-id="f0061-119">Indicates if expiration is required for eligibility or assignment.</span></span>|
|<span data-ttu-id="f0061-120">maximumDuration</span><span class="sxs-lookup"><span data-stu-id="f0061-120">maximumDuration</span></span>|<span data-ttu-id="f0061-121">Длительность</span><span class="sxs-lookup"><span data-stu-id="f0061-121">Duration</span></span>|<span data-ttu-id="f0061-122">Максимальная продолжительность, разрешенная для получения права или назначения, которая не является постоянной.</span><span class="sxs-lookup"><span data-stu-id="f0061-122">The maximum duration allowed for eligiblity or assignment which is not permanent.</span></span>|
|<span data-ttu-id="f0061-123">target</span><span class="sxs-lookup"><span data-stu-id="f0061-123">target</span></span>|[<span data-ttu-id="f0061-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="f0061-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="f0061-125">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="f0061-125">The target for the rule.</span></span> <span data-ttu-id="f0061-126">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="f0061-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0061-127">Связи</span><span class="sxs-lookup"><span data-stu-id="f0061-127">Relationships</span></span>
<span data-ttu-id="f0061-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f0061-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0061-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f0061-129">JSON representation</span></span>
<span data-ttu-id="f0061-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0061-130">The following is a JSON representation of the resource.</span></span>
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

