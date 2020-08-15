---
title: Тип ресурса Акцесспаккаже
description: Пакет Access определяет коллекции ролей ресурсов и политики, которые могут получить доступ к этим ресурсам для одного или нескольких пользователей.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 42c38793e3a8618d180dcf860bde0401397cacbd
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757239"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="449d4-103">Тип ресурса Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="449d4-103">accessPackage resource type</span></span>

<span data-ttu-id="449d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="449d4-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="449d4-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)пакет Access определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="449d4-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="449d4-106">Каждый пакет Access ссылается на один каталог пакетов доступа и содержит ссылки на ресурсы из этого каталога с помощью областей ролей, определяющих доступ к пакету.</span><span class="sxs-lookup"><span data-stu-id="449d4-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="449d4-107">Пакет Access также содержит ссылки на политики назначения пакетов Access, каждый из которых определяет, кто может запрашивать или назначать назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="449d4-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="449d4-108">Чтобы назначить пользователя пакету Access, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , ссылающийся на политику назначения пакетов доступа и пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="449d4-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="449d4-109">Методы</span><span class="sxs-lookup"><span data-stu-id="449d4-109">Methods</span></span>

| <span data-ttu-id="449d4-110">Метод</span><span class="sxs-lookup"><span data-stu-id="449d4-110">Method</span></span>       | <span data-ttu-id="449d4-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="449d4-111">Return Type</span></span> | <span data-ttu-id="449d4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="449d4-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="449d4-113">Список Акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="449d4-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="449d4-114">Коллекция [акцесспаккаже](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="449d4-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="449d4-115">Получение списка объектов **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="449d4-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="449d4-116">Создание Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="449d4-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="449d4-117">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="449d4-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="449d4-118">Создание нового объекта **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="449d4-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="449d4-119">Получение Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="449d4-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="449d4-120">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="449d4-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="449d4-121">Чтение свойств и связей объекта **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="449d4-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="449d4-122">Обновление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="449d4-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="449d4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="449d4-123">None</span></span> | <span data-ttu-id="449d4-124">Обновление свойств объекта **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="449d4-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="449d4-125">Удаление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="449d4-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="449d4-126">Нет</span><span class="sxs-lookup"><span data-stu-id="449d4-126">None</span></span> | <span data-ttu-id="449d4-127">Удаление **акцесспаккаже**.</span><span class="sxs-lookup"><span data-stu-id="449d4-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="449d4-128">Список Акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="449d4-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="449d4-129">Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="449d4-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="449d4-130">Получение списка объектов **акцесспаккажересаурцеролескопе** для этого пакета Access.</span><span class="sxs-lookup"><span data-stu-id="449d4-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="449d4-131">Создание Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="449d4-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="449d4-132">Нет</span><span class="sxs-lookup"><span data-stu-id="449d4-132">None</span></span> | <span data-ttu-id="449d4-133">Создайте новый объект **акцесспаккажересаурцеролескопе** для этого пакета Access.</span><span class="sxs-lookup"><span data-stu-id="449d4-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="449d4-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="449d4-134">Properties</span></span>

| <span data-ttu-id="449d4-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="449d4-135">Property</span></span>     | <span data-ttu-id="449d4-136">Тип</span><span class="sxs-lookup"><span data-stu-id="449d4-136">Type</span></span>        | <span data-ttu-id="449d4-137">Описание</span><span class="sxs-lookup"><span data-stu-id="449d4-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="449d4-138">каталогид</span><span class="sxs-lookup"><span data-stu-id="449d4-138">catalogId</span></span>|<span data-ttu-id="449d4-139">Строка</span><span class="sxs-lookup"><span data-stu-id="449d4-139">String</span></span>|<span data-ttu-id="449d4-140">Идентификатор каталога пакетов доступа, на который ссылается этот пакет Access.</span><span class="sxs-lookup"><span data-stu-id="449d4-140">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="449d4-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="449d4-141">Read-only.</span></span>|
|<span data-ttu-id="449d4-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="449d4-142">createdBy</span></span>|<span data-ttu-id="449d4-143">Строка</span><span class="sxs-lookup"><span data-stu-id="449d4-143">String</span></span>|<span data-ttu-id="449d4-144">Имя участника-пользователя или идентификатор субъекта, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="449d4-144">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="449d4-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="449d4-145">Read-only.</span></span>|
|<span data-ttu-id="449d4-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="449d4-146">createdDateTime</span></span>|<span data-ttu-id="449d4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="449d4-147">DateTimeOffset</span></span>|<span data-ttu-id="449d4-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="449d4-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="449d4-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="449d4-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="449d4-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="449d4-150">Read-only.</span></span>|
|<span data-ttu-id="449d4-151">description</span><span class="sxs-lookup"><span data-stu-id="449d4-151">description</span></span>|<span data-ttu-id="449d4-152">String</span><span class="sxs-lookup"><span data-stu-id="449d4-152">String</span></span>|<span data-ttu-id="449d4-153">Описание пакета Access.</span><span class="sxs-lookup"><span data-stu-id="449d4-153">The description of the access package.</span></span>|
|<span data-ttu-id="449d4-154">displayName</span><span class="sxs-lookup"><span data-stu-id="449d4-154">displayName</span></span>|<span data-ttu-id="449d4-155">Строка</span><span class="sxs-lookup"><span data-stu-id="449d4-155">String</span></span>|<span data-ttu-id="449d4-156">Отображаемое имя пакета Access.</span><span class="sxs-lookup"><span data-stu-id="449d4-156">The display name of the access package.</span></span>|
|<span data-ttu-id="449d4-157">id</span><span class="sxs-lookup"><span data-stu-id="449d4-157">id</span></span>|<span data-ttu-id="449d4-158">String</span><span class="sxs-lookup"><span data-stu-id="449d4-158">String</span></span>| <span data-ttu-id="449d4-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="449d4-159">Read-only.</span></span>|
|<span data-ttu-id="449d4-160">Скрытый</span><span class="sxs-lookup"><span data-stu-id="449d4-160">isHidden</span></span>|<span data-ttu-id="449d4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="449d4-161">Boolean</span></span>|<span data-ttu-id="449d4-162">Указывает, является ли пакет доступа скрытым от запрашивающего.</span><span class="sxs-lookup"><span data-stu-id="449d4-162">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="449d4-163">исролескопесвисибле</span><span class="sxs-lookup"><span data-stu-id="449d4-163">isRoleScopesVisible</span></span>|<span data-ttu-id="449d4-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="449d4-164">Boolean</span></span>|<span data-ttu-id="449d4-165">Указывает, видимы ли области ролей.</span><span class="sxs-lookup"><span data-stu-id="449d4-165">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="449d4-166">модифиедби</span><span class="sxs-lookup"><span data-stu-id="449d4-166">modifiedBy</span></span>|<span data-ttu-id="449d4-167">Строка</span><span class="sxs-lookup"><span data-stu-id="449d4-167">String</span></span>|<span data-ttu-id="449d4-168">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="449d4-168">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="449d4-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="449d4-169">Read-only.</span></span>|
|<span data-ttu-id="449d4-170">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="449d4-170">modifiedDateTime</span></span>|<span data-ttu-id="449d4-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="449d4-171">DateTimeOffset</span></span>|<span data-ttu-id="449d4-172">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="449d4-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="449d4-173">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="449d4-173">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="449d4-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="449d4-174">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="449d4-175">Отношения</span><span class="sxs-lookup"><span data-stu-id="449d4-175">Relationships</span></span>

| <span data-ttu-id="449d4-176">Связь</span><span class="sxs-lookup"><span data-stu-id="449d4-176">Relationship</span></span> | <span data-ttu-id="449d4-177">Тип</span><span class="sxs-lookup"><span data-stu-id="449d4-177">Type</span></span>        | <span data-ttu-id="449d4-178">Описание</span><span class="sxs-lookup"><span data-stu-id="449d4-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="449d4-179">акцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="449d4-179">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="449d4-180">Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="449d4-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="449d4-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="449d4-181">Read-only.</span></span> <span data-ttu-id="449d4-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="449d4-182">Nullable.</span></span>|
|<span data-ttu-id="449d4-183">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="449d4-183">accessPackageCatalog</span></span>|[<span data-ttu-id="449d4-184">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="449d4-184">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="449d4-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="449d4-185">Read-only.</span></span> <span data-ttu-id="449d4-186">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="449d4-186">Nullable.</span></span>|
|<span data-ttu-id="449d4-187">акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="449d4-187">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="449d4-188">Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="449d4-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="449d4-189">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="449d4-189">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="449d4-190">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="449d4-190">JSON representation</span></span>

<span data-ttu-id="449d4-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="449d4-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "baseType": "",
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
