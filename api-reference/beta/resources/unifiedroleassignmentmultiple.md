---
title: Тип ресурса unifiedRoleAssignmentMultiple
description: Назначение роли — это связь между определением роли и основным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4df17c6b112cefe03a12631ee763f49e976fb568
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159845"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="3920f-103">Тип ресурса unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3920f-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="3920f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3920f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3920f-105">Для предоставления доступа к ресурсам используется unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="3920f-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="3920f-106">Он представляет определение роли, назначенное массиву основных ролей (обычно пользователю) в массиве областей.</span><span class="sxs-lookup"><span data-stu-id="3920f-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="3920f-107">Примером такого поставщика RBAC является Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="3920f-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="3920f-108">В Microsoft Intune можно создать назначение роли с несколькими основными и несколькими уровнями.</span><span class="sxs-lookup"><span data-stu-id="3920f-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="3920f-109">Требуется **предоставить directoryScopeIds** или **appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="3920f-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="3920f-110">Методы</span><span class="sxs-lookup"><span data-stu-id="3920f-110">Methods</span></span>

| <span data-ttu-id="3920f-111">Метод</span><span class="sxs-lookup"><span data-stu-id="3920f-111">Method</span></span>       | <span data-ttu-id="3920f-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3920f-112">Return Type</span></span> | <span data-ttu-id="3920f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3920f-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3920f-114">Получение unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3920f-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="3920f-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3920f-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="3920f-116">Чтение свойств и связей объекта unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="3920f-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="3920f-117">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3920f-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="3920f-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3920f-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="3920f-119">Создание новой unifiedRoleAssignmentMultiple путем публикации в коллекции roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="3920f-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="3920f-120">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3920f-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="3920f-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3920f-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="3920f-122">Обновление существующего объекта unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="3920f-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="3920f-123">Удаление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3920f-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="3920f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="3920f-124">None</span></span> | <span data-ttu-id="3920f-125">Удаление объекта unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="3920f-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3920f-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="3920f-126">Properties</span></span>

