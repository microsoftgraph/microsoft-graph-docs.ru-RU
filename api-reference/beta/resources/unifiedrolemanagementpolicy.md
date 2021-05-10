---
title: тип ресурса unifiedRoleManagementPolicy
description: В unifiedRoleManagementPolicy указаны различные политики, связанные с областью и определением ролей. Она получена из microsoft.graph.policyBase.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 73510f928fa4a32e92ff0a50b3439ab60dfb95f8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299665"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a><span data-ttu-id="202cc-104">тип ресурса unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="202cc-104">unifiedRoleManagementPolicy resource type</span></span>

<span data-ttu-id="202cc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="202cc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="202cc-106">В unifiedRoleManagementPolicy указаны различные политики, связанные с областью и определением ролей.</span><span class="sxs-lookup"><span data-stu-id="202cc-106">A unifiedRoleManagementPolicy specifies the various policies associated with a scope and role definition.</span></span> <span data-ttu-id="202cc-107">Она получена из microsoft.graph.policyBase.</span><span class="sxs-lookup"><span data-stu-id="202cc-107">It is derived from microsoft.graph.policyBase.</span></span>

## <a name="methods"></a><span data-ttu-id="202cc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="202cc-108">Methods</span></span>
|<span data-ttu-id="202cc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="202cc-109">Method</span></span>|<span data-ttu-id="202cc-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="202cc-110">Return type</span></span>|<span data-ttu-id="202cc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="202cc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="202cc-112">Список унифицированныхRoleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="202cc-112">List unifiedRoleManagementPolicies</span></span>](../api/unifiedrolemanagementpolicy-list.md)|<span data-ttu-id="202cc-113">[коллекция unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="202cc-113">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection</span></span>|<span data-ttu-id="202cc-114">Получите список объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="202cc-114">Get a list of the [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects and their properties.</span></span>|
|[<span data-ttu-id="202cc-115">Get unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="202cc-115">Get unifiedRoleManagementPolicy</span></span>](../api/unifiedrolemanagementpolicy-get.md)|[<span data-ttu-id="202cc-116">unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="202cc-116">unifiedRoleManagementPolicy</span></span>](../resources/unifiedrolemanagementpolicy.md)|<span data-ttu-id="202cc-117">Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicy.](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="202cc-117">Read the properties and relationships of an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object.</span></span>|
|[<span data-ttu-id="202cc-118">Список effectiveRules</span><span class="sxs-lookup"><span data-stu-id="202cc-118">List effectiveRules</span></span>](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|<span data-ttu-id="202cc-119">[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="202cc-119">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="202cc-120">Получите ресурсы unifiedRoleManagementPolicyRule из свойства эффективной навигацииRules.</span><span class="sxs-lookup"><span data-stu-id="202cc-120">Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.</span></span>|
|[<span data-ttu-id="202cc-121">Список правил</span><span class="sxs-lookup"><span data-stu-id="202cc-121">List rules</span></span>](../api/unifiedrolemanagementpolicy-list-rules.md)|<span data-ttu-id="202cc-122">[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="202cc-122">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="202cc-123">Получите ресурсы unifiedRoleManagementPolicyRule из свойства навигации правил.</span><span class="sxs-lookup"><span data-stu-id="202cc-123">Get the unifiedRoleManagementPolicyRule resources from the rules navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="202cc-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="202cc-124">Properties</span></span>
|<span data-ttu-id="202cc-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="202cc-125">Property</span></span>|<span data-ttu-id="202cc-126">Тип</span><span class="sxs-lookup"><span data-stu-id="202cc-126">Type</span></span>|<span data-ttu-id="202cc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="202cc-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="202cc-128">description</span><span class="sxs-lookup"><span data-stu-id="202cc-128">description</span></span>|<span data-ttu-id="202cc-129">Строка</span><span class="sxs-lookup"><span data-stu-id="202cc-129">String</span></span>|<span data-ttu-id="202cc-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="202cc-130">Description for the policy.</span></span>|
|<span data-ttu-id="202cc-131">displayName</span><span class="sxs-lookup"><span data-stu-id="202cc-131">displayName</span></span>|<span data-ttu-id="202cc-132">Строка</span><span class="sxs-lookup"><span data-stu-id="202cc-132">String</span></span>|<span data-ttu-id="202cc-133">Отображение имени политики.</span><span class="sxs-lookup"><span data-stu-id="202cc-133">Display name for the policy.</span></span>|
|<span data-ttu-id="202cc-134">id</span><span class="sxs-lookup"><span data-stu-id="202cc-134">id</span></span>|<span data-ttu-id="202cc-135">Строка</span><span class="sxs-lookup"><span data-stu-id="202cc-135">String</span></span>|<span data-ttu-id="202cc-136">Уникальный идентификатор для политики.</span><span class="sxs-lookup"><span data-stu-id="202cc-136">Unique identifier for the policy.</span></span>|
|<span data-ttu-id="202cc-137">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="202cc-137">isOrganizationDefault</span></span>|<span data-ttu-id="202cc-138">Логический</span><span class="sxs-lookup"><span data-stu-id="202cc-138">Boolean</span></span>|<span data-ttu-id="202cc-139">Это может быть установлено только для одной широкой политики клиента, которая будет применяться для всех областей и ролей.</span><span class="sxs-lookup"><span data-stu-id="202cc-139">This can only be set to true for a single tenant wide policy which will apply to all scopes and roles.</span></span> <span data-ttu-id="202cc-140">Установите область ScopeId на "/" и scopeType в Directory.</span><span class="sxs-lookup"><span data-stu-id="202cc-140">Set the scopeId to "/" and scopeType to Directory.</span></span>|
|<span data-ttu-id="202cc-141">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="202cc-141">lastModifiedBy</span></span>|[<span data-ttu-id="202cc-142">identity</span><span class="sxs-lookup"><span data-stu-id="202cc-142">identity</span></span>](../resources/identity.md)|<span data-ttu-id="202cc-143">Идентификатор, который в последний раз изменил параметр роли.</span><span class="sxs-lookup"><span data-stu-id="202cc-143">The identity who last modified the role setting.</span></span>|
|<span data-ttu-id="202cc-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="202cc-144">lastModifiedDateTime</span></span>|<span data-ttu-id="202cc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="202cc-145">DateTimeOffset</span></span>|<span data-ttu-id="202cc-146">Время последнего изменения параметра роли.</span><span class="sxs-lookup"><span data-stu-id="202cc-146">The time when the role setting was last modified.</span></span>|
|<span data-ttu-id="202cc-147">scopeId</span><span class="sxs-lookup"><span data-stu-id="202cc-147">scopeId</span></span>|<span data-ttu-id="202cc-148">Строка</span><span class="sxs-lookup"><span data-stu-id="202cc-148">String</span></span>|<span data-ttu-id="202cc-149">ID области, в которой создается политика.</span><span class="sxs-lookup"><span data-stu-id="202cc-149">The id of the scope where the policy is created.</span></span> <span data-ttu-id="202cc-150">Например,</span><span class="sxs-lookup"><span data-stu-id="202cc-150">E.g.</span></span> <span data-ttu-id="202cc-151">"/", groupId и т. д.</span><span class="sxs-lookup"><span data-stu-id="202cc-151">"/", groupId, etc.</span></span>|
|<span data-ttu-id="202cc-152">scopeType</span><span class="sxs-lookup"><span data-stu-id="202cc-152">scopeType</span></span>|<span data-ttu-id="202cc-153">Строка</span><span class="sxs-lookup"><span data-stu-id="202cc-153">String</span></span>|<span data-ttu-id="202cc-154">Тип области, в которой создается политика.</span><span class="sxs-lookup"><span data-stu-id="202cc-154">The type of the scope where the policy is created.</span></span> <span data-ttu-id="202cc-155">Один из Directory, DirectoryRole, Group.</span><span class="sxs-lookup"><span data-stu-id="202cc-155">One of Directory, DirectoryRole, Group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="202cc-156">Связи</span><span class="sxs-lookup"><span data-stu-id="202cc-156">Relationships</span></span>
|<span data-ttu-id="202cc-157">Связь</span><span class="sxs-lookup"><span data-stu-id="202cc-157">Relationship</span></span>|<span data-ttu-id="202cc-158">Тип</span><span class="sxs-lookup"><span data-stu-id="202cc-158">Type</span></span>|<span data-ttu-id="202cc-159">Описание</span><span class="sxs-lookup"><span data-stu-id="202cc-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="202cc-160">effectiveRules</span><span class="sxs-lookup"><span data-stu-id="202cc-160">effectiveRules</span></span>|<span data-ttu-id="202cc-161">[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="202cc-161">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="202cc-162">Список эффективных правил, таких как правило утверждения, правило истечения срока действия и т. д. оценивается на основе унаследованных ссылок.</span><span class="sxs-lookup"><span data-stu-id="202cc-162">The list of effective rules like approval rule, expiration rule, etc. evaluated based on inherited referenced rules.</span></span> <span data-ttu-id="202cc-163">Например,</span><span class="sxs-lookup"><span data-stu-id="202cc-163">E.g.</span></span> <span data-ttu-id="202cc-164">Если существует широкая политика клиента по обеспечению соблюдения правила утверждения включения, эффективным правилом будет включение утверждения, даже если у полиса есть правило, чтобы отключить утверждение.</span><span class="sxs-lookup"><span data-stu-id="202cc-164">If there is a tenant wide policy to enforce enabling approval rule, the effective rule will be to enable approval even if the polcy has a rule to disable approval.</span></span>|
|<span data-ttu-id="202cc-165">правила</span><span class="sxs-lookup"><span data-stu-id="202cc-165">rules</span></span>|<span data-ttu-id="202cc-166">[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="202cc-166">[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection</span></span>|<span data-ttu-id="202cc-167">Коллекция правил, таких как правило утверждения, правило истечения срока действия и т. д.</span><span class="sxs-lookup"><span data-stu-id="202cc-167">The collection of rules like approval rule, expiration rule, etc.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="202cc-168">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="202cc-168">JSON representation</span></span>
<span data-ttu-id="202cc-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="202cc-169">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isOrganizationDefault": "Boolean",
  "scopeId": "String",
  "scopeType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

