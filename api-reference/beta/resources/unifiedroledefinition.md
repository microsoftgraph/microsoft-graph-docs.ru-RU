---
title: тип ресурса unifiedRoleDefinition
description: Единое определение роли — это набор разрешений
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 1b0c80a5844abd5ce5fbbce477841d59f2859af4
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334565"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="df8d1-103">тип ресурса unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-103">unifiedRoleDefinition resource type</span></span>

<span data-ttu-id="df8d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df8d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df8d1-105">Представляет коллекцию разрешений с перечислением операций, таких как чтение, запись и удаление, которые могут выполняться поставщиком RBAC в рамках управления Microsoft 365 [RBAC](rolemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="df8d1-105">Represents a collection of permissions listing the operations, such as read, write, and delete, that can be performed by an RBAC provider, as part of Microsoft 365 RBAC [role management](rolemanagement.md).</span></span>

<span data-ttu-id="df8d1-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="df8d1-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="df8d1-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="df8d1-107">cloud PC</span></span> 
- <span data-ttu-id="df8d1-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="df8d1-108">device management (Intune)</span></span>
- <span data-ttu-id="df8d1-109">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="df8d1-109">directory (Azure AD)</span></span> 
- <span data-ttu-id="df8d1-110">управление правами (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="df8d1-110">entitlement management (Azure AD)</span></span>

> [!NOTE]
> <span data-ttu-id="df8d1-111">Поставщики облачных ПК и управления правами RBAC в настоящее время поддерживают только [список](../api/rbacapplication-list-roledefinitions.md) и [получают](../api/unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="df8d1-111">The cloud PC and entitlement management RBAC providers currently support only the [list](../api/rbacapplication-list-roledefinitions.md) and [get](../api/unifiedroledefinition-get.md) operations.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="df8d1-112">Методы</span><span class="sxs-lookup"><span data-stu-id="df8d1-112">Methods</span></span>

| <span data-ttu-id="df8d1-113">Метод</span><span class="sxs-lookup"><span data-stu-id="df8d1-113">Method</span></span>       | <span data-ttu-id="df8d1-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="df8d1-114">Return Type</span></span> | <span data-ttu-id="df8d1-115">Описание</span><span class="sxs-lookup"><span data-stu-id="df8d1-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="df8d1-116">Список unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-116">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="df8d1-117">[коллекция unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="df8d1-117">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="df8d1-118">Ознакомьтесь со списком объектов unifiedRoleDefinition и их свойствами.</span><span class="sxs-lookup"><span data-stu-id="df8d1-118">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="df8d1-119">Get unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-119">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="df8d1-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="df8d1-121">Ознакомьтесь с свойствами объекта unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="df8d1-121">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="df8d1-122">Создание unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-122">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="df8d1-123">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-123">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="df8d1-124">Создайте объект unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="df8d1-124">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="df8d1-125">Обновление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-125">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="df8d1-126">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-126">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="df8d1-127">Обновление объекта unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="df8d1-127">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="df8d1-128">Удаление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="df8d1-128">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="df8d1-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="df8d1-129">None</span></span> | <span data-ttu-id="df8d1-130">Удаление объекта unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="df8d1-130">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="df8d1-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="df8d1-131">Properties</span></span>

| <span data-ttu-id="df8d1-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="df8d1-132">Property</span></span>     | <span data-ttu-id="df8d1-133">Тип</span><span class="sxs-lookup"><span data-stu-id="df8d1-133">Type</span></span>        | <span data-ttu-id="df8d1-134">Описание</span><span class="sxs-lookup"><span data-stu-id="df8d1-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df8d1-135">description</span><span class="sxs-lookup"><span data-stu-id="df8d1-135">description</span></span>|<span data-ttu-id="df8d1-136">String</span><span class="sxs-lookup"><span data-stu-id="df8d1-136">String</span></span>| <span data-ttu-id="df8d1-137">Описание единогоRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="df8d1-137">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="df8d1-138">Только для чтения, **когда isBuiltIn** является правдой.</span><span class="sxs-lookup"><span data-stu-id="df8d1-138">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="df8d1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="df8d1-139">displayName</span></span>|<span data-ttu-id="df8d1-140">String</span><span class="sxs-lookup"><span data-stu-id="df8d1-140">String</span></span>| <span data-ttu-id="df8d1-141">Имя отображения для unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="df8d1-141">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="df8d1-142">Только для чтения, **когда isBuiltIn** является правдой.</span><span class="sxs-lookup"><span data-stu-id="df8d1-142">Read-only when **isBuiltIn** is true.</span></span> <span data-ttu-id="df8d1-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df8d1-143">Required.</span></span>  <span data-ttu-id="df8d1-144">Поддерживает `$filter` `eq` (и `startsWith` только операторов).</span><span class="sxs-lookup"><span data-stu-id="df8d1-144">Supports `$filter` (`eq` and `startsWith` operators only).</span></span>|
|<span data-ttu-id="df8d1-145">id</span><span class="sxs-lookup"><span data-stu-id="df8d1-145">id</span></span>|<span data-ttu-id="df8d1-146">String</span><span class="sxs-lookup"><span data-stu-id="df8d1-146">String</span></span>| <span data-ttu-id="df8d1-147">Уникальный идентификатор для единойRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="df8d1-147">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="df8d1-148">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="df8d1-148">Key, not nullable, Read-only.</span></span>  <span data-ttu-id="df8d1-149">Поддерживает `$filter` `eq` (только оператор).</span><span class="sxs-lookup"><span data-stu-id="df8d1-149">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="df8d1-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="df8d1-150">isBuiltIn</span></span>|<span data-ttu-id="df8d1-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8d1-151">Boolean</span></span>| <span data-ttu-id="df8d1-152">Флаг, указывающий, является ли unifiedRoleDefinition частью набора по умолчанию, включенного в продукт или настраиваемый.</span><span class="sxs-lookup"><span data-stu-id="df8d1-152">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="df8d1-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="df8d1-153">Read-only.</span></span>  <span data-ttu-id="df8d1-154">Поддерживает `$filter` `eq` (только оператор).</span><span class="sxs-lookup"><span data-stu-id="df8d1-154">Supports `$filter` (`eq` operator only).</span></span>|
|<span data-ttu-id="df8d1-155">isEnabled</span><span class="sxs-lookup"><span data-stu-id="df8d1-155">isEnabled</span></span>|<span data-ttu-id="df8d1-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="df8d1-156">Boolean</span></span>| <span data-ttu-id="df8d1-157">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="df8d1-157">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="df8d1-158">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="df8d1-158">If false the role is not available for assignment.</span></span> <span data-ttu-id="df8d1-159">Только для чтения, **когда isBuiltIn** является правдой.</span><span class="sxs-lookup"><span data-stu-id="df8d1-159">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="df8d1-160">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="df8d1-160">resourceScopes</span></span>|<span data-ttu-id="df8d1-161">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="df8d1-161">String collection</span></span>| <span data-ttu-id="df8d1-162">К списку областей применяются разрешения, предоставленные определением ролей.</span><span class="sxs-lookup"><span data-stu-id="df8d1-162">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="df8d1-163">В настоящее `/` время поддерживается только.</span><span class="sxs-lookup"><span data-stu-id="df8d1-163">Currently only `/` is supported.</span></span> <span data-ttu-id="df8d1-164">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="df8d1-164">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="df8d1-165">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это будет отохошено. Присоединение области к назначению ролей**</span><span class="sxs-lookup"><span data-stu-id="df8d1-165">**DO NOT USE. This will be deprecated soon. Attach scope to role assignment**</span></span> | 
|<span data-ttu-id="df8d1-166">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="df8d1-166">rolePermissions</span></span>|<span data-ttu-id="df8d1-167">[коллекция unifiedRolePermission](unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="df8d1-167">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="df8d1-168">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="df8d1-168">List of permissions included in the role.</span></span> <span data-ttu-id="df8d1-169">Только для чтения, **когда isBuiltIn** является правдой.</span><span class="sxs-lookup"><span data-stu-id="df8d1-169">Read-only when **isBuiltIn** is true.</span></span> <span data-ttu-id="df8d1-170">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df8d1-170">Required.</span></span> |
|<span data-ttu-id="df8d1-171">templateId</span><span class="sxs-lookup"><span data-stu-id="df8d1-171">templateId</span></span>|<span data-ttu-id="df8d1-172">String</span><span class="sxs-lookup"><span data-stu-id="df8d1-172">String</span></span>| <span data-ttu-id="df8d1-173">Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным.</span><span class="sxs-lookup"><span data-stu-id="df8d1-173">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="df8d1-174">Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах.</span><span class="sxs-lookup"><span data-stu-id="df8d1-174">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="df8d1-175">Только для чтения, **когда isBuiltIn** является правдой.</span><span class="sxs-lookup"><span data-stu-id="df8d1-175">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="df8d1-176">version</span><span class="sxs-lookup"><span data-stu-id="df8d1-176">version</span></span>|<span data-ttu-id="df8d1-177">String</span><span class="sxs-lookup"><span data-stu-id="df8d1-177">String</span></span>| <span data-ttu-id="df8d1-178">Указывает версию единойRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="df8d1-178">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="df8d1-179">Только для чтения, **когда isBuiltIn** является правдой.</span><span class="sxs-lookup"><span data-stu-id="df8d1-179">Read-only when **isBuiltIn** is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df8d1-180">Связи</span><span class="sxs-lookup"><span data-stu-id="df8d1-180">Relationships</span></span>

| <span data-ttu-id="df8d1-181">Связь</span><span class="sxs-lookup"><span data-stu-id="df8d1-181">Relationship</span></span> | <span data-ttu-id="df8d1-182">Тип</span><span class="sxs-lookup"><span data-stu-id="df8d1-182">Type</span></span>   |<span data-ttu-id="df8d1-183">Описание</span><span class="sxs-lookup"><span data-stu-id="df8d1-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df8d1-184">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="df8d1-184">inheritsPermissionsFrom</span></span>| <span data-ttu-id="df8d1-185">[коллекция unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="df8d1-185">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="df8d1-186">Только для чтения набор определений ролей, которые наследует заданное определение роли.</span><span class="sxs-lookup"><span data-stu-id="df8d1-186">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="df8d1-187">Только встроенные роли Azure AD поддерживают этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="df8d1-187">Only Azure AD built-in roles support this attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="df8d1-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df8d1-188">JSON representation</span></span>

<span data-ttu-id="df8d1-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df8d1-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": ["String"],
  "rolePermissions": [{"@odata.type": "microsoft.graph.unifiedRolePermission"}],
  "templateId": "String",
  "inheritsPermissionsFrom": [{"@odata.type": "microsoft.graph.unifiedRoleDefinition"}],
  "version": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


