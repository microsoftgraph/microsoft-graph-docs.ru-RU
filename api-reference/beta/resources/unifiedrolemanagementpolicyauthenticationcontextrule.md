---
title: тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule
description: В единойroleManagementPolicyAuthenticationContextRule указывается правило включить, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d6c9eb94272dcc7e9cbbe27657b50d50688ac9d9
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299700"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a><span data-ttu-id="2a764-104">тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule</span><span class="sxs-lookup"><span data-stu-id="2a764-104">unifiedRoleManagementPolicyAuthenticationContextRule resource type</span></span>

<span data-ttu-id="2a764-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a764-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a764-106">В единойroleManagementPolicyAuthenticationContextRule указывается правило включить, связанное с политикой управления ролью.</span><span class="sxs-lookup"><span data-stu-id="2a764-106">A unifiedRoleManagementPolicyAuthenticationContextRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="2a764-107">Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="2a764-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="2a764-108">Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="2a764-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2a764-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a764-109">Properties</span></span>
|<span data-ttu-id="2a764-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a764-110">Property</span></span>|<span data-ttu-id="2a764-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2a764-111">Type</span></span>|<span data-ttu-id="2a764-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2a764-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a764-113">claimValue</span><span class="sxs-lookup"><span data-stu-id="2a764-113">claimValue</span></span>|<span data-ttu-id="2a764-114">Строка</span><span class="sxs-lookup"><span data-stu-id="2a764-114">String</span></span>|<span data-ttu-id="2a764-115">Значение утверждения контекста проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2a764-115">Value of the authentication context claim.</span></span>|
|<span data-ttu-id="2a764-116">id</span><span class="sxs-lookup"><span data-stu-id="2a764-116">id</span></span>|<span data-ttu-id="2a764-117">Строка</span><span class="sxs-lookup"><span data-stu-id="2a764-117">String</span></span>|<span data-ttu-id="2a764-118">Уникальный идентификатор для правила.</span><span class="sxs-lookup"><span data-stu-id="2a764-118">Unique identifier for the rule.</span></span> <span data-ttu-id="2a764-119">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="2a764-119">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="2a764-120">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2a764-120">isEnabled</span></span>|<span data-ttu-id="2a764-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a764-121">Boolean</span></span>|<span data-ttu-id="2a764-122">Указывает, включен ли параметр.</span><span class="sxs-lookup"><span data-stu-id="2a764-122">Indicates if the setting is enabled.</span></span>|
|<span data-ttu-id="2a764-123">target</span><span class="sxs-lookup"><span data-stu-id="2a764-123">target</span></span>|[<span data-ttu-id="2a764-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="2a764-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="2a764-125">Цель правила.</span><span class="sxs-lookup"><span data-stu-id="2a764-125">The target for the rule.</span></span> <span data-ttu-id="2a764-126">Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="2a764-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a764-127">Связи</span><span class="sxs-lookup"><span data-stu-id="2a764-127">Relationships</span></span>
<span data-ttu-id="2a764-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2a764-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a764-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2a764-129">JSON representation</span></span>
<span data-ttu-id="2a764-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a764-130">The following is a JSON representation of the resource.</span></span>
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

