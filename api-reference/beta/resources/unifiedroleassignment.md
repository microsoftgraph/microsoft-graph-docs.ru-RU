---
title: тип ресурса unifiedRoleAssignment
description: Назначение ролей — это связь между определением роли и главным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 16e03168f9eee4af8c6e69c7ee4fb774494643b4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351001"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="edd33-103">тип ресурса unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edd33-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="edd33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edd33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edd33-105">Для предоставления доступа к ресурсам используется единая системаRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="edd33-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="edd33-106">Он представляет определение роли, назначенное основному (обычно пользователю) в определенной области.</span><span class="sxs-lookup"><span data-stu-id="edd33-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="edd33-107">Необходимо предоставить directoryScopeId или appScopeId.</span><span class="sxs-lookup"><span data-stu-id="edd33-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="edd33-108">Методы</span><span class="sxs-lookup"><span data-stu-id="edd33-108">Methods</span></span>

| <span data-ttu-id="edd33-109">Метод</span><span class="sxs-lookup"><span data-stu-id="edd33-109">Method</span></span>       | <span data-ttu-id="edd33-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="edd33-110">Return Type</span></span> | <span data-ttu-id="edd33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="edd33-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="edd33-112">Список unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edd33-112">List unifiedRoleAssignment</span></span>](../api/rbacapplication-list-roleassignments.md) | [<span data-ttu-id="edd33-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edd33-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="edd33-114">Ознакомьтесь со списком объектов unifiedRoleAssignment и их свойствами.</span><span class="sxs-lookup"><span data-stu-id="edd33-114">Read a list of unifiedRoleAssignment objects and their properties.</span></span> |
| [<span data-ttu-id="edd33-115">Get unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edd33-115">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="edd33-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edd33-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="edd33-117">Чтение свойств и связей объекта unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="edd33-117">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="edd33-118">Создание unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edd33-118">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="edd33-119">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edd33-119">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="edd33-120">Создайте новую унифицированную функциюRoleAssignment, разместив в коллекции roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="edd33-120">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="edd33-121">Удаление unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="edd33-121">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="edd33-122">Нет</span><span class="sxs-lookup"><span data-stu-id="edd33-122">None</span></span> | <span data-ttu-id="edd33-123">Удаление объекта unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="edd33-123">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="edd33-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="edd33-124">Properties</span></span>

| <span data-ttu-id="edd33-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="edd33-125">Property</span></span>     | <span data-ttu-id="edd33-126">Тип</span><span class="sxs-lookup"><span data-stu-id="edd33-126">Type</span></span>        | <span data-ttu-id="edd33-127">Описание</span><span class="sxs-lookup"><span data-stu-id="edd33-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="edd33-128">id</span><span class="sxs-lookup"><span data-stu-id="edd33-128">id</span></span>|<span data-ttu-id="edd33-129">Строка</span><span class="sxs-lookup"><span data-stu-id="edd33-129">String</span></span>| <span data-ttu-id="edd33-130">Уникальный идентификатор для единойRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="edd33-130">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="edd33-131">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="edd33-131">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="edd33-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="edd33-132">roleDefinitionId</span></span>|<span data-ttu-id="edd33-133">Строка</span><span class="sxs-lookup"><span data-stu-id="edd33-133">String</span></span>| <span data-ttu-id="edd33-134">Идентификатор унифицированногоRoleDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="edd33-134">Identifier of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="edd33-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edd33-135">Read-only.</span></span> <span data-ttu-id="edd33-136">Поддерживает `$filter` `eq` (только оператор).</span><span class="sxs-lookup"><span data-stu-id="edd33-136">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="edd33-137">principalId</span><span class="sxs-lookup"><span data-stu-id="edd33-137">principalId</span></span>|<span data-ttu-id="edd33-138">Строка</span><span class="sxs-lookup"><span data-stu-id="edd33-138">String</span></span>| <span data-ttu-id="edd33-139">Идентификатор основного, которому предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="edd33-139">Identifier of the principal to which the assignment is granted.</span></span> <span data-ttu-id="edd33-140">Поддерживает `$filter` `eq` (только оператор).</span><span class="sxs-lookup"><span data-stu-id="edd33-140">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="edd33-141">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="edd33-141">directoryScopeId</span></span>|<span data-ttu-id="edd33-142">Строка</span><span class="sxs-lookup"><span data-stu-id="edd33-142">String</span></span>|<span data-ttu-id="edd33-143">Идентификатор объекта каталога, представляющего область назначения.</span><span class="sxs-lookup"><span data-stu-id="edd33-143">Identifier of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="edd33-144">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="edd33-144">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="edd33-145">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="edd33-145">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="edd33-146">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="edd33-146">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="edd33-147">appScopeId</span><span class="sxs-lookup"><span data-stu-id="edd33-147">appScopeId</span></span>|<span data-ttu-id="edd33-148">Строка</span><span class="sxs-lookup"><span data-stu-id="edd33-148">String</span></span>|<span data-ttu-id="edd33-149">Идентификатор конкретной области приложения, когда область назначения является конкретной.</span><span class="sxs-lookup"><span data-stu-id="edd33-149">Identifier of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="edd33-150">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="edd33-150">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="edd33-151">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="edd33-151">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="edd33-152">Используйте `/` для области для клиента.</span><span class="sxs-lookup"><span data-stu-id="edd33-152">Use `/` for tenant-wide scope.</span></span> <span data-ttu-id="edd33-153">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="edd33-153">App scopes are scopes that are defined and understood by this application only.</span></span>  <span data-ttu-id="edd33-154">Для поставщика управления правами используйте области приложений для указания каталога, например `/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997` .</span><span class="sxs-lookup"><span data-stu-id="edd33-154">For the entitlement management provider, use app scopes to specify a catalog, for example `/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997`.</span></span>|
|<span data-ttu-id="edd33-155">resourceScope</span><span class="sxs-lookup"><span data-stu-id="edd33-155">resourceScope</span></span>|<span data-ttu-id="edd33-156">Строка</span><span class="sxs-lookup"><span data-stu-id="edd33-156">String</span></span>| <span data-ttu-id="edd33-157">Область применения unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="edd33-157">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="edd33-158">Это для `/` всей службы.</span><span class="sxs-lookup"><span data-stu-id="edd33-158">This is `/` for service-wide.</span></span> <span data-ttu-id="edd33-159">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось.**</span><span class="sxs-lookup"><span data-stu-id="edd33-159">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="edd33-160">Связи</span><span class="sxs-lookup"><span data-stu-id="edd33-160">Relationships</span></span>

| <span data-ttu-id="edd33-161">Связь</span><span class="sxs-lookup"><span data-stu-id="edd33-161">Relationship</span></span> | <span data-ttu-id="edd33-162">Тип</span><span class="sxs-lookup"><span data-stu-id="edd33-162">Type</span></span>   |<span data-ttu-id="edd33-163">Описание</span><span class="sxs-lookup"><span data-stu-id="edd33-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edd33-164">appScope</span><span class="sxs-lookup"><span data-stu-id="edd33-164">appScope</span></span>|[<span data-ttu-id="edd33-165">appScope</span><span class="sxs-lookup"><span data-stu-id="edd33-165">appScope</span></span>](appscope.md)|<span data-ttu-id="edd33-166">Сведения о конкретной области приложения, когда область назначения является конкретной.</span><span class="sxs-lookup"><span data-stu-id="edd33-166">Details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="edd33-167">Объект containment.</span><span class="sxs-lookup"><span data-stu-id="edd33-167">Containment entity.</span></span> |
|<span data-ttu-id="edd33-168">directoryScope</span><span class="sxs-lookup"><span data-stu-id="edd33-168">directoryScope</span></span>|[<span data-ttu-id="edd33-169">directoryObject</span><span class="sxs-lookup"><span data-stu-id="edd33-169">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="edd33-170">Объект каталога, который является областью назначения.</span><span class="sxs-lookup"><span data-stu-id="edd33-170">The directory object that is the scope of the assignment.</span></span> <span data-ttu-id="edd33-171">При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей.</span><span class="sxs-lookup"><span data-stu-id="edd33-171">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="edd33-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edd33-172">Read-only.</span></span> <span data-ttu-id="edd33-173">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="edd33-173">Supports `$expand`.</span></span> |
|<span data-ttu-id="edd33-174">основной</span><span class="sxs-lookup"><span data-stu-id="edd33-174">principal</span></span>|[<span data-ttu-id="edd33-175">directoryObject</span><span class="sxs-lookup"><span data-stu-id="edd33-175">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="edd33-176">Назначенная директор.</span><span class="sxs-lookup"><span data-stu-id="edd33-176">The assigned principal.</span></span> <span data-ttu-id="edd33-177">При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="edd33-177">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="edd33-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="edd33-178">Read-only.</span></span> <span data-ttu-id="edd33-179">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="edd33-179">Supports `$expand`.</span></span> |
|<span data-ttu-id="edd33-180">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="edd33-180">roleDefinition</span></span>|[<span data-ttu-id="edd33-181">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="edd33-181">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="edd33-182">РольDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="edd33-182">The roleDefinition the assignment is for.</span></span> <span data-ttu-id="edd33-183">При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="edd33-183">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="edd33-184">**roleDefinition.id** будет автоматически расширена.</span><span class="sxs-lookup"><span data-stu-id="edd33-184">**roleDefinition.id** will be auto expanded.</span></span> <span data-ttu-id="edd33-185">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="edd33-185">Supports `$expand`.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="edd33-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edd33-186">JSON representation</span></span>

<span data-ttu-id="edd33-187">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edd33-187">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalId": "String",
  "principal": {"@odata.type": "microsoft.graph.directoryObject"},
  "directoryScopeId": "String",
  "directoryScope": {"@odata.type": "microsoft.graph.directoryObject"},
  "appScopeId": "String",
  "appScope": {"@odata.type": "microsoft.graph.appScope"},
  "resourceScope": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
