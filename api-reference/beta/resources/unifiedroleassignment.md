---
title: Тип ресурса Унифиедролеассигнмент
description: Назначение роли — это связь между определением роли и участником в определенной области для предоставления доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76055128876ab2c4340b55c43c4065f3aac73e4d
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160235"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="c9234-103">Тип ресурса Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="c9234-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="c9234-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9234-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9234-105">Унифиедролеассигнмент используется для предоставления доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="c9234-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="c9234-106">Он представляет определение роли, назначенное участнику (обычно пользователю) в определенной области.</span><span class="sxs-lookup"><span data-stu-id="c9234-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="c9234-107">Указание Директорископеид или Аппскопеид является обязательным.</span><span class="sxs-lookup"><span data-stu-id="c9234-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="c9234-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c9234-108">Methods</span></span>

| <span data-ttu-id="c9234-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c9234-109">Method</span></span>       | <span data-ttu-id="c9234-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c9234-110">Return Type</span></span> | <span data-ttu-id="c9234-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c9234-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c9234-112">Получение Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="c9234-112">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="c9234-113">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="c9234-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="c9234-114">Чтение свойств и связей объекта Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="c9234-114">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="c9234-115">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="c9234-115">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="c9234-116">унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="c9234-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="c9234-117">Создание нового Унифиедролеассигнмент путем отправки в коллекцию roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="c9234-117">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="c9234-118">Удаление Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="c9234-118">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="c9234-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c9234-119">None</span></span> | <span data-ttu-id="c9234-120">Удаление объекта Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="c9234-120">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c9234-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9234-121">Properties</span></span>

