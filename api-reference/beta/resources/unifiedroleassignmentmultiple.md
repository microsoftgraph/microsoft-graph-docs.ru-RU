---
title: Тип ресурса Унифиедролеассигнментмултипле
description: Назначение роли — это связь между определением роли и участником в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20e0d7a213ea6e46db9cf9774c46bda0070ecd27
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218032"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="116ca-103">Тип ресурса Унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="116ca-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="116ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="116ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="116ca-105">Унифиедролеассигнментмултипле используется для предоставления доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="116ca-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="116ca-106">Он представляет определение роли, назначенное массиву субъектов (как правило, пользователем), на массивах областей.</span><span class="sxs-lookup"><span data-stu-id="116ca-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="116ca-107">Примером такого поставщика RBAC является Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="116ca-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="116ca-108">В Microsoft Intune можно создать назначение роли с несколькими участниками и несколькими областями.</span><span class="sxs-lookup"><span data-stu-id="116ca-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="116ca-109">Указание **директорископеидс** или **аппскопеидс** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="116ca-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="116ca-110">Методы</span><span class="sxs-lookup"><span data-stu-id="116ca-110">Methods</span></span>

| <span data-ttu-id="116ca-111">Метод</span><span class="sxs-lookup"><span data-stu-id="116ca-111">Method</span></span>       | <span data-ttu-id="116ca-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="116ca-112">Return Type</span></span> | <span data-ttu-id="116ca-113">Описание</span><span class="sxs-lookup"><span data-stu-id="116ca-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="116ca-114">Получение unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="116ca-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="116ca-115">унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="116ca-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="116ca-116">Чтение свойств и связей объекта Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="116ca-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="116ca-117">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="116ca-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="116ca-118">унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="116ca-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="116ca-119">Создание нового Унифиедролеассигнментмултипле путем отправки в коллекцию roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="116ca-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="116ca-120">Обновление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="116ca-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="116ca-121">унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="116ca-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="116ca-122">Обновление существующего объекта Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="116ca-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="116ca-123">Удаление unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="116ca-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="116ca-124">Нет</span><span class="sxs-lookup"><span data-stu-id="116ca-124">None</span></span> | <span data-ttu-id="116ca-125">Удаление объекта Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="116ca-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="116ca-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="116ca-126">Properties</span></span>

