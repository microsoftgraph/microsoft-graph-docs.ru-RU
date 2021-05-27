---
title: тип ресурса unifiedRoleManagementPolicyRule
description: В единойRoleManagementPolicyRule указывается правило, связанное с политикой управления ролью. Это абстрактно.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa0bc719fe4722692b1ff42861cccede7150780d
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682245"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a><span data-ttu-id="763ef-104">тип ресурса unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="763ef-104">unifiedRoleManagementPolicyRule resource type</span></span>

<span data-ttu-id="763ef-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="763ef-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="763ef-106">В единойRoleManagementPolicyRule указывается правило, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="763ef-106">A unifiedRoleManagementPolicyRule specifies the rule associated with a role management policy.</span></span> <span data-ttu-id="763ef-107">Это абстрактно.</span><span class="sxs-lookup"><span data-stu-id="763ef-107">It is abstract.</span></span>

## <a name="methods"></a><span data-ttu-id="763ef-108">Методы</span><span class="sxs-lookup"><span data-stu-id="763ef-108">Methods</span></span>
|<span data-ttu-id="763ef-109">Метод</span><span class="sxs-lookup"><span data-stu-id="763ef-109">Method</span></span>|<span data-ttu-id="763ef-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="763ef-110">Return type</span></span>|<span data-ttu-id="763ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="763ef-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="763ef-112">Список unifiedRoleManagementPolicyRules</span><span class="sxs-lookup"><span data-stu-id="763ef-112">List unifiedRoleManagementPolicyRules</span></span>](../api/unifiedrolemanagementpolicyrule-list.md)|<span data-ttu-id="763ef-113">[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="763ef-113">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="763ef-114">Получите список объектов [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="763ef-114">Get a list of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects and their properties.</span></span>|
|[<span data-ttu-id="763ef-115">Get unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="763ef-115">Get unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-get.md)|[<span data-ttu-id="763ef-116">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="763ef-116">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="763ef-117">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="763ef-117">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|
|[<span data-ttu-id="763ef-118">Обновление unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="763ef-118">Update unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-update.md)|[<span data-ttu-id="763ef-119">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="763ef-119">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="763ef-120">Обновление свойств единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="763ef-120">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="763ef-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="763ef-121">Properties</span></span>
|<span data-ttu-id="763ef-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="763ef-122">Property</span></span>|<span data-ttu-id="763ef-123">Тип</span><span class="sxs-lookup"><span data-stu-id="763ef-123">Type</span></span>|<span data-ttu-id="763ef-124">Описание</span><span class="sxs-lookup"><span data-stu-id="763ef-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="763ef-125">id</span><span class="sxs-lookup"><span data-stu-id="763ef-125">id</span></span>|<span data-ttu-id="763ef-126">String</span><span class="sxs-lookup"><span data-stu-id="763ef-126">String</span></span>|<span data-ttu-id="763ef-127">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="763ef-127">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="763ef-128">target</span><span class="sxs-lookup"><span data-stu-id="763ef-128">target</span></span>|[<span data-ttu-id="763ef-129">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="763ef-129">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="763ef-130">Цель правила политики.</span><span class="sxs-lookup"><span data-stu-id="763ef-130">The target for the policy rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="763ef-131">Связи</span><span class="sxs-lookup"><span data-stu-id="763ef-131">Relationships</span></span>
<span data-ttu-id="763ef-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="763ef-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="763ef-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="763ef-133">JSON representation</span></span>
<span data-ttu-id="763ef-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="763ef-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```

