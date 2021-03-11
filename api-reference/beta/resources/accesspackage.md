---
title: тип ресурса accessPackage
description: Пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам для одного или более пользователей.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 98e9a22137f9f6faaa39fbbb010a32b40f8f0254
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720846"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="bd6de-103">тип ресурса accessPackage</span><span class="sxs-lookup"><span data-stu-id="bd6de-103">accessPackage resource type</span></span>

<span data-ttu-id="bd6de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd6de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd6de-105">В управлении правами [Azure AD](entitlementmanagement-root.md)пакет доступа определяет коллекции ролей ресурсов и политики получения доступа к этим ресурсам одним или более пользователями.</span><span class="sxs-lookup"><span data-stu-id="bd6de-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="bd6de-106">Каждый пакет доступа ссылается на единый каталог пакетов доступа и имеет ссылки на ресурсы из этого каталога с помощью областей ролей, определенных ресурсами, которые определяют доступ, который предоставляет пакет.</span><span class="sxs-lookup"><span data-stu-id="bd6de-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="bd6de-107">Пакет доступа также связывается с политиками назначения пакета доступа, каждая из которых определяет, кто может запрашивать или кому назначено назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bd6de-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="bd6de-108">Чтобы назначить пользователя пакету доступа, создайте [accessPackageAssignmentRequest,](../api/accesspackageassignmentrequest-post.md) который ссылается на политику назначения пакета доступа и пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bd6de-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="bd6de-109">Методы</span><span class="sxs-lookup"><span data-stu-id="bd6de-109">Methods</span></span>

