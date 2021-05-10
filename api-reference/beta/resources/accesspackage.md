---
title: тип ресурса accessPackage
description: Пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2d288465b04986b98de7b67fa049657b8bcf0a58
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298533"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="5eb98-103">тип ресурса accessPackage</span><span class="sxs-lookup"><span data-stu-id="5eb98-103">accessPackage resource type</span></span>

<span data-ttu-id="5eb98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eb98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eb98-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.</span><span class="sxs-lookup"><span data-stu-id="5eb98-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  

<span data-ttu-id="5eb98-106">Каждый пакет доступа ссылается на единый каталог пакетов доступа и имеет ссылки на ресурсы из этого каталога с помощью областей ролей, определенных ресурсами, которые определяют доступ, который предоставляет пакет.</span><span class="sxs-lookup"><span data-stu-id="5eb98-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="5eb98-107">Пакет доступа также связывается с политиками назначения пакета доступа, каждая из которых определяет, кто может запрашивать или кому назначено назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="5eb98-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="5eb98-108">Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на политику назначения пакета доступа и пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="5eb98-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="5eb98-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5eb98-109">Methods</span></span>

| <span data-ttu-id="5eb98-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5eb98-110">Method</span></span>       | <span data-ttu-id="5eb98-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5eb98-111">Return Type</span></span> | <span data-ttu-id="5eb98-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5eb98-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5eb98-113">Пакеты доступа к спискам</span><span class="sxs-lookup"><span data-stu-id="5eb98-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="5eb98-114">[коллекция accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="5eb98-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="5eb98-115">Извлечение списка **объектов accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="5eb98-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="5eb98-116">Создание accessPackage</span><span class="sxs-lookup"><span data-stu-id="5eb98-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="5eb98-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="5eb98-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="5eb98-118">Создайте новый **объект accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="5eb98-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="5eb98-119">Получить accessPackage</span><span class="sxs-lookup"><span data-stu-id="5eb98-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="5eb98-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="5eb98-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="5eb98-121">Чтение свойств и связей объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="5eb98-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="5eb98-122">Обновление accessPackage</span><span class="sxs-lookup"><span data-stu-id="5eb98-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="5eb98-123">Нет</span><span class="sxs-lookup"><span data-stu-id="5eb98-123">None</span></span> | <span data-ttu-id="5eb98-124">Обновление свойств объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="5eb98-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="5eb98-125">Удаление accessPackage</span><span class="sxs-lookup"><span data-stu-id="5eb98-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="5eb98-126">Нет</span><span class="sxs-lookup"><span data-stu-id="5eb98-126">None</span></span> | <span data-ttu-id="5eb98-127">Удаление **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="5eb98-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="5eb98-128">Список accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="5eb98-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="5eb98-129">[коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="5eb98-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="5eb98-130">Извлечение списка **объектов accessPackageResourceRoleScope** для этого пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="5eb98-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="5eb98-131">Создание accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="5eb98-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="5eb98-132">Нет</span><span class="sxs-lookup"><span data-stu-id="5eb98-132">None</span></span> | <span data-ttu-id="5eb98-133">Создайте новый **объект accessPackageResourceRoleScope** для этого пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="5eb98-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |
|[<span data-ttu-id="5eb98-134">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="5eb98-134">filterByCurrentUser</span></span>](../api/accesspackage-filterbycurrentuser.md)|<span data-ttu-id="5eb98-135">[коллекция accessPackage](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="5eb98-135">[accessPackage](../resources/accesspackage.md) collection</span></span>|<span data-ttu-id="5eb98-136">Извлечение списка **объектов accessPackage,** фильтруемых на входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="5eb98-136">Retrieve the list of **accessPackage** objects filtered on the signed-in user.</span></span>|

## <a name="properties"></a><span data-ttu-id="5eb98-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="5eb98-137">Properties</span></span>

| <span data-ttu-id="5eb98-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="5eb98-138">Property</span></span>     | <span data-ttu-id="5eb98-139">Тип</span><span class="sxs-lookup"><span data-stu-id="5eb98-139">Type</span></span>        | <span data-ttu-id="5eb98-140">Описание</span><span class="sxs-lookup"><span data-stu-id="5eb98-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5eb98-141">catalogId</span><span class="sxs-lookup"><span data-stu-id="5eb98-141">catalogId</span></span>|<span data-ttu-id="5eb98-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5eb98-142">String</span></span>|<span data-ttu-id="5eb98-143">ID каталога пакетов доступа, ссылаясь на этот пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="5eb98-143">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="5eb98-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eb98-144">Read-only.</span></span>|
|<span data-ttu-id="5eb98-145">createdBy</span><span class="sxs-lookup"><span data-stu-id="5eb98-145">createdBy</span></span>|<span data-ttu-id="5eb98-146">String</span><span class="sxs-lookup"><span data-stu-id="5eb98-146">String</span></span>|<span data-ttu-id="5eb98-147">UPN пользователя или удостоверения субъекта, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="5eb98-147">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="5eb98-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eb98-148">Read-only.</span></span>|
|<span data-ttu-id="5eb98-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5eb98-149">createdDateTime</span></span>|<span data-ttu-id="5eb98-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eb98-150">DateTimeOffset</span></span>|<span data-ttu-id="5eb98-151">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5eb98-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5eb98-152">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5eb98-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5eb98-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eb98-153">Read-only.</span></span>|
|<span data-ttu-id="5eb98-154">description</span><span class="sxs-lookup"><span data-stu-id="5eb98-154">description</span></span>|<span data-ttu-id="5eb98-155">Строка</span><span class="sxs-lookup"><span data-stu-id="5eb98-155">String</span></span>|<span data-ttu-id="5eb98-156">Описание пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="5eb98-156">The description of the access package.</span></span>|
|<span data-ttu-id="5eb98-157">displayName</span><span class="sxs-lookup"><span data-stu-id="5eb98-157">displayName</span></span>|<span data-ttu-id="5eb98-158">Строка</span><span class="sxs-lookup"><span data-stu-id="5eb98-158">String</span></span>|<span data-ttu-id="5eb98-159">Отображение имени пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="5eb98-159">The display name of the access package.</span></span>|
|<span data-ttu-id="5eb98-160">id</span><span class="sxs-lookup"><span data-stu-id="5eb98-160">id</span></span>|<span data-ttu-id="5eb98-161">String</span><span class="sxs-lookup"><span data-stu-id="5eb98-161">String</span></span>| <span data-ttu-id="5eb98-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eb98-162">Read-only.</span></span>|
|<span data-ttu-id="5eb98-163">isHidden</span><span class="sxs-lookup"><span data-stu-id="5eb98-163">isHidden</span></span>|<span data-ttu-id="5eb98-164">Логический</span><span class="sxs-lookup"><span data-stu-id="5eb98-164">Boolean</span></span>|<span data-ttu-id="5eb98-165">Скрыт ли пакет доступа от запросителя.</span><span class="sxs-lookup"><span data-stu-id="5eb98-165">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="5eb98-166">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="5eb98-166">isRoleScopesVisible</span></span>|<span data-ttu-id="5eb98-167">Логический</span><span class="sxs-lookup"><span data-stu-id="5eb98-167">Boolean</span></span>|<span data-ttu-id="5eb98-168">Указывает, видны ли области ролей.</span><span class="sxs-lookup"><span data-stu-id="5eb98-168">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="5eb98-169">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="5eb98-169">modifiedBy</span></span>|<span data-ttu-id="5eb98-170">Строка</span><span class="sxs-lookup"><span data-stu-id="5eb98-170">String</span></span>|<span data-ttu-id="5eb98-171">UpN пользователя, который в последний раз изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="5eb98-171">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="5eb98-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eb98-172">Read-only.</span></span>|
|<span data-ttu-id="5eb98-173">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5eb98-173">modifiedDateTime</span></span>|<span data-ttu-id="5eb98-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5eb98-174">DateTimeOffset</span></span>|<span data-ttu-id="5eb98-175">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5eb98-175">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5eb98-176">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5eb98-176">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5eb98-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eb98-177">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5eb98-178">Связи</span><span class="sxs-lookup"><span data-stu-id="5eb98-178">Relationships</span></span>

| <span data-ttu-id="5eb98-179">Связь</span><span class="sxs-lookup"><span data-stu-id="5eb98-179">Relationship</span></span> | <span data-ttu-id="5eb98-180">Тип</span><span class="sxs-lookup"><span data-stu-id="5eb98-180">Type</span></span>        | <span data-ttu-id="5eb98-181">Описание</span><span class="sxs-lookup"><span data-stu-id="5eb98-181">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5eb98-182">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="5eb98-182">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="5eb98-183">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span><span class="sxs-lookup"><span data-stu-id="5eb98-183">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="5eb98-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5eb98-p107">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5eb98-186">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5eb98-186">accessPackageCatalog</span></span>|[<span data-ttu-id="5eb98-187">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5eb98-187">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="5eb98-p108">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5eb98-p108">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5eb98-190">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="5eb98-190">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="5eb98-191">[коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="5eb98-191">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="5eb98-192">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5eb98-192">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5eb98-193">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5eb98-193">JSON representation</span></span>

<span data-ttu-id="5eb98-194">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5eb98-194">The following is a JSON representation of the resource.</span></span>

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


