---
title: тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule
description: В единойroleManagementPolicyAuthenticationContextRule указывается правило включить, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5e3db8812b58b8276ab2fdd977e110f30a874c9b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680698"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a><span data-ttu-id="75cd5-104">тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule</span><span class="sxs-lookup"><span data-stu-id="75cd5-104">unifiedRoleManagementPolicyAuthenticationContextRule resource type</span></span>

<span data-ttu-id="75cd5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75cd5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75cd5-106">В единойroleManagementPolicyAuthenticationContextRule указывается правило включить, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="75cd5-106">A unifiedRoleManagementPolicyAuthenticationContextRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="75cd5-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="75cd5-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="75cd5-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="75cd5-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="75cd5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="75cd5-109">Properties</span></span>
|<span data-ttu-id="75cd5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="75cd5-110">Property</span></span>|<span data-ttu-id="75cd5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="75cd5-111">Type</span></span>|<span data-ttu-id="75cd5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="75cd5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75cd5-113">claimValue</span><span class="sxs-lookup"><span data-stu-id="75cd5-113">claimValue</span></span>|<span data-ttu-id="75cd5-114">String</span><span class="sxs-lookup"><span data-stu-id="75cd5-114">String</span></span>|<span data-ttu-id="75cd5-115">Значение утверждения контекста проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="75cd5-115">Value of the authentication context claim.</span></span>|
|<span data-ttu-id="75cd5-116">id</span><span class="sxs-lookup"><span data-stu-id="75cd5-116">id</span></span>|<span data-ttu-id="75cd5-117">String</span><span class="sxs-lookup"><span data-stu-id="75cd5-117">String</span></span>|<span data-ttu-id="75cd5-118">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="75cd5-118">Unique identifier for the rule.</span></span> <span data-ttu-id="75cd5-119">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="75cd5-119">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="75cd5-120">isEnabled</span><span class="sxs-lookup"><span data-stu-id="75cd5-120">isEnabled</span></span>|<span data-ttu-id="75cd5-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="75cd5-121">Boolean</span></span>|<span data-ttu-id="75cd5-122">Указывает, включен ли параметр.</span><span class="sxs-lookup"><span data-stu-id="75cd5-122">Indicates if the setting is enabled.</span></span>|
|<span data-ttu-id="75cd5-123">target</span><span class="sxs-lookup"><span data-stu-id="75cd5-123">target</span></span>|[<span data-ttu-id="75cd5-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="75cd5-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="75cd5-125">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="75cd5-125">The target for the rule.</span></span> <span data-ttu-id="75cd5-126">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="75cd5-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="75cd5-127">Связи</span><span class="sxs-lookup"><span data-stu-id="75cd5-127">Relationships</span></span>
<span data-ttu-id="75cd5-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="75cd5-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75cd5-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="75cd5-129">JSON representation</span></span>
<span data-ttu-id="75cd5-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75cd5-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isEnabled": "Boolean",
  "claimValue": "String"
}
```

