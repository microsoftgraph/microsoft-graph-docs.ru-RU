---
title: тип ресурса unifiedRoleManagementPolicyRule
description: В единойRoleManagementPolicyRule указывается правило, связанное с политикой управления ролью. Это абстрактно.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 420ebfca11d2873ad942782fb8e7d97e893b7185
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299507"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a><span data-ttu-id="dd16a-104">тип ресурса unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="dd16a-104">unifiedRoleManagementPolicyRule resource type</span></span>

<span data-ttu-id="dd16a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd16a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd16a-106">В единойRoleManagementPolicyRule указывается правило, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="dd16a-106">A unifiedRoleManagementPolicyRule specifies the rule associated with a role management policy.</span></span> <span data-ttu-id="dd16a-107">Это абстрактно.</span><span class="sxs-lookup"><span data-stu-id="dd16a-107">It is abstract.</span></span>

## <a name="methods"></a><span data-ttu-id="dd16a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="dd16a-108">Methods</span></span>
|<span data-ttu-id="dd16a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="dd16a-109">Method</span></span>|<span data-ttu-id="dd16a-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="dd16a-110">Return type</span></span>|<span data-ttu-id="dd16a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dd16a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dd16a-112">Список unifiedRoleManagementPolicyRules</span><span class="sxs-lookup"><span data-stu-id="dd16a-112">List unifiedRoleManagementPolicyRules</span></span>](../api/unifiedrolemanagementpolicyrule-list.md)|<span data-ttu-id="dd16a-113">[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="dd16a-113">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="dd16a-114">Получите список объектов [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="dd16a-114">Get a list of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects and their properties.</span></span>|
|[<span data-ttu-id="dd16a-115">Get unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="dd16a-115">Get unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-get.md)|[<span data-ttu-id="dd16a-116">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="dd16a-116">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="dd16a-117">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="dd16a-117">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|
|[<span data-ttu-id="dd16a-118">Обновление unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="dd16a-118">Update unifiedRoleManagementPolicyRule</span></span>](../api/unifiedrolemanagementpolicyrule-update.md)|[<span data-ttu-id="dd16a-119">unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="dd16a-119">unifiedRoleManagementPolicyRule</span></span>](../resources/unifiedrolemanagementpolicyrule.md)|<span data-ttu-id="dd16a-120">Обновление свойств единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="dd16a-120">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd16a-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd16a-121">Properties</span></span>
|<span data-ttu-id="dd16a-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd16a-122">Property</span></span>|<span data-ttu-id="dd16a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="dd16a-123">Type</span></span>|<span data-ttu-id="dd16a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dd16a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd16a-125">id</span><span class="sxs-lookup"><span data-stu-id="dd16a-125">id</span></span>|<span data-ttu-id="dd16a-126">Строка</span><span class="sxs-lookup"><span data-stu-id="dd16a-126">String</span></span>|<span data-ttu-id="dd16a-127">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="dd16a-127">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="dd16a-128">target</span><span class="sxs-lookup"><span data-stu-id="dd16a-128">target</span></span>|[<span data-ttu-id="dd16a-129">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="dd16a-129">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="dd16a-130">Цель правила политики.</span><span class="sxs-lookup"><span data-stu-id="dd16a-130">The target for the policy rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd16a-131">Связи</span><span class="sxs-lookup"><span data-stu-id="dd16a-131">Relationships</span></span>
<span data-ttu-id="dd16a-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dd16a-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd16a-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dd16a-133">JSON representation</span></span>
<span data-ttu-id="dd16a-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd16a-134">The following is a JSON representation of the resource.</span></span>
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

