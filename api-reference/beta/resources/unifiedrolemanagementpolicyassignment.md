---
title: тип ресурса unifiedRoleManagementPolicyAssignment
description: УнифицированнаяRoleManagementPolicyAssignment назначает политику определенной области и определению ролей.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0b51d9c088a9d6da4e1a3a671dd578e07ed22691
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682623"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a><span data-ttu-id="3d3b5-103">тип ресурса unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="3d3b5-103">unifiedRoleManagementPolicyAssignment resource type</span></span>

<span data-ttu-id="3d3b5-104">УнифицированнаяRoleManagementPolicyAssignment назначает политику определенной области и определению ролей.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-104">A unifiedRoleManagementPolicyAssignment assigns the policy to a specific scope and role definition.</span></span>

## <a name="methods"></a><span data-ttu-id="3d3b5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3d3b5-105">Methods</span></span>
|<span data-ttu-id="3d3b5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3d3b5-106">Method</span></span>|<span data-ttu-id="3d3b5-107">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="3d3b5-107">Return type</span></span>|<span data-ttu-id="3d3b5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3b5-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3d3b5-109">Список унифицированныхRoleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="3d3b5-109">List unifiedRoleManagementPolicyAssignments</span></span>](../api/unifiedrolemanagementpolicyassignment-list.md)|<span data-ttu-id="3d3b5-110">[коллекция unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3d3b5-110">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection</span></span>|<span data-ttu-id="3d3b5-111">Получите список объектов [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-111">Get a list of the [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) objects and their properties.</span></span>|
|[<span data-ttu-id="3d3b5-112">Get unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="3d3b5-112">Get unifiedRoleManagementPolicyAssignment</span></span>](../api/unifiedrolemanagementpolicyassignment-get.md)|[<span data-ttu-id="3d3b5-113">unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="3d3b5-113">unifiedRoleManagementPolicyAssignment</span></span>](../resources/unifiedrolemanagementpolicyassignment.md)|<span data-ttu-id="3d3b5-114">Ознакомьтесь с свойствами и отношениями единого [объектаRoleManagementPolicyAssignment.](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3d3b5-114">Read the properties and relationships of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3d3b5-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d3b5-115">Properties</span></span>
|<span data-ttu-id="3d3b5-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d3b5-116">Property</span></span>|<span data-ttu-id="3d3b5-117">Тип</span><span class="sxs-lookup"><span data-stu-id="3d3b5-117">Type</span></span>|<span data-ttu-id="3d3b5-118">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3b5-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d3b5-119">id</span><span class="sxs-lookup"><span data-stu-id="3d3b5-119">id</span></span>|<span data-ttu-id="3d3b5-120">String</span><span class="sxs-lookup"><span data-stu-id="3d3b5-120">String</span></span>|<span data-ttu-id="3d3b5-121">Уникальный идентификатор для назначения политики.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-121">Unique identifier for the policy assignment.</span></span>|
|<span data-ttu-id="3d3b5-122">policyId</span><span class="sxs-lookup"><span data-stu-id="3d3b5-122">policyId</span></span>|<span data-ttu-id="3d3b5-123">String</span><span class="sxs-lookup"><span data-stu-id="3d3b5-123">String</span></span>|<span data-ttu-id="3d3b5-124">ID политики.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-124">The id of the policy.</span></span>|
|<span data-ttu-id="3d3b5-125">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3d3b5-125">roleDefinitionId</span></span>|<span data-ttu-id="3d3b5-126">String</span><span class="sxs-lookup"><span data-stu-id="3d3b5-126">String</span></span>|<span data-ttu-id="3d3b5-127">ID определения роли, в котором применяется политика.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-127">The id of the role definition where the policy applies.</span></span> <span data-ttu-id="3d3b5-128">Если не указано, политика применяется ко всем ролям.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-128">If not specified, the policy applies to all roles.</span></span>|
|<span data-ttu-id="3d3b5-129">scopeId</span><span class="sxs-lookup"><span data-stu-id="3d3b5-129">scopeId</span></span>|<span data-ttu-id="3d3b5-130">String</span><span class="sxs-lookup"><span data-stu-id="3d3b5-130">String</span></span>|<span data-ttu-id="3d3b5-131">ID области, в которой назначена политика.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-131">The id of the scope where the policy is assigned.</span></span> <span data-ttu-id="3d3b5-132">Например,</span><span class="sxs-lookup"><span data-stu-id="3d3b5-132">E.g.</span></span> <span data-ttu-id="3d3b5-133">"/", groupId и т. д.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-133">"/", groupId, etc.</span></span>|
|<span data-ttu-id="3d3b5-134">scopeType</span><span class="sxs-lookup"><span data-stu-id="3d3b5-134">scopeType</span></span>|<span data-ttu-id="3d3b5-135">String</span><span class="sxs-lookup"><span data-stu-id="3d3b5-135">String</span></span>|<span data-ttu-id="3d3b5-136">Тип области, в которой назначена политика.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-136">The type of the scope where the policy is assigned.</span></span> <span data-ttu-id="3d3b5-137">Один из Directory, DirectoryRole, Group.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-137">One of Directory, DirectoryRole, Group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d3b5-138">Связи</span><span class="sxs-lookup"><span data-stu-id="3d3b5-138">Relationships</span></span>
|<span data-ttu-id="3d3b5-139">Связь</span><span class="sxs-lookup"><span data-stu-id="3d3b5-139">Relationship</span></span>|<span data-ttu-id="3d3b5-140">Тип</span><span class="sxs-lookup"><span data-stu-id="3d3b5-140">Type</span></span>|<span data-ttu-id="3d3b5-141">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3b5-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d3b5-142">policy</span><span class="sxs-lookup"><span data-stu-id="3d3b5-142">policy</span></span>|[<span data-ttu-id="3d3b5-143">unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="3d3b5-143">unifiedRoleManagementPolicy</span></span>](../resources/unifiedrolemanagementpolicy.md)|<span data-ttu-id="3d3b5-144">Политика назначения.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-144">The policy for the assignment.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d3b5-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d3b5-145">JSON representation</span></span>
<span data-ttu-id="3d3b5-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "id": "String (identifier)",
  "policyId": "String",
  "scopeId": "String",
  "scopeType": "String",
  "roleDefinitionId": "String"
}
```