| <span data-ttu-id="c9234-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9234-122">Property</span></span>     | <span data-ttu-id="c9234-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c9234-123">Type</span></span>        | <span data-ttu-id="c9234-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c9234-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c9234-125">id</span><span class="sxs-lookup"><span data-stu-id="c9234-125">id</span></span>|<span data-ttu-id="c9234-126">Строка</span><span class="sxs-lookup"><span data-stu-id="c9234-126">String</span></span>| <span data-ttu-id="c9234-127">Уникальный идентификатор для Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="c9234-127">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="c9234-128">Key, не допускающая значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9234-128">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="c9234-129">роледефинитионид</span><span class="sxs-lookup"><span data-stu-id="c9234-129">roleDefinitionId</span></span>|<span data-ttu-id="c9234-130">Строка</span><span class="sxs-lookup"><span data-stu-id="c9234-130">String</span></span>| <span data-ttu-id="c9234-131">Идентификатор Унифиедроледефинитион, для которого предназначено назначение.</span><span class="sxs-lookup"><span data-stu-id="c9234-131">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="c9234-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9234-132">Read only.</span></span> |
|<span data-ttu-id="c9234-133">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c9234-133">roleDefinition</span></span>|[<span data-ttu-id="c9234-134">унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="c9234-134">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="c9234-135">Свойство, определяющее roleDefinition, для которого предназначено назначение.</span><span class="sxs-lookup"><span data-stu-id="c9234-135">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="c9234-136">Предоставляется таким образом, чтобы абоненты могли получить определение роли `$expand` одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c9234-136">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="c9234-137">roleDefinition.Id будет автоматически расширен</span><span class="sxs-lookup"><span data-stu-id="c9234-137">roleDefinition.Id will be auto expanded</span></span>
|<span data-ttu-id="c9234-138">principalId</span><span class="sxs-lookup"><span data-stu-id="c9234-138">principalId</span></span>|<span data-ttu-id="c9234-139">Строка</span><span class="sxs-lookup"><span data-stu-id="c9234-139">String</span></span>| <span data-ttu-id="c9234-140">ObjectID субъекта, которому предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="c9234-140">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="c9234-141">Участники</span><span class="sxs-lookup"><span data-stu-id="c9234-141">principal</span></span>|[<span data-ttu-id="c9234-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c9234-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="c9234-143">Свойство, ссылающееся на назначенный участник.</span><span class="sxs-lookup"><span data-stu-id="c9234-143">Property referencing the assigned principal.</span></span> <span data-ttu-id="c9234-144">Предоставляется таким образом, чтобы абоненты могли получать субъект `$expand` с помощью одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c9234-144">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="c9234-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9234-145">Read-only.</span></span> |
|<span data-ttu-id="c9234-146">директорископеид</span><span class="sxs-lookup"><span data-stu-id="c9234-146">directoryScopeId</span></span>|<span data-ttu-id="c9234-147">Строка</span><span class="sxs-lookup"><span data-stu-id="c9234-147">String</span></span>|<span data-ttu-id="c9234-148">Идентификатор объекта каталога, представляющий область назначения.</span><span class="sxs-lookup"><span data-stu-id="c9234-148">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="c9234-149">Область назначения определяет набор ресурсов, доступ к которым предоставлен участнику.</span><span class="sxs-lookup"><span data-stu-id="c9234-149">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="c9234-150">Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="c9234-150">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="c9234-151">Области приложений — это области, которые определены и поняты только для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="c9234-151">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="c9234-152">директорископе</span><span class="sxs-lookup"><span data-stu-id="c9234-152">directoryScope</span></span>|[<span data-ttu-id="c9234-153">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c9234-153">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="c9234-154">Свойство, ссылающееся на объект каталога, который является областью назначения.</span><span class="sxs-lookup"><span data-stu-id="c9234-154">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="c9234-155">Предоставляется таким образом, чтобы абоненты могли получать объект каталога `$expand` с использованием одновременно с получением назначения роли.</span><span class="sxs-lookup"><span data-stu-id="c9234-155">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="c9234-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9234-156">Read-only.</span></span> |
|<span data-ttu-id="c9234-157">аппскопеид</span><span class="sxs-lookup"><span data-stu-id="c9234-157">appScopeId</span></span>|<span data-ttu-id="c9234-158">Строка</span><span class="sxs-lookup"><span data-stu-id="c9234-158">String</span></span>|<span data-ttu-id="c9234-159">Идентификатор определенной области приложения, когда область назначения относится к приложению.</span><span class="sxs-lookup"><span data-stu-id="c9234-159">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="c9234-160">Область назначения определяет набор ресурсов, доступ к которым предоставлен участнику.</span><span class="sxs-lookup"><span data-stu-id="c9234-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="c9234-161">Области каталогов — это общие области, которые хранятся в каталоге, который понимается несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="c9234-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="c9234-162">Используйте "/" для области действия на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="c9234-162">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="c9234-163">Области приложений — это области, которые определены и поняты только для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="c9234-163">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="c9234-164">аппскопе</span><span class="sxs-lookup"><span data-stu-id="c9234-164">appScope</span></span>|[<span data-ttu-id="c9234-165">аппскопе</span><span class="sxs-lookup"><span data-stu-id="c9234-165">appScope</span></span>](appscope.md)|<span data-ttu-id="c9234-166">Свойство только для чтения, в котором сведения об определенной области приложения, когда область назначения относится только к приложению.</span><span class="sxs-lookup"><span data-stu-id="c9234-166">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="c9234-167">Сущность вложения.</span><span class="sxs-lookup"><span data-stu-id="c9234-167">Containment entity.</span></span> |
|<span data-ttu-id="c9234-168">ресаурцескопе</span><span class="sxs-lookup"><span data-stu-id="c9234-168">resourceScope</span></span>|<span data-ttu-id="c9234-169">Строка</span><span class="sxs-lookup"><span data-stu-id="c9234-169">String</span></span>| <span data-ttu-id="c9234-170">Область, в которой применяется Унифиедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="c9234-170">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="c9234-171">Это "/" для всей службы.</span><span class="sxs-lookup"><span data-stu-id="c9234-171">This is "/" for service-wide.</span></span> <span data-ttu-id="c9234-172">**НЕ ИСПОЛЬЗУЙТЕ. Это свойство будет нерекомендуемым в ближайшее время.**</span><span class="sxs-lookup"><span data-stu-id="c9234-172">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9234-173">Отношения</span><span class="sxs-lookup"><span data-stu-id="c9234-173">Relationships</span></span>

<span data-ttu-id="c9234-174">Нет</span><span class="sxs-lookup"><span data-stu-id="c9234-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9234-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9234-175">JSON representation</span></span>

<span data-ttu-id="c9234-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9234-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
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