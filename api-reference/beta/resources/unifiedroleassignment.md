---
title: тип ресурса unifiedRoleAssignment
description: Назначение ролей — это связь между определением роли и главным в определенной области для предоставления доступа.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 04d296371a5d10dc447ea7588fdfbf5faea4f99d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442721"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="79e37-103">тип ресурса unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79e37-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="79e37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79e37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79e37-105">Для предоставления доступа к ресурсам используется единая системаRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79e37-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="79e37-106">Он представляет определение роли, назначенное основному (обычно пользователю) в определенной области.</span><span class="sxs-lookup"><span data-stu-id="79e37-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="79e37-107">Необходимо предоставить directoryScopeId или appScopeId.</span><span class="sxs-lookup"><span data-stu-id="79e37-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="79e37-108">Методы</span><span class="sxs-lookup"><span data-stu-id="79e37-108">Methods</span></span>

| <span data-ttu-id="79e37-109">Метод</span><span class="sxs-lookup"><span data-stu-id="79e37-109">Method</span></span>       | <span data-ttu-id="79e37-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="79e37-110">Return Type</span></span> | <span data-ttu-id="79e37-111">Описание</span><span class="sxs-lookup"><span data-stu-id="79e37-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="79e37-112">Get unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79e37-112">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="79e37-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79e37-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="79e37-114">Чтение свойств и связей объекта unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79e37-114">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="79e37-115">Создание unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79e37-115">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="79e37-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79e37-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="79e37-117">Создайте новую унифицированную функциюRoleAssignment, разместив в коллекции roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79e37-117">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="79e37-118">Удаление unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="79e37-118">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="79e37-119">Нет</span><span class="sxs-lookup"><span data-stu-id="79e37-119">None</span></span> | <span data-ttu-id="79e37-120">Удаление объекта unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79e37-120">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="79e37-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="79e37-121">Properties</span></span>