| <span data-ttu-id="3920f-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="3920f-127">Property</span></span>     | <span data-ttu-id="3920f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="3920f-128">Type</span></span>        | <span data-ttu-id="3920f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3920f-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3920f-130">id</span><span class="sxs-lookup"><span data-stu-id="3920f-130">id</span></span> | <span data-ttu-id="3920f-131">String</span><span class="sxs-lookup"><span data-stu-id="3920f-131">String</span></span> | <span data-ttu-id="3920f-132">Уникальный идентификатор unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="3920f-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="3920f-133">Ключ, не значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3920f-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="3920f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3920f-134">displayName</span></span> | <span data-ttu-id="3920f-135">String</span><span class="sxs-lookup"><span data-stu-id="3920f-135">String</span></span> | <span data-ttu-id="3920f-136">Имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3920f-136">Name of the role assignment.</span></span> <span data-ttu-id="3920f-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3920f-137">Required.</span></span> |
| <span data-ttu-id="3920f-138">description</span><span class="sxs-lookup"><span data-stu-id="3920f-138">description</span></span> | <span data-ttu-id="3920f-139">String</span><span class="sxs-lookup"><span data-stu-id="3920f-139">String</span></span> | <span data-ttu-id="3920f-140">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3920f-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="3920f-141">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3920f-141">roleDefinitionId</span></span> | <span data-ttu-id="3920f-142">String</span><span class="sxs-lookup"><span data-stu-id="3920f-142">String</span></span> | <span data-ttu-id="3920f-143">ИД unifiedRoleDefinition, для который требуется назначение.</span><span class="sxs-lookup"><span data-stu-id="3920f-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="3920f-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3920f-144">roleDefinition</span></span> | [<span data-ttu-id="3920f-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3920f-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="3920f-146">Свойство, указывающее roleDefinition, для которого назначение.</span><span class="sxs-lookup"><span data-stu-id="3920f-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="3920f-147">Предоставляется, чтобы вызыватели могли получить определение роли одновременно с получением `$expand` назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3920f-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="3920f-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3920f-148">Read-only.</span></span>  |
| <span data-ttu-id="3920f-149">principalIds</span><span class="sxs-lookup"><span data-stu-id="3920f-149">principalIds</span></span> | <span data-ttu-id="3920f-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3920f-150">String collection</span></span> | <span data-ttu-id="3920f-151">Objectids of the principals to which the assignment is granted.</span><span class="sxs-lookup"><span data-stu-id="3920f-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="3920f-152">principals</span><span class="sxs-lookup"><span data-stu-id="3920f-152">principals</span></span>| <span data-ttu-id="3920f-153">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3920f-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="3920f-154">Коллекция только для чтения, ссылаясь на назначенную сумму.</span><span class="sxs-lookup"><span data-stu-id="3920f-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="3920f-155">Предоставляется для того, чтобы вызыватели могли получать основных ролей, используя `$expand` одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3920f-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="3920f-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3920f-156">Read-only.</span></span> |
| <span data-ttu-id="3920f-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="3920f-157">directoryScopeIds</span></span> | <span data-ttu-id="3920f-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3920f-158">String collection</span></span> | <span data-ttu-id="3920f-159">ИД объектов каталога, представляющих области назначения.</span><span class="sxs-lookup"><span data-stu-id="3920f-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="3920f-160">Области назначения определяют набор ресурсов, к которым были предоставлены доступ к этим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="3920f-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="3920f-161">Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="3920f-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="3920f-162">Области приложения — это области, которые определяются и понятны только этому приложению.</span><span class="sxs-lookup"><span data-stu-id="3920f-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="3920f-163">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="3920f-163">directoryScopes</span></span> | <span data-ttu-id="3920f-164">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3920f-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="3920f-165">Коллекция только для чтения, ссылаясь на объекты каталога, которые являются областью назначения.</span><span class="sxs-lookup"><span data-stu-id="3920f-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="3920f-166">Предоставляется для того, чтобы вызыватели могли получать объекты каталога одновременно с получением `$expand` назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3920f-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="3920f-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3920f-167">Read-only.</span></span> |
| <span data-ttu-id="3920f-168">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="3920f-168">appScopeIds</span></span> | <span data-ttu-id="3920f-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3920f-169">String collection</span></span> | <span data-ttu-id="3920f-170">Ids of the app specific scopes when the assignment scopes are app specific.</span><span class="sxs-lookup"><span data-stu-id="3920f-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="3920f-171">Области назначения определяют набор ресурсов, к которым был предоставлен доступ для основного.</span><span class="sxs-lookup"><span data-stu-id="3920f-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="3920f-172">Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="3920f-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="3920f-173">Используйте "/" для области на клиенте.</span><span class="sxs-lookup"><span data-stu-id="3920f-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="3920f-174">Области приложения — это области, которые определяются и понятны только этому приложению.</span><span class="sxs-lookup"><span data-stu-id="3920f-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="3920f-175">appScopes</span><span class="sxs-lookup"><span data-stu-id="3920f-175">appScopes</span></span> | <span data-ttu-id="3920f-176">[Коллекция appScope](appscope.md)</span><span class="sxs-lookup"><span data-stu-id="3920f-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="3920f-177">Коллекция только для чтения с подробными сведениями об областях приложения, если области назначения являются конкретными для приложения.</span><span class="sxs-lookup"><span data-stu-id="3920f-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="3920f-178">Объект Containment.</span><span class="sxs-lookup"><span data-stu-id="3920f-178">Containment entity.</span></span> <span data-ttu-id="3920f-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3920f-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="3920f-180">Связи</span><span class="sxs-lookup"><span data-stu-id="3920f-180">Relationships</span></span>

<span data-ttu-id="3920f-181">Нет</span><span class="sxs-lookup"><span data-stu-id="3920f-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3920f-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3920f-182">JSON representation</span></span>

<span data-ttu-id="3920f-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3920f-183">The following is a JSON representation of the resource.</span></span>

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


