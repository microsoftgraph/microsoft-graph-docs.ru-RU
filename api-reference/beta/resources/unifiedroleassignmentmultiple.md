---
title: Тип ресурса Унифиедролеассигнментмултипле
description: Назначение роли — это связь между определением роли и участником в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: eb763490e9d60ca386400eef3dae1b9e2d382d21
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038676"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="7733c-103">Тип ресурса Унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="7733c-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="7733c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7733c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7733c-105">Унифиедролеассигнментмултипле используется для предоставления доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="7733c-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="7733c-106">Он представляет определение роли, назначенное массиву субъектов (как правило, пользователем), на массивах областей.</span><span class="sxs-lookup"><span data-stu-id="7733c-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="7733c-107">Примером такого поставщика RBAC является Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="7733c-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="7733c-108">В Microsoft Intune можно создать назначение роли с несколькими участниками и несколькими областями.</span><span class="sxs-lookup"><span data-stu-id="7733c-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="7733c-109">Указание **директорископеидс** или **аппскопеидс** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7733c-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="7733c-110">Методы</span><span class="sxs-lookup"><span data-stu-id="7733c-110">Methods</span></span>

| <span data-ttu-id="7733c-111">Метод</span><span class="sxs-lookup"><span data-stu-id="7733c-111">Method</span></span>       | <span data-ttu-id="7733c-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7733c-112">Return Type</span></span> | <span data-ttu-id="7733c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="7733c-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7733c-114">Получение unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="7733c-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="7733c-115">унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="7733c-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="7733c-116">Чтение свойств и связей объекта Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="7733c-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="7733c-117">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="7733c-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="7733c-118">унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="7733c-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="7733c-119">Создание нового Унифиедролеассигнментмултипле путем отправки в коллекцию roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="7733c-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="7733c-120">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="7733c-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="7733c-121">унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="7733c-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="7733c-122">Обновление существующего объекта Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="7733c-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="7733c-123">Удаление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="7733c-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="7733c-124">Нет</span><span class="sxs-lookup"><span data-stu-id="7733c-124">None</span></span> | <span data-ttu-id="7733c-125">Удаление объекта Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="7733c-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7733c-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="7733c-126">Properties</span></span>