| <span data-ttu-id="79e37-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="79e37-122">Property</span></span>     | <span data-ttu-id="79e37-123">Тип</span><span class="sxs-lookup"><span data-stu-id="79e37-123">Type</span></span>        | <span data-ttu-id="79e37-124">Описание</span><span class="sxs-lookup"><span data-stu-id="79e37-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79e37-125">id</span><span class="sxs-lookup"><span data-stu-id="79e37-125">id</span></span>|<span data-ttu-id="79e37-126">String</span><span class="sxs-lookup"><span data-stu-id="79e37-126">String</span></span>| <span data-ttu-id="79e37-127">Уникальный идентификатор для единойRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79e37-127">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="79e37-128">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="79e37-128">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="79e37-129">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="79e37-129">roleDefinitionId</span></span>|<span data-ttu-id="79e37-130">String</span><span class="sxs-lookup"><span data-stu-id="79e37-130">String</span></span>| <span data-ttu-id="79e37-131">ID унифицированногоRoleDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="79e37-131">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="79e37-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79e37-132">Read only.</span></span> |
|<span data-ttu-id="79e37-133">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="79e37-133">roleDefinition</span></span>|[<span data-ttu-id="79e37-134">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="79e37-134">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="79e37-135">Свойство, указывающее рольDefinition для назначения.</span><span class="sxs-lookup"><span data-stu-id="79e37-135">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="79e37-136">При условии, что вызыватели могут получать определение роли, используя одновременно `$expand` с назначением роли.</span><span class="sxs-lookup"><span data-stu-id="79e37-136">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="79e37-137">roleDefinition.Id будет автоматически расширена</span><span class="sxs-lookup"><span data-stu-id="79e37-137">roleDefinition.Id will be auto expanded</span></span>
|<span data-ttu-id="79e37-138">principalId</span><span class="sxs-lookup"><span data-stu-id="79e37-138">principalId</span></span>|<span data-ttu-id="79e37-139">String</span><span class="sxs-lookup"><span data-stu-id="79e37-139">String</span></span>| <span data-ttu-id="79e37-140">Объект объекта, которому предоставляется назначение.</span><span class="sxs-lookup"><span data-stu-id="79e37-140">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="79e37-141">основной</span><span class="sxs-lookup"><span data-stu-id="79e37-141">principal</span></span>|[<span data-ttu-id="79e37-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="79e37-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="79e37-143">Свойство, ссылаясь на назначенного доверенного.</span><span class="sxs-lookup"><span data-stu-id="79e37-143">Property referencing the assigned principal.</span></span> <span data-ttu-id="79e37-144">При условии, что звонители могут получать основное использование одновременно с `$expand` назначением ролей.</span><span class="sxs-lookup"><span data-stu-id="79e37-144">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="79e37-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79e37-145">Read-only.</span></span> |
|<span data-ttu-id="79e37-146">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="79e37-146">directoryScopeId</span></span>|<span data-ttu-id="79e37-147">String</span><span class="sxs-lookup"><span data-stu-id="79e37-147">String</span></span>|<span data-ttu-id="79e37-148">Id объекта каталога, представляющего область назначения.</span><span class="sxs-lookup"><span data-stu-id="79e37-148">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="79e37-149">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="79e37-149">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="79e37-150">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="79e37-150">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="79e37-151">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="79e37-151">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="79e37-152">directoryScope</span><span class="sxs-lookup"><span data-stu-id="79e37-152">directoryScope</span></span>|[<span data-ttu-id="79e37-153">directoryObject</span><span class="sxs-lookup"><span data-stu-id="79e37-153">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="79e37-154">Свойство, ссылаясь на объект каталога, который является областью назначения.</span><span class="sxs-lookup"><span data-stu-id="79e37-154">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="79e37-155">При условии, что вызыватели могут получать объект каталога с помощью одновременно с назначением `$expand` ролей.</span><span class="sxs-lookup"><span data-stu-id="79e37-155">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="79e37-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79e37-156">Read-only.</span></span> |
|<span data-ttu-id="79e37-157">appScopeId</span><span class="sxs-lookup"><span data-stu-id="79e37-157">appScopeId</span></span>|<span data-ttu-id="79e37-158">String</span><span class="sxs-lookup"><span data-stu-id="79e37-158">String</span></span>|<span data-ttu-id="79e37-159">Id конкретной области приложения, когда область назначения является конкретной.</span><span class="sxs-lookup"><span data-stu-id="79e37-159">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="79e37-160">Область назначения определяет набор ресурсов, к которым доверителем был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="79e37-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="79e37-161">Области каталогов — это общие области, хранимые в каталоге, понятные нескольким приложениям.</span><span class="sxs-lookup"><span data-stu-id="79e37-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="79e37-162">Используйте "/" для области для клиента.</span><span class="sxs-lookup"><span data-stu-id="79e37-162">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="79e37-163">Области приложений — это области, которые определяются и понимаются только этим приложением.</span><span class="sxs-lookup"><span data-stu-id="79e37-163">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="79e37-164">appScope</span><span class="sxs-lookup"><span data-stu-id="79e37-164">appScope</span></span>|[<span data-ttu-id="79e37-165">appScope</span><span class="sxs-lookup"><span data-stu-id="79e37-165">appScope</span></span>](appscope.md)|<span data-ttu-id="79e37-166">Свойство только для чтения с подробными сведениями о области приложения, если область назначения является конкретной.</span><span class="sxs-lookup"><span data-stu-id="79e37-166">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="79e37-167">Объект containment.</span><span class="sxs-lookup"><span data-stu-id="79e37-167">Containment entity.</span></span> |
|<span data-ttu-id="79e37-168">resourceScope</span><span class="sxs-lookup"><span data-stu-id="79e37-168">resourceScope</span></span>|<span data-ttu-id="79e37-169">String</span><span class="sxs-lookup"><span data-stu-id="79e37-169">String</span></span>| <span data-ttu-id="79e37-170">Область применения unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="79e37-170">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="79e37-171">Это "/" для всей службы.</span><span class="sxs-lookup"><span data-stu-id="79e37-171">This is "/" for service-wide.</span></span> <span data-ttu-id="79e37-172">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось.**</span><span class="sxs-lookup"><span data-stu-id="79e37-172">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="79e37-173">Связи</span><span class="sxs-lookup"><span data-stu-id="79e37-173">Relationships</span></span>

<span data-ttu-id="79e37-174">Нет</span><span class="sxs-lookup"><span data-stu-id="79e37-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79e37-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79e37-175">JSON representation</span></span>

<span data-ttu-id="79e37-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79e37-176">The following is a JSON representation of the resource.</span></span>

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

