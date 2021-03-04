---
title: тип ресурса accessPackage
description: Пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a8dab67cfff9e695c94c7cbcf4549e49eb9812fa
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433294"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="98e66-103">тип ресурса accessPackage</span><span class="sxs-lookup"><span data-stu-id="98e66-103">accessPackage resource type</span></span>

<span data-ttu-id="98e66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98e66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98e66-105">В управлении правами [Azure AD](entitlementmanagement-root.md)пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам одним или более пользователями.</span><span class="sxs-lookup"><span data-stu-id="98e66-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="98e66-106">Каждый пакет доступа ссылается на единый каталог пакетов доступа и имеет ссылки на ресурсы из этого каталога с помощью областей ролей, определенных ресурсами, которые определяют доступ, который предоставляет пакет.</span><span class="sxs-lookup"><span data-stu-id="98e66-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="98e66-107">Пакет доступа также связывается с политиками назначения пакета доступа, каждая из которых определяет, кто может запрашивать или кому назначено назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="98e66-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="98e66-108">Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на политику назначения пакета доступа и пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="98e66-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="98e66-109">Методы</span><span class="sxs-lookup"><span data-stu-id="98e66-109">Methods</span></span>

| <span data-ttu-id="98e66-110">Метод</span><span class="sxs-lookup"><span data-stu-id="98e66-110">Method</span></span>       | <span data-ttu-id="98e66-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98e66-111">Return Type</span></span> | <span data-ttu-id="98e66-112">Описание</span><span class="sxs-lookup"><span data-stu-id="98e66-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="98e66-113">Пакеты доступа к спискам</span><span class="sxs-lookup"><span data-stu-id="98e66-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="98e66-114">[коллекция accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="98e66-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="98e66-115">Извлечение списка **объектов accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="98e66-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="98e66-116">Создание accessPackage</span><span class="sxs-lookup"><span data-stu-id="98e66-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="98e66-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="98e66-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="98e66-118">Создайте новый **объект accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="98e66-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="98e66-119">Получить accessPackage</span><span class="sxs-lookup"><span data-stu-id="98e66-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="98e66-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="98e66-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="98e66-121">Чтение свойств и связей объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="98e66-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="98e66-122">Обновление accessPackage</span><span class="sxs-lookup"><span data-stu-id="98e66-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="98e66-123">Нет</span><span class="sxs-lookup"><span data-stu-id="98e66-123">None</span></span> | <span data-ttu-id="98e66-124">Обновление свойств объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="98e66-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="98e66-125">Удаление accessPackage</span><span class="sxs-lookup"><span data-stu-id="98e66-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="98e66-126">Нет</span><span class="sxs-lookup"><span data-stu-id="98e66-126">None</span></span> | <span data-ttu-id="98e66-127">Удаление **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="98e66-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="98e66-128">Список accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="98e66-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="98e66-129">[коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="98e66-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="98e66-130">Извлечение списка **объектов accessPackageResourceRoleScope** для этого пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="98e66-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="98e66-131">Создание accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="98e66-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="98e66-132">Нет</span><span class="sxs-lookup"><span data-stu-id="98e66-132">None</span></span> | <span data-ttu-id="98e66-133">Создайте новый **объект accessPackageResourceRoleScope** для этого пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="98e66-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="98e66-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="98e66-134">Properties</span></span>

| <span data-ttu-id="98e66-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="98e66-135">Property</span></span>     | <span data-ttu-id="98e66-136">Тип</span><span class="sxs-lookup"><span data-stu-id="98e66-136">Type</span></span>        | <span data-ttu-id="98e66-137">Описание</span><span class="sxs-lookup"><span data-stu-id="98e66-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98e66-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="98e66-138">catalogId</span></span>|<span data-ttu-id="98e66-139">String</span><span class="sxs-lookup"><span data-stu-id="98e66-139">String</span></span>|<span data-ttu-id="98e66-140">ID каталога пакетов доступа, ссылаясь на этот пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="98e66-140">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="98e66-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e66-141">Read-only.</span></span>|
|<span data-ttu-id="98e66-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="98e66-142">createdBy</span></span>|<span data-ttu-id="98e66-143">String</span><span class="sxs-lookup"><span data-stu-id="98e66-143">String</span></span>|<span data-ttu-id="98e66-144">UPN пользователя или удостоверения субъекта, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="98e66-144">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="98e66-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e66-145">Read-only.</span></span>|
|<span data-ttu-id="98e66-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98e66-146">createdDateTime</span></span>|<span data-ttu-id="98e66-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e66-147">DateTimeOffset</span></span>|<span data-ttu-id="98e66-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="98e66-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="98e66-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="98e66-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="98e66-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e66-150">Read-only.</span></span>|
|<span data-ttu-id="98e66-151">description</span><span class="sxs-lookup"><span data-stu-id="98e66-151">description</span></span>|<span data-ttu-id="98e66-152">String</span><span class="sxs-lookup"><span data-stu-id="98e66-152">String</span></span>|<span data-ttu-id="98e66-153">Описание пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="98e66-153">The description of the access package.</span></span>|
|<span data-ttu-id="98e66-154">displayName</span><span class="sxs-lookup"><span data-stu-id="98e66-154">displayName</span></span>|<span data-ttu-id="98e66-155">String</span><span class="sxs-lookup"><span data-stu-id="98e66-155">String</span></span>|<span data-ttu-id="98e66-156">Отображение имени пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="98e66-156">The display name of the access package.</span></span>|
|<span data-ttu-id="98e66-157">id</span><span class="sxs-lookup"><span data-stu-id="98e66-157">id</span></span>|<span data-ttu-id="98e66-158">String</span><span class="sxs-lookup"><span data-stu-id="98e66-158">String</span></span>| <span data-ttu-id="98e66-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e66-159">Read-only.</span></span>|
|<span data-ttu-id="98e66-160">isHidden</span><span class="sxs-lookup"><span data-stu-id="98e66-160">isHidden</span></span>|<span data-ttu-id="98e66-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="98e66-161">Boolean</span></span>|<span data-ttu-id="98e66-162">Скрыт ли пакет доступа от запросителя.</span><span class="sxs-lookup"><span data-stu-id="98e66-162">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="98e66-163">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="98e66-163">isRoleScopesVisible</span></span>|<span data-ttu-id="98e66-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="98e66-164">Boolean</span></span>|<span data-ttu-id="98e66-165">Указывает, видны ли области ролей.</span><span class="sxs-lookup"><span data-stu-id="98e66-165">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="98e66-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="98e66-166">modifiedBy</span></span>|<span data-ttu-id="98e66-167">String</span><span class="sxs-lookup"><span data-stu-id="98e66-167">String</span></span>|<span data-ttu-id="98e66-168">UpN пользователя, который в последний раз изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="98e66-168">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="98e66-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e66-169">Read-only.</span></span>|
|<span data-ttu-id="98e66-170">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98e66-170">modifiedDateTime</span></span>|<span data-ttu-id="98e66-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98e66-171">DateTimeOffset</span></span>|<span data-ttu-id="98e66-172">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="98e66-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="98e66-173">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="98e66-173">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="98e66-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e66-174">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="98e66-175">Связи</span><span class="sxs-lookup"><span data-stu-id="98e66-175">Relationships</span></span>

| <span data-ttu-id="98e66-176">Связь</span><span class="sxs-lookup"><span data-stu-id="98e66-176">Relationship</span></span> | <span data-ttu-id="98e66-177">Тип</span><span class="sxs-lookup"><span data-stu-id="98e66-177">Type</span></span>        | <span data-ttu-id="98e66-178">Описание</span><span class="sxs-lookup"><span data-stu-id="98e66-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98e66-179">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="98e66-179">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="98e66-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span><span class="sxs-lookup"><span data-stu-id="98e66-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="98e66-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e66-181">Read-only.</span></span> <span data-ttu-id="98e66-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="98e66-182">Nullable.</span></span>|
|<span data-ttu-id="98e66-183">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="98e66-183">accessPackageCatalog</span></span>|[<span data-ttu-id="98e66-184">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="98e66-184">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="98e66-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e66-185">Read-only.</span></span> <span data-ttu-id="98e66-186">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="98e66-186">Nullable.</span></span>|
|<span data-ttu-id="98e66-187">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="98e66-187">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="98e66-188">[коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="98e66-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="98e66-189">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="98e66-189">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98e66-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98e66-190">JSON representation</span></span>

<span data-ttu-id="98e66-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98e66-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


