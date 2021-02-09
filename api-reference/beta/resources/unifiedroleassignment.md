---
title: Тип ресурса unifiedRoleAssignment
description: Назначение роли — это связь между определением роли и основным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4dc0ec6bb692c88d2b01a440bae1d7789bd042a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159033"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="ff34f-103">Тип ресурса unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff34f-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="ff34f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff34f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff34f-105">Для предоставления доступа к ресурсам используется unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff34f-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="ff34f-106">Он представляет определение роли, назначенное основному пользователю в определенной области.</span><span class="sxs-lookup"><span data-stu-id="ff34f-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="ff34f-107">Требуется предоставить directoryScopeId или appScopeId.</span><span class="sxs-lookup"><span data-stu-id="ff34f-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="ff34f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ff34f-108">Methods</span></span>

| <span data-ttu-id="ff34f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ff34f-109">Method</span></span>       | <span data-ttu-id="ff34f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff34f-110">Return Type</span></span> | <span data-ttu-id="ff34f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ff34f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ff34f-112">Get unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff34f-112">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="ff34f-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff34f-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="ff34f-114">Чтение свойств и связей объекта unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff34f-114">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="ff34f-115">Создание unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff34f-115">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="ff34f-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff34f-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="ff34f-117">Создание нового unifiedRoleAssignment путем публикации в коллекции roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff34f-117">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="ff34f-118">Удаление unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff34f-118">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="ff34f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ff34f-119">None</span></span> | <span data-ttu-id="ff34f-120">Удаление объекта unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff34f-120">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff34f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff34f-121">Properties</span></span>