| <span data-ttu-id="bd6de-110">Метод</span><span class="sxs-lookup"><span data-stu-id="bd6de-110">Method</span></span>       | <span data-ttu-id="bd6de-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd6de-111">Return Type</span></span> | <span data-ttu-id="bd6de-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bd6de-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bd6de-113">Пакеты доступа к спискам</span><span class="sxs-lookup"><span data-stu-id="bd6de-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="bd6de-114">[коллекция accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="bd6de-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="bd6de-115">Извлечение списка **объектов accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="bd6de-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="bd6de-116">Создание accessPackage</span><span class="sxs-lookup"><span data-stu-id="bd6de-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="bd6de-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="bd6de-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="bd6de-118">Создайте новый **объект accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="bd6de-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="bd6de-119">Получить accessPackage</span><span class="sxs-lookup"><span data-stu-id="bd6de-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="bd6de-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="bd6de-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="bd6de-121">Чтение свойств и связей объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="bd6de-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="bd6de-122">Обновление accessPackage</span><span class="sxs-lookup"><span data-stu-id="bd6de-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="bd6de-123">Нет</span><span class="sxs-lookup"><span data-stu-id="bd6de-123">None</span></span> | <span data-ttu-id="bd6de-124">Обновление свойств объекта **accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="bd6de-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="bd6de-125">Удаление accessPackage</span><span class="sxs-lookup"><span data-stu-id="bd6de-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="bd6de-126">Нет</span><span class="sxs-lookup"><span data-stu-id="bd6de-126">None</span></span> | <span data-ttu-id="bd6de-127">Удаление **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="bd6de-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="bd6de-128">Список accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="bd6de-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="bd6de-129">[коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="bd6de-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="bd6de-130">Извлечение списка **объектов accessPackageResourceRoleScope** для этого пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bd6de-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="bd6de-131">Создание accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="bd6de-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="bd6de-132">Нет</span><span class="sxs-lookup"><span data-stu-id="bd6de-132">None</span></span> | <span data-ttu-id="bd6de-133">Создайте новый **объект accessPackageResourceRoleScope** для этого пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bd6de-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="bd6de-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd6de-134">Properties</span></span>

| <span data-ttu-id="bd6de-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd6de-135">Property</span></span>     | <span data-ttu-id="bd6de-136">Тип</span><span class="sxs-lookup"><span data-stu-id="bd6de-136">Type</span></span>        | <span data-ttu-id="bd6de-137">Описание</span><span class="sxs-lookup"><span data-stu-id="bd6de-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bd6de-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="bd6de-138">catalogId</span></span>|<span data-ttu-id="bd6de-139">String</span><span class="sxs-lookup"><span data-stu-id="bd6de-139">String</span></span>|<span data-ttu-id="bd6de-140">ID каталога пакетов доступа, ссылаясь на этот пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="bd6de-140">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="bd6de-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd6de-141">Read-only.</span></span>|
|<span data-ttu-id="bd6de-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="bd6de-142">createdBy</span></span>|<span data-ttu-id="bd6de-143">String</span><span class="sxs-lookup"><span data-stu-id="bd6de-143">String</span></span>|<span data-ttu-id="bd6de-144">UPN пользователя или удостоверения субъекта, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="bd6de-144">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="bd6de-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd6de-145">Read-only.</span></span>|
|<span data-ttu-id="bd6de-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd6de-146">createdDateTime</span></span>|<span data-ttu-id="bd6de-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd6de-147">DateTimeOffset</span></span>|<span data-ttu-id="bd6de-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bd6de-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bd6de-149">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="bd6de-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="bd6de-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd6de-150">Read-only.</span></span>|
|<span data-ttu-id="bd6de-151">description</span><span class="sxs-lookup"><span data-stu-id="bd6de-151">description</span></span>|<span data-ttu-id="bd6de-152">String</span><span class="sxs-lookup"><span data-stu-id="bd6de-152">String</span></span>|<span data-ttu-id="bd6de-153">Описание пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bd6de-153">The description of the access package.</span></span>|
|<span data-ttu-id="bd6de-154">displayName</span><span class="sxs-lookup"><span data-stu-id="bd6de-154">displayName</span></span>|<span data-ttu-id="bd6de-155">String</span><span class="sxs-lookup"><span data-stu-id="bd6de-155">String</span></span>|<span data-ttu-id="bd6de-156">Отображение имени пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bd6de-156">The display name of the access package.</span></span>|
|<span data-ttu-id="bd6de-157">id</span><span class="sxs-lookup"><span data-stu-id="bd6de-157">id</span></span>|<span data-ttu-id="bd6de-158">String</span><span class="sxs-lookup"><span data-stu-id="bd6de-158">String</span></span>| <span data-ttu-id="bd6de-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd6de-159">Read-only.</span></span>|
|<span data-ttu-id="bd6de-160">isHidden</span><span class="sxs-lookup"><span data-stu-id="bd6de-160">isHidden</span></span>|<span data-ttu-id="bd6de-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd6de-161">Boolean</span></span>|<span data-ttu-id="bd6de-162">Скрыт ли пакет доступа от запросителя.</span><span class="sxs-lookup"><span data-stu-id="bd6de-162">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="bd6de-163">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="bd6de-163">isRoleScopesVisible</span></span>|<span data-ttu-id="bd6de-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd6de-164">Boolean</span></span>|<span data-ttu-id="bd6de-165">Указывает, видны ли области ролей.</span><span class="sxs-lookup"><span data-stu-id="bd6de-165">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="bd6de-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="bd6de-166">modifiedBy</span></span>|<span data-ttu-id="bd6de-167">String</span><span class="sxs-lookup"><span data-stu-id="bd6de-167">String</span></span>|<span data-ttu-id="bd6de-168">UpN пользователя, который в последний раз изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="bd6de-168">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="bd6de-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd6de-169">Read-only.</span></span>|
|<span data-ttu-id="bd6de-170">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd6de-170">modifiedDateTime</span></span>|<span data-ttu-id="bd6de-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd6de-171">DateTimeOffset</span></span>|<span data-ttu-id="bd6de-172">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bd6de-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bd6de-173">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="bd6de-173">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="bd6de-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd6de-174">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bd6de-175">Связи</span><span class="sxs-lookup"><span data-stu-id="bd6de-175">Relationships</span></span>

| <span data-ttu-id="bd6de-176">Связь</span><span class="sxs-lookup"><span data-stu-id="bd6de-176">Relationship</span></span> | <span data-ttu-id="bd6de-177">Тип</span><span class="sxs-lookup"><span data-stu-id="bd6de-177">Type</span></span>        | <span data-ttu-id="bd6de-178">Описание</span><span class="sxs-lookup"><span data-stu-id="bd6de-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bd6de-179">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="bd6de-179">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="bd6de-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span><span class="sxs-lookup"><span data-stu-id="bd6de-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="bd6de-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd6de-181">Read-only.</span></span> <span data-ttu-id="bd6de-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bd6de-182">Nullable.</span></span>|
|<span data-ttu-id="bd6de-183">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="bd6de-183">accessPackageCatalog</span></span>|[<span data-ttu-id="bd6de-184">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="bd6de-184">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="bd6de-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bd6de-185">Read-only.</span></span> <span data-ttu-id="bd6de-186">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bd6de-186">Nullable.</span></span>|
|<span data-ttu-id="bd6de-187">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="bd6de-187">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="bd6de-188">[коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="bd6de-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="bd6de-189">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bd6de-189">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd6de-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd6de-190">JSON representation</span></span>

<span data-ttu-id="bd6de-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd6de-191">The following is a JSON representation of the resource.</span></span>

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


