---
title: тип ресурса unifiedRoleAssignment
description: Назначение ролей — это связь между определением роли и главным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c52e6bb05c9258680a36f04ad428c24a3a2829fc
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239973"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="25cba-103">тип ресурса unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25cba-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="25cba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25cba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25cba-105">Для предоставления доступа к ресурсам используется единая системаRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="25cba-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="25cba-106">Он представляет определение роли, назначенное основному (обычно пользователю) в определенной области.</span><span class="sxs-lookup"><span data-stu-id="25cba-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="25cba-107">Необходимо предоставить directoryScopeId или appScopeId.</span><span class="sxs-lookup"><span data-stu-id="25cba-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="25cba-108">Методы</span><span class="sxs-lookup"><span data-stu-id="25cba-108">Methods</span></span>

| <span data-ttu-id="25cba-109">Метод</span><span class="sxs-lookup"><span data-stu-id="25cba-109">Method</span></span>       | <span data-ttu-id="25cba-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="25cba-110">Return Type</span></span> | <span data-ttu-id="25cba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="25cba-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="25cba-112">Список unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25cba-112">List unifiedRoleAssignment</span></span>](../api/rbacapplication-list-roleassignments.md) | [<span data-ttu-id="25cba-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25cba-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="25cba-114">Ознакомьтесь со списком объектов unifiedRoleAssignment и их свойствами.</span><span class="sxs-lookup"><span data-stu-id="25cba-114">Read a list of unifiedRoleAssignment objects and their properties.</span></span> |
| [<span data-ttu-id="25cba-115">Get unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25cba-115">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="25cba-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25cba-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="25cba-117">Чтение свойств и связей объекта unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="25cba-117">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="25cba-118">Создание unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25cba-118">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="25cba-119">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25cba-119">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="25cba-120">Создайте новую унифицированную функциюRoleAssignment, разместив в коллекции roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="25cba-120">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="25cba-121">Удаление unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25cba-121">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="25cba-122">Нет</span><span class="sxs-lookup"><span data-stu-id="25cba-122">None</span></span> | <span data-ttu-id="25cba-123">Удаление объекта unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="25cba-123">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="25cba-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="25cba-124">Properties</span></span>

| <span data-ttu-id="25cba-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="25cba-125">Property</span></span>     | <span data-ttu-id="25cba-126">Тип</span><span class="sxs-lookup"><span data-stu-id="25cba-126">Type</span></span>        | <span data-ttu-id="25cba-127">Описание</span><span class="sxs-lookup"><span data-stu-id="25cba-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="25cba-128">id</span><span class="sxs-lookup"><span data-stu-id="25cba-128">id</span></span>|<span data-ttu-id="25cba-129">Строка</span><span class="sxs-lookup"><span data-stu-id="25cba-129">String</span></span>| <span data-ttu-id="25cba-130">Уникальный идентификатор для единойRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="25cba-130">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="25cba-131">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="25cba-131">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="25cba-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="25cba-132">roleDefinitionId</span></span>|<span data-ttu-id="25cba-133">Строка</span><span class="sxs-lookup"><span data-stu-id="25cba-133">String</span></span>| <span data-ttu-id="25cba-134">Идентификатор унифицированногоRoleDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="25cba-134">Identifier of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="25cba-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25cba-135">Read-only.</span></span> <span data-ttu-id="25cba-136">Поддерживает `$filter` `eq` (только оператор).</span><span class="sxs-lookup"><span data-stu-id="25cba-136">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="25cba-137">principalId</span><span class="sxs-lookup"><span data-stu-id="25cba-137">principalId</span></span>|<span data-ttu-id="25cba-138">Строка</span><span class="sxs-lookup"><span data-stu-id="25cba-138">String</span></span>| <span data-ttu-id="25cba-139">Идентификатор основного, которому предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="25cba-139">Identifier of the principal to which the assignment is granted.</span></span> <span data-ttu-id="25cba-140">Поддерживает `$filter` `eq` (только оператор).</span><span class="sxs-lookup"><span data-stu-id="25cba-140">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="25cba-141">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="25cba-141">directoryScopeId</span></span>|<span data-ttu-id="25cba-142">Строка</span><span class="sxs-lookup"><span data-stu-id="25cba-142">String</span></span>|<span data-ttu-id="25cba-143">Идентификатор объекта каталога, представляющего область назначения.</span><span class="sxs-lookup"><span data-stu-id="25cba-143">Identifier of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="25cba-144">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="25cba-144">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="25cba-145">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="25cba-145">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="25cba-146">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="25cba-146">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="25cba-147">appScopeId</span><span class="sxs-lookup"><span data-stu-id="25cba-147">appScopeId</span></span>|<span data-ttu-id="25cba-148">Строка</span><span class="sxs-lookup"><span data-stu-id="25cba-148">String</span></span>|<span data-ttu-id="25cba-149">Идентификатор конкретной области приложения, когда область назначения является конкретной.</span><span class="sxs-lookup"><span data-stu-id="25cba-149">Identifier of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="25cba-150">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="25cba-150">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="25cba-151">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="25cba-151">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="25cba-152">Используйте `/` для области для клиента.</span><span class="sxs-lookup"><span data-stu-id="25cba-152">Use `/` for tenant-wide scope.</span></span> <span data-ttu-id="25cba-153">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="25cba-153">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="25cba-154">resourceScope</span><span class="sxs-lookup"><span data-stu-id="25cba-154">resourceScope</span></span>|<span data-ttu-id="25cba-155">Строка</span><span class="sxs-lookup"><span data-stu-id="25cba-155">String</span></span>| <span data-ttu-id="25cba-156">Область применения unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="25cba-156">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="25cba-157">Это для `/` всей службы.</span><span class="sxs-lookup"><span data-stu-id="25cba-157">This is `/` for service-wide.</span></span> <span data-ttu-id="25cba-158">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось.**</span><span class="sxs-lookup"><span data-stu-id="25cba-158">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="25cba-159">Связи</span><span class="sxs-lookup"><span data-stu-id="25cba-159">Relationships</span></span>

| <span data-ttu-id="25cba-160">Связь</span><span class="sxs-lookup"><span data-stu-id="25cba-160">Relationship</span></span> | <span data-ttu-id="25cba-161">Тип</span><span class="sxs-lookup"><span data-stu-id="25cba-161">Type</span></span>   |<span data-ttu-id="25cba-162">Описание</span><span class="sxs-lookup"><span data-stu-id="25cba-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25cba-163">appScope</span><span class="sxs-lookup"><span data-stu-id="25cba-163">appScope</span></span>|[<span data-ttu-id="25cba-164">appScope</span><span class="sxs-lookup"><span data-stu-id="25cba-164">appScope</span></span>](appscope.md)|<span data-ttu-id="25cba-165">Сведения о конкретной области приложения, когда область назначения является конкретной.</span><span class="sxs-lookup"><span data-stu-id="25cba-165">Details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="25cba-166">Объект containment.</span><span class="sxs-lookup"><span data-stu-id="25cba-166">Containment entity.</span></span> |
|<span data-ttu-id="25cba-167">directoryScope</span><span class="sxs-lookup"><span data-stu-id="25cba-167">directoryScope</span></span>|[<span data-ttu-id="25cba-168">directoryObject</span><span class="sxs-lookup"><span data-stu-id="25cba-168">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="25cba-169">Объект каталога, который является областью назначения.</span><span class="sxs-lookup"><span data-stu-id="25cba-169">The directory object that is the scope of the assignment.</span></span> <span data-ttu-id="25cba-170">При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей.</span><span class="sxs-lookup"><span data-stu-id="25cba-170">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="25cba-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25cba-171">Read-only.</span></span> <span data-ttu-id="25cba-172">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="25cba-172">Supports `$expand`.</span></span> |
|<span data-ttu-id="25cba-173">основной</span><span class="sxs-lookup"><span data-stu-id="25cba-173">principal</span></span>|[<span data-ttu-id="25cba-174">directoryObject</span><span class="sxs-lookup"><span data-stu-id="25cba-174">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="25cba-175">Назначенная директор.</span><span class="sxs-lookup"><span data-stu-id="25cba-175">The assigned principal.</span></span> <span data-ttu-id="25cba-176">При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="25cba-176">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="25cba-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25cba-177">Read-only.</span></span> <span data-ttu-id="25cba-178">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="25cba-178">Supports `$expand`.</span></span> |
|<span data-ttu-id="25cba-179">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="25cba-179">roleDefinition</span></span>|[<span data-ttu-id="25cba-180">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="25cba-180">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="25cba-181">РольDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="25cba-181">The roleDefinition the assignment is for.</span></span> <span data-ttu-id="25cba-182">При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="25cba-182">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="25cba-183">**roleDefinition.id** будет автоматически расширена.</span><span class="sxs-lookup"><span data-stu-id="25cba-183">**roleDefinition.id** will be auto expanded.</span></span> <span data-ttu-id="25cba-184">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="25cba-184">Supports `$expand`.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="25cba-185">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25cba-185">JSON representation</span></span>

<span data-ttu-id="25cba-186">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25cba-186">The following is a JSON representation of the resource.</span></span>

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