| <span data-ttu-id="ff34f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff34f-122">Property</span></span>     | <span data-ttu-id="ff34f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ff34f-123">Type</span></span>        | <span data-ttu-id="ff34f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ff34f-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff34f-125">id</span><span class="sxs-lookup"><span data-stu-id="ff34f-125">id</span></span>|<span data-ttu-id="ff34f-126">String</span><span class="sxs-lookup"><span data-stu-id="ff34f-126">String</span></span>| <span data-ttu-id="ff34f-127">Уникальный идентификатор unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff34f-127">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="ff34f-128">Ключ, а не значение null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff34f-128">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="ff34f-129">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ff34f-129">roleDefinitionId</span></span>|<span data-ttu-id="ff34f-130">String</span><span class="sxs-lookup"><span data-stu-id="ff34f-130">String</span></span>| <span data-ttu-id="ff34f-131">ИД unifiedRoleDefinition, для который требуется назначение.</span><span class="sxs-lookup"><span data-stu-id="ff34f-131">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="ff34f-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff34f-132">Read only.</span></span> |
|<span data-ttu-id="ff34f-133">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff34f-133">roleDefinition</span></span>|[<span data-ttu-id="ff34f-134">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ff34f-134">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="ff34f-135">Свойство, указывающее roleDefinition, для которого назначение.</span><span class="sxs-lookup"><span data-stu-id="ff34f-135">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="ff34f-136">Предоставляется для того, чтобы вызыватели могли получить определение роли одновременно с получением `$expand` назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ff34f-136">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="ff34f-137">roleDefinition.Id будет автоматически расширена</span><span class="sxs-lookup"><span data-stu-id="ff34f-137">roleDefinition.Id will be auto expanded</span></span>
|<span data-ttu-id="ff34f-138">principalId</span><span class="sxs-lookup"><span data-stu-id="ff34f-138">principalId</span></span>|<span data-ttu-id="ff34f-139">String</span><span class="sxs-lookup"><span data-stu-id="ff34f-139">String</span></span>| <span data-ttu-id="ff34f-140">Objectid основного объекта, которому предоставлено назначение.</span><span class="sxs-lookup"><span data-stu-id="ff34f-140">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="ff34f-141">principal</span><span class="sxs-lookup"><span data-stu-id="ff34f-141">principal</span></span>|[<span data-ttu-id="ff34f-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ff34f-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="ff34f-143">Свойство, ссылаясь на назначенного директора.</span><span class="sxs-lookup"><span data-stu-id="ff34f-143">Property referencing the assigned principal.</span></span> <span data-ttu-id="ff34f-144">Предоставляется для того, чтобы вызыватели могли получить основное значение одновременно с получением `$expand` назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ff34f-144">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="ff34f-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff34f-145">Read-only.</span></span> |
|<span data-ttu-id="ff34f-146">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="ff34f-146">directoryScopeId</span></span>|<span data-ttu-id="ff34f-147">String</span><span class="sxs-lookup"><span data-stu-id="ff34f-147">String</span></span>|<span data-ttu-id="ff34f-148">ИД объекта каталога, представляющего область назначения.</span><span class="sxs-lookup"><span data-stu-id="ff34f-148">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="ff34f-149">Область назначения определяет набор ресурсов, к которым был предоставлен доступ для основного.</span><span class="sxs-lookup"><span data-stu-id="ff34f-149">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="ff34f-150">Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="ff34f-150">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="ff34f-151">Области приложения — это области, которые определяются и понятны только этому приложению.</span><span class="sxs-lookup"><span data-stu-id="ff34f-151">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="ff34f-152">directoryScope</span><span class="sxs-lookup"><span data-stu-id="ff34f-152">directoryScope</span></span>|[<span data-ttu-id="ff34f-153">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ff34f-153">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="ff34f-154">Свойство, ссылаясь на объект каталога, который является областью назначения.</span><span class="sxs-lookup"><span data-stu-id="ff34f-154">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="ff34f-155">Предоставляется для того, чтобы вызыватели могли получить объект каталога одновременно с получением `$expand` назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ff34f-155">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="ff34f-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff34f-156">Read-only.</span></span> |
|<span data-ttu-id="ff34f-157">appScopeId</span><span class="sxs-lookup"><span data-stu-id="ff34f-157">appScopeId</span></span>|<span data-ttu-id="ff34f-158">String</span><span class="sxs-lookup"><span data-stu-id="ff34f-158">String</span></span>|<span data-ttu-id="ff34f-159">ИД конкретной области приложения, если область назначения является конкретной областью приложения.</span><span class="sxs-lookup"><span data-stu-id="ff34f-159">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="ff34f-160">Область назначения определяет набор ресурсов, к которым был предоставлен доступ для основного.</span><span class="sxs-lookup"><span data-stu-id="ff34f-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="ff34f-161">Области каталогов — это общие области, хранимые в каталоге, которые понимаются несколькими приложениями.</span><span class="sxs-lookup"><span data-stu-id="ff34f-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="ff34f-162">Используйте "/" для области на клиенте.</span><span class="sxs-lookup"><span data-stu-id="ff34f-162">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="ff34f-163">Области приложения — это области, которые определяются и понятны только этому приложению.</span><span class="sxs-lookup"><span data-stu-id="ff34f-163">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="ff34f-164">appScope</span><span class="sxs-lookup"><span data-stu-id="ff34f-164">appScope</span></span>|[<span data-ttu-id="ff34f-165">appScope</span><span class="sxs-lookup"><span data-stu-id="ff34f-165">appScope</span></span>](appscope.md)|<span data-ttu-id="ff34f-166">Свойство только для чтения с подробными сведениями об определенной области приложения, если область назначения является конкретной областью приложения.</span><span class="sxs-lookup"><span data-stu-id="ff34f-166">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="ff34f-167">Объект Containment.</span><span class="sxs-lookup"><span data-stu-id="ff34f-167">Containment entity.</span></span> |
|<span data-ttu-id="ff34f-168">resourceScope</span><span class="sxs-lookup"><span data-stu-id="ff34f-168">resourceScope</span></span>|<span data-ttu-id="ff34f-169">String</span><span class="sxs-lookup"><span data-stu-id="ff34f-169">String</span></span>| <span data-ttu-id="ff34f-170">Область применения unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff34f-170">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="ff34f-171">Это "/" для службы.</span><span class="sxs-lookup"><span data-stu-id="ff34f-171">This is "/" for service-wide.</span></span> <span data-ttu-id="ff34f-172">**НЕ ИСПОЛЬЗУЙТЕ. Это свойство скоро будет неподготовлено.**</span><span class="sxs-lookup"><span data-stu-id="ff34f-172">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff34f-173">Связи</span><span class="sxs-lookup"><span data-stu-id="ff34f-173">Relationships</span></span>

<span data-ttu-id="ff34f-174">Нет</span><span class="sxs-lookup"><span data-stu-id="ff34f-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff34f-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff34f-175">JSON representation</span></span>

<span data-ttu-id="ff34f-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff34f-176">The following is a JSON representation of the resource.</span></span>

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