| <span data-ttu-id="7733c-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="7733c-127">Property</span></span>     | <span data-ttu-id="7733c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="7733c-128">Type</span></span>        | <span data-ttu-id="7733c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7733c-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7733c-130">id</span><span class="sxs-lookup"><span data-stu-id="7733c-130">id</span></span> | <span data-ttu-id="7733c-131">String</span><span class="sxs-lookup"><span data-stu-id="7733c-131">String</span></span> | <span data-ttu-id="7733c-132">Уникальный идентификатор для Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="7733c-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="7733c-133">Key, не допускающая значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7733c-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="7733c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7733c-134">displayName</span></span> | <span data-ttu-id="7733c-135">Строка</span><span class="sxs-lookup"><span data-stu-id="7733c-135">String</span></span> | <span data-ttu-id="7733c-136">Имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7733c-136">Name of the role assignment.</span></span> <span data-ttu-id="7733c-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7733c-137">Required.</span></span> |
| <span data-ttu-id="7733c-138">description</span><span class="sxs-lookup"><span data-stu-id="7733c-138">description</span></span> | <span data-ttu-id="7733c-139">String</span><span class="sxs-lookup"><span data-stu-id="7733c-139">String</span></span> | <span data-ttu-id="7733c-140">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7733c-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="7733c-141">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="7733c-141">roleDefinitionId</span></span> | <span data-ttu-id="7733c-142">String</span><span class="sxs-lookup"><span data-stu-id="7733c-142">String</span></span> | <span data-ttu-id="7733c-143">Идентификатор Унифиедроледефинитион, для которого предназначено назначение.</span><span class="sxs-lookup"><span data-stu-id="7733c-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="7733c-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="7733c-144">roleDefinition</span></span> | [<span data-ttu-id="7733c-145">унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="7733c-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="7733c-146">Свойство, определяющее roleDefinition, для которого предназначено назначение.</span><span class="sxs-lookup"><span data-stu-id="7733c-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="7733c-147">Предоставляется таким образом, чтобы абоненты могли получить определение роли `$expand` одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7733c-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="7733c-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7733c-148">Read-only.</span></span>  |
| <span data-ttu-id="7733c-149">принЦипалидс</span><span class="sxs-lookup"><span data-stu-id="7733c-149">principalIds</span></span> | <span data-ttu-id="7733c-150">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7733c-150">String collection</span></span> | <span data-ttu-id="7733c-151">ObjectID субъектов, которым предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="7733c-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="7733c-152">субъектов</span><span class="sxs-lookup"><span data-stu-id="7733c-152">principals</span></span>| <span data-ttu-id="7733c-153">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7733c-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="7733c-154">Коллекция, доступная только для чтения, ссылающаяся на назначенные субъекты.</span><span class="sxs-lookup"><span data-stu-id="7733c-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="7733c-155">Предоставляется таким образом, чтобы абоненты могли получать участников с помощью `$expand` одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7733c-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="7733c-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7733c-156">Read-only.</span></span> |
| <span data-ttu-id="7733c-157">директорископеидс</span><span class="sxs-lookup"><span data-stu-id="7733c-157">directoryScopeIds</span></span> | <span data-ttu-id="7733c-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7733c-158">String collection</span></span> | <span data-ttu-id="7733c-159">Идентификаторы объектов каталога, представляющие области назначения.</span><span class="sxs-lookup"><span data-stu-id="7733c-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="7733c-160">Области назначения определяют набор ресурсов, доступ к которым получают участники.</span><span class="sxs-lookup"><span data-stu-id="7733c-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="7733c-161">Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="7733c-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="7733c-162">Области приложений — это области, которые определены и поняты только для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7733c-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="7733c-163">директорископес</span><span class="sxs-lookup"><span data-stu-id="7733c-163">directoryScopes</span></span> | <span data-ttu-id="7733c-164">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7733c-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="7733c-165">Коллекция, доступная только для чтения, ссылающаяся на объекты каталога, которые являются областью назначения.</span><span class="sxs-lookup"><span data-stu-id="7733c-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="7733c-166">Предоставляется таким образом, чтобы абоненты могли получать объекты каталога с использованием `$expand` одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="7733c-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="7733c-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7733c-167">Read-only.</span></span> |
| <span data-ttu-id="7733c-168">аппскопеидс</span><span class="sxs-lookup"><span data-stu-id="7733c-168">appScopeIds</span></span> | <span data-ttu-id="7733c-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7733c-169">String collection</span></span> | <span data-ttu-id="7733c-170">Идентификаторы определенных областей приложений, когда области назначения относятся к приложениям.</span><span class="sxs-lookup"><span data-stu-id="7733c-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="7733c-171">Области назначения определяют набор ресурсов, доступ к которым предоставлен субъекту.</span><span class="sxs-lookup"><span data-stu-id="7733c-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="7733c-172">Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="7733c-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="7733c-173">Используйте "/" для области действия на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="7733c-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="7733c-174">Области приложений — это области, которые определены и поняты только для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7733c-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="7733c-175">аппскопес</span><span class="sxs-lookup"><span data-stu-id="7733c-175">appScopes</span></span> | <span data-ttu-id="7733c-176">Коллекция [аппскопе](appscope.md)</span><span class="sxs-lookup"><span data-stu-id="7733c-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="7733c-177">Коллекция, доступная только для чтения, с подробными сведениями о конкретных областях приложения, когда области назначения относятся только к приложениям.</span><span class="sxs-lookup"><span data-stu-id="7733c-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="7733c-178">Сущность вложения.</span><span class="sxs-lookup"><span data-stu-id="7733c-178">Containment entity.</span></span> <span data-ttu-id="7733c-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7733c-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="7733c-180">Отношения</span><span class="sxs-lookup"><span data-stu-id="7733c-180">Relationships</span></span>

<span data-ttu-id="7733c-181">Нет</span><span class="sxs-lookup"><span data-stu-id="7733c-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7733c-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7733c-182">JSON representation</span></span>

<span data-ttu-id="7733c-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7733c-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "baseType": "",
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
