---
title: Тип ресурса accessPackage
description: Пакет доступа определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e47b8076e70c5b7c792c0232c63ae9ce828ac146
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155645"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="7ac2b-103">Тип ресурса accessPackage</span><span class="sxs-lookup"><span data-stu-id="7ac2b-103">accessPackage resource type</span></span>

<span data-ttu-id="7ac2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ac2b-105">В службе управления правами [Azure AD](entitlementmanagement-root.md)пакет доступа определяет коллекции ролей ресурсов и политики предоставления доступа к этим ресурсам одним или более пользователями.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="7ac2b-106">Каждый пакет доступа ссылается на один каталог пакетов доступа и содержит ссылки на ресурсы из этого каталога через области ролей для определенных ресурсов, которые определяют доступ, который предоставляет пакет.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="7ac2b-107">Пакет доступа также ссылается на политики назначения пакетов доступа, каждая из которых определяет, кто может запрашивать или кому назначено назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="7ac2b-108">Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на пакет доступа и политику назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="7ac2b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="7ac2b-109">Methods</span></span>

| <span data-ttu-id="7ac2b-110">Метод</span><span class="sxs-lookup"><span data-stu-id="7ac2b-110">Method</span></span>       | <span data-ttu-id="7ac2b-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ac2b-111">Return Type</span></span> | <span data-ttu-id="7ac2b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac2b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7ac2b-113">Список accessPackages</span><span class="sxs-lookup"><span data-stu-id="7ac2b-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="7ac2b-114">[Коллекция accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="7ac2b-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="7ac2b-115">Получить список объектов **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="7ac2b-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="7ac2b-116">Создание accessPackage</span><span class="sxs-lookup"><span data-stu-id="7ac2b-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="7ac2b-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="7ac2b-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="7ac2b-118">Создание объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="7ac2b-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="7ac2b-119">Get accessPackage</span><span class="sxs-lookup"><span data-stu-id="7ac2b-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="7ac2b-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="7ac2b-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="7ac2b-121">Чтение свойств и связей объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="7ac2b-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="7ac2b-122">Обновление accessPackage</span><span class="sxs-lookup"><span data-stu-id="7ac2b-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="7ac2b-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7ac2b-123">None</span></span> | <span data-ttu-id="7ac2b-124">Обновление свойств объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="7ac2b-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="7ac2b-125">Удаление accessPackage</span><span class="sxs-lookup"><span data-stu-id="7ac2b-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="7ac2b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="7ac2b-126">None</span></span> | <span data-ttu-id="7ac2b-127">Удаление **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="7ac2b-128">Список accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="7ac2b-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="7ac2b-129">[Коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="7ac2b-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="7ac2b-130">Получить список объектов **accessPackageResourceRoleScope** для этого пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="7ac2b-131">Создание accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="7ac2b-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="7ac2b-132">Нет</span><span class="sxs-lookup"><span data-stu-id="7ac2b-132">None</span></span> | <span data-ttu-id="7ac2b-133">Создайте новый **объект accessPackageResourceRoleScope** для этого пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ac2b-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ac2b-134">Properties</span></span>

| <span data-ttu-id="7ac2b-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ac2b-135">Property</span></span>     | <span data-ttu-id="7ac2b-136">Тип</span><span class="sxs-lookup"><span data-stu-id="7ac2b-136">Type</span></span>        | <span data-ttu-id="7ac2b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac2b-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ac2b-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="7ac2b-138">catalogId</span></span>|<span data-ttu-id="7ac2b-139">String</span><span class="sxs-lookup"><span data-stu-id="7ac2b-139">String</span></span>|<span data-ttu-id="7ac2b-140">ИД каталога пакетов доступа, ссылаясь на этот пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-140">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="7ac2b-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-141">Read-only.</span></span>|
|<span data-ttu-id="7ac2b-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="7ac2b-142">createdBy</span></span>|<span data-ttu-id="7ac2b-143">String</span><span class="sxs-lookup"><span data-stu-id="7ac2b-143">String</span></span>|<span data-ttu-id="7ac2b-144">UpN пользователя или удостоверения субъекта, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-144">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="7ac2b-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-145">Read-only.</span></span>|
|<span data-ttu-id="7ac2b-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac2b-146">createdDateTime</span></span>|<span data-ttu-id="7ac2b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac2b-147">DateTimeOffset</span></span>|<span data-ttu-id="7ac2b-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7ac2b-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7ac2b-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7ac2b-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-150">Read-only.</span></span>|
|<span data-ttu-id="7ac2b-151">description</span><span class="sxs-lookup"><span data-stu-id="7ac2b-151">description</span></span>|<span data-ttu-id="7ac2b-152">String</span><span class="sxs-lookup"><span data-stu-id="7ac2b-152">String</span></span>|<span data-ttu-id="7ac2b-153">Описание пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-153">The description of the access package.</span></span>|
|<span data-ttu-id="7ac2b-154">displayName</span><span class="sxs-lookup"><span data-stu-id="7ac2b-154">displayName</span></span>|<span data-ttu-id="7ac2b-155">String</span><span class="sxs-lookup"><span data-stu-id="7ac2b-155">String</span></span>|<span data-ttu-id="7ac2b-156">Отображаемого имени пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-156">The display name of the access package.</span></span>|
|<span data-ttu-id="7ac2b-157">id</span><span class="sxs-lookup"><span data-stu-id="7ac2b-157">id</span></span>|<span data-ttu-id="7ac2b-158">String</span><span class="sxs-lookup"><span data-stu-id="7ac2b-158">String</span></span>| <span data-ttu-id="7ac2b-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-159">Read-only.</span></span>|
|<span data-ttu-id="7ac2b-160">isHidden</span><span class="sxs-lookup"><span data-stu-id="7ac2b-160">isHidden</span></span>|<span data-ttu-id="7ac2b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac2b-161">Boolean</span></span>|<span data-ttu-id="7ac2b-162">Является ли пакет доступа скрытым от запрашивателя.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-162">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="7ac2b-163">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="7ac2b-163">isRoleScopesVisible</span></span>|<span data-ttu-id="7ac2b-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac2b-164">Boolean</span></span>|<span data-ttu-id="7ac2b-165">Указывает, видны ли области ролей.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-165">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="7ac2b-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="7ac2b-166">modifiedBy</span></span>|<span data-ttu-id="7ac2b-167">String</span><span class="sxs-lookup"><span data-stu-id="7ac2b-167">String</span></span>|<span data-ttu-id="7ac2b-168">Имя пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-168">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="7ac2b-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-169">Read-only.</span></span>|
|<span data-ttu-id="7ac2b-170">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac2b-170">modifiedDateTime</span></span>|<span data-ttu-id="7ac2b-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac2b-171">DateTimeOffset</span></span>|<span data-ttu-id="7ac2b-172">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="7ac2b-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7ac2b-173">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-173">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7ac2b-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-174">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7ac2b-175">Связи</span><span class="sxs-lookup"><span data-stu-id="7ac2b-175">Relationships</span></span>

| <span data-ttu-id="7ac2b-176">Связь</span><span class="sxs-lookup"><span data-stu-id="7ac2b-176">Relationship</span></span> | <span data-ttu-id="7ac2b-177">Тип</span><span class="sxs-lookup"><span data-stu-id="7ac2b-177">Type</span></span>        | <span data-ttu-id="7ac2b-178">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac2b-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ac2b-179">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="7ac2b-179">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="7ac2b-180">[Коллекция accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7ac2b-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="7ac2b-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-181">Read-only.</span></span> <span data-ttu-id="7ac2b-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-182">Nullable.</span></span>|
|<span data-ttu-id="7ac2b-183">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7ac2b-183">accessPackageCatalog</span></span>|[<span data-ttu-id="7ac2b-184">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7ac2b-184">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="7ac2b-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-185">Read-only.</span></span> <span data-ttu-id="7ac2b-186">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-186">Nullable.</span></span>|
|<span data-ttu-id="7ac2b-187">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="7ac2b-187">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="7ac2b-188">[Коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="7ac2b-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="7ac2b-189">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-189">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ac2b-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ac2b-190">JSON representation</span></span>

<span data-ttu-id="7ac2b-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ac2b-191">The following is a JSON representation of the resource.</span></span>

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


