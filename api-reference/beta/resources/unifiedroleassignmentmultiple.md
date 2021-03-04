---
title: тип ресурса unifiedRoleAssignmentMultiple
description: Назначение ролей — это связь между определением роли и главным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f612fea9ce7aa54cce505a4f2d77370f45947c44
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442707"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="9c5c8-103">тип ресурса unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9c5c8-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="9c5c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c5c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c5c8-105">Для предоставления доступа к ресурсам используется unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="9c5c8-106">Оно представляет определение роли, назначенное массиву принципов (как правило, пользователю) по массиву областей.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="9c5c8-107">Примером такого поставщика RBAC является Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="9c5c8-108">В Microsoft Intune можно создать назначение ролей с несколькими основными и несколькими областьми.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="9c5c8-109">Необходимо **предоставить либо directoryScopeIds,** либо **appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="9c5c8-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="9c5c8-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9c5c8-110">Methods</span></span>

| <span data-ttu-id="9c5c8-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9c5c8-111">Method</span></span>       | <span data-ttu-id="9c5c8-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9c5c8-112">Return Type</span></span> | <span data-ttu-id="9c5c8-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9c5c8-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9c5c8-114">Получение unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9c5c8-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="9c5c8-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9c5c8-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="9c5c8-116">Чтение свойств и связей объекта unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="9c5c8-117">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9c5c8-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="9c5c8-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9c5c8-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="9c5c8-119">Создайте новую единую системуRoleAssignmentMultiple, разместив в коллекции roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="9c5c8-120">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9c5c8-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="9c5c8-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9c5c8-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="9c5c8-122">Обновление существующего объекта unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="9c5c8-123">Удаление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9c5c8-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="9c5c8-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9c5c8-124">None</span></span> | <span data-ttu-id="9c5c8-125">Удаление объекта unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c5c8-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c5c8-126">Properties</span></span>

| <span data-ttu-id="9c5c8-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c5c8-127">Property</span></span>     | <span data-ttu-id="9c5c8-128">Тип</span><span class="sxs-lookup"><span data-stu-id="9c5c8-128">Type</span></span>        | <span data-ttu-id="9c5c8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="9c5c8-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9c5c8-130">id</span><span class="sxs-lookup"><span data-stu-id="9c5c8-130">id</span></span> | <span data-ttu-id="9c5c8-131">String</span><span class="sxs-lookup"><span data-stu-id="9c5c8-131">String</span></span> | <span data-ttu-id="9c5c8-132">Уникальный идентификатор для единойRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="9c5c8-133">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="9c5c8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9c5c8-134">displayName</span></span> | <span data-ttu-id="9c5c8-135">String</span><span class="sxs-lookup"><span data-stu-id="9c5c8-135">String</span></span> | <span data-ttu-id="9c5c8-136">Имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-136">Name of the role assignment.</span></span> <span data-ttu-id="9c5c8-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-137">Required.</span></span> |
| <span data-ttu-id="9c5c8-138">description</span><span class="sxs-lookup"><span data-stu-id="9c5c8-138">description</span></span> | <span data-ttu-id="9c5c8-139">String</span><span class="sxs-lookup"><span data-stu-id="9c5c8-139">String</span></span> | <span data-ttu-id="9c5c8-140">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="9c5c8-141">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9c5c8-141">roleDefinitionId</span></span> | <span data-ttu-id="9c5c8-142">String</span><span class="sxs-lookup"><span data-stu-id="9c5c8-142">String</span></span> | <span data-ttu-id="9c5c8-143">ID унифицированногоRoleDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="9c5c8-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9c5c8-144">roleDefinition</span></span> | [<span data-ttu-id="9c5c8-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9c5c8-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="9c5c8-146">Свойство, указывающее рольDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="9c5c8-147">При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="9c5c8-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-148">Read-only.</span></span>  |
| <span data-ttu-id="9c5c8-149">principalIds</span><span class="sxs-lookup"><span data-stu-id="9c5c8-149">principalIds</span></span> | <span data-ttu-id="9c5c8-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9c5c8-150">String collection</span></span> | <span data-ttu-id="9c5c8-151">Objectids of the principals to which the assignment is granted.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="9c5c8-152">основные</span><span class="sxs-lookup"><span data-stu-id="9c5c8-152">principals</span></span>| <span data-ttu-id="9c5c8-153">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9c5c8-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="9c5c8-154">Коллекция только для чтения, ссылаясь на назначенных директоров.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="9c5c8-155">При условии, что звонители смогут получать главные принципы одновременно с `$expand` назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="9c5c8-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-156">Read-only.</span></span> |
| <span data-ttu-id="9c5c8-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="9c5c8-157">directoryScopeIds</span></span> | <span data-ttu-id="9c5c8-158">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9c5c8-158">String collection</span></span> | <span data-ttu-id="9c5c8-159">Ids объектов каталога, представляющих области назначения.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="9c5c8-160">Области назначения определяют набор ресурсов, к которым доверимы получили доступ.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="9c5c8-161">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="9c5c8-162">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="9c5c8-163">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="9c5c8-163">directoryScopes</span></span> | <span data-ttu-id="9c5c8-164">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9c5c8-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="9c5c8-165">Коллекция только для чтения, ссылаясь на объекты каталога, которые являются областью назначения.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="9c5c8-166">При условии, что вызыватели могут получать объекты каталога, используя одновременно `$expand` с назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="9c5c8-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-167">Read-only.</span></span> |
| <span data-ttu-id="9c5c8-168">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="9c5c8-168">appScopeIds</span></span> | <span data-ttu-id="9c5c8-169">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9c5c8-169">String collection</span></span> | <span data-ttu-id="9c5c8-170">Ids of the app specific scopes when the assignment scopes are app specific.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="9c5c8-171">Области назначения определяют набор ресурсов, для которых доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="9c5c8-172">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="9c5c8-173">Используйте "/" для области для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="9c5c8-174">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="9c5c8-175">appScopes</span><span class="sxs-lookup"><span data-stu-id="9c5c8-175">appScopes</span></span> | <span data-ttu-id="9c5c8-176">[коллекция appScope](appscope.md)</span><span class="sxs-lookup"><span data-stu-id="9c5c8-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="9c5c8-177">Коллекция только для чтения с подробными сведениями о конкретных областях приложения, когда области назначения являются конкретными приложениями.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="9c5c8-178">Объект containment.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-178">Containment entity.</span></span> <span data-ttu-id="9c5c8-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="9c5c8-180">Связи</span><span class="sxs-lookup"><span data-stu-id="9c5c8-180">Relationships</span></span>

<span data-ttu-id="9c5c8-181">Нет</span><span class="sxs-lookup"><span data-stu-id="9c5c8-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c5c8-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c5c8-182">JSON representation</span></span>

<span data-ttu-id="9c5c8-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c5c8-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalIds": ["string"],
  "principals": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directoryScopeIds": ["string"],
  "directoryScopes": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "appScopeIds": ["string"],
  "appScopes": [{"@odata.type": "microsoft.graph.appScope"}],
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignmentMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