| <span data-ttu-id="116ca-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="116ca-127">Property</span></span>     | <span data-ttu-id="116ca-128">Тип</span><span class="sxs-lookup"><span data-stu-id="116ca-128">Type</span></span>        | <span data-ttu-id="116ca-129">Описание</span><span class="sxs-lookup"><span data-stu-id="116ca-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="116ca-130">id</span><span class="sxs-lookup"><span data-stu-id="116ca-130">id</span></span> | <span data-ttu-id="116ca-131">String</span><span class="sxs-lookup"><span data-stu-id="116ca-131">String</span></span> | <span data-ttu-id="116ca-132">Уникальный идентификатор для Унифиедролеассигнментмултипле.</span><span class="sxs-lookup"><span data-stu-id="116ca-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="116ca-133">Key, не допускающая значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="116ca-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="116ca-134">displayName</span><span class="sxs-lookup"><span data-stu-id="116ca-134">displayName</span></span> | <span data-ttu-id="116ca-135">Строка</span><span class="sxs-lookup"><span data-stu-id="116ca-135">String</span></span> | <span data-ttu-id="116ca-136">Имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="116ca-136">Name of the role assignment.</span></span> |
| <span data-ttu-id="116ca-137">description</span><span class="sxs-lookup"><span data-stu-id="116ca-137">description</span></span> | <span data-ttu-id="116ca-138">String</span><span class="sxs-lookup"><span data-stu-id="116ca-138">String</span></span> | <span data-ttu-id="116ca-139">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="116ca-139">Description of the role assignment.</span></span> |
| <span data-ttu-id="116ca-140">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="116ca-140">roleDefinitionId</span></span> | <span data-ttu-id="116ca-141">String</span><span class="sxs-lookup"><span data-stu-id="116ca-141">String</span></span> | <span data-ttu-id="116ca-142">Идентификатор Унифиедроледефинитион, для которого предназначено назначение.</span><span class="sxs-lookup"><span data-stu-id="116ca-142">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="116ca-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="116ca-143">Read only.</span></span> |
| <span data-ttu-id="116ca-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="116ca-144">roleDefinition</span></span> | [<span data-ttu-id="116ca-145">унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="116ca-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="116ca-146">Свойство, определяющее roleDefinition, для которого предназначено назначение.</span><span class="sxs-lookup"><span data-stu-id="116ca-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="116ca-147">Предоставляется таким образом, чтобы абоненты могли получить определение роли `$expand` одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="116ca-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> |
| <span data-ttu-id="116ca-148">принЦипалидс</span><span class="sxs-lookup"><span data-stu-id="116ca-148">principalIds</span></span> | <span data-ttu-id="116ca-149">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="116ca-149">String collection</span></span> | <span data-ttu-id="116ca-150">ObjectID субъектов, которым предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="116ca-150">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="116ca-151">субъектов</span><span class="sxs-lookup"><span data-stu-id="116ca-151">principals</span></span>| <span data-ttu-id="116ca-152">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="116ca-152">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="116ca-153">Коллекция, доступная только для чтения, ссылающаяся на назначенные субъекты.</span><span class="sxs-lookup"><span data-stu-id="116ca-153">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="116ca-154">Предоставляется таким образом, чтобы абоненты могли получать участников с `$expand` помощью одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="116ca-154">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="116ca-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="116ca-155">Read-only.</span></span> |
| <span data-ttu-id="116ca-156">директорископеидс</span><span class="sxs-lookup"><span data-stu-id="116ca-156">directoryScopeIds</span></span> | <span data-ttu-id="116ca-157">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="116ca-157">String collection</span></span> | <span data-ttu-id="116ca-158">Идентификаторы объектов каталога, представляющие области назначения.</span><span class="sxs-lookup"><span data-stu-id="116ca-158">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="116ca-159">Области назначения определяют набор ресурсов, доступ к которым получают участники.</span><span class="sxs-lookup"><span data-stu-id="116ca-159">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="116ca-160">Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="116ca-160">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="116ca-161">Области приложений — это области, которые определены и поняты только для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="116ca-161">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="116ca-162">директорископес</span><span class="sxs-lookup"><span data-stu-id="116ca-162">directoryScopes</span></span> | <span data-ttu-id="116ca-163">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="116ca-163">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="116ca-164">Коллекция, доступная только для чтения, ссылающаяся на объекты каталога, которые являются областью назначения.</span><span class="sxs-lookup"><span data-stu-id="116ca-164">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="116ca-165">Предоставляется таким образом, чтобы абоненты могли получать объекты каталога `$expand` с использованием одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="116ca-165">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="116ca-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="116ca-166">Read-only.</span></span> |
| <span data-ttu-id="116ca-167">аппскопеидс</span><span class="sxs-lookup"><span data-stu-id="116ca-167">appScopeIds</span></span> | <span data-ttu-id="116ca-168">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="116ca-168">String collection</span></span> | <span data-ttu-id="116ca-169">Идентификаторы определенных областей приложений, когда области назначения относятся к приложениям.</span><span class="sxs-lookup"><span data-stu-id="116ca-169">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="116ca-170">Области назначения определяют набор ресурсов, доступ к которым предоставлен субъекту.</span><span class="sxs-lookup"><span data-stu-id="116ca-170">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="116ca-171">Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="116ca-171">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="116ca-172">Используйте "/" для области действия на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="116ca-172">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="116ca-173">Области приложений — это области, которые определены и поняты только для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="116ca-173">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="116ca-174">аппскопес</span><span class="sxs-lookup"><span data-stu-id="116ca-174">appScopes</span></span> | <span data-ttu-id="116ca-175">Коллекция [аппскопе](appscope.md)</span><span class="sxs-lookup"><span data-stu-id="116ca-175">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="116ca-176">Коллекция, доступная только для чтения, с подробными сведениями о конкретных областях приложения, когда области назначения относятся только к приложениям.</span><span class="sxs-lookup"><span data-stu-id="116ca-176">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="116ca-177">Сущность вложения.</span><span class="sxs-lookup"><span data-stu-id="116ca-177">Containment entity.</span></span> |

## <a name="relationships"></a><span data-ttu-id="116ca-178">Связи</span><span class="sxs-lookup"><span data-stu-id="116ca-178">Relationships</span></span>

<span data-ttu-id="116ca-179">Нет</span><span class="sxs-lookup"><span data-stu-id="116ca-179">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="116ca-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="116ca-180">JSON representation</span></span>

<span data-ttu-id="116ca-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="116ca-181">The following is a JSON representation of the resource.</span></span>

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