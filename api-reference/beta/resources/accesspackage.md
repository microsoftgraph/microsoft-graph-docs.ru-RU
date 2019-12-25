---
title: Тип ресурса Акцесспаккаже
description: Пакет Access определяет коллекции ролей ресурсов и политики, которые могут получить доступ к этим ресурсам для одного или нескольких пользователей.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a944309d59383b8c1501495c12d937acb13adbbb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870983"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="d7d98-103">Тип ресурса Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="d7d98-103">accessPackage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7d98-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)пакет Access определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="d7d98-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="d7d98-105">Каждый пакет Access ссылается на один каталог пакетов доступа и содержит ссылки на ресурсы из этого каталога с помощью областей ролей, определяющих доступ к пакету.</span><span class="sxs-lookup"><span data-stu-id="d7d98-105">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="d7d98-106">Пакет Access также содержит ссылки на политики назначения пакетов Access, каждый из которых определяет, кто может запрашивать или назначать назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d7d98-106">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="d7d98-107">Чтобы назначить пользователя пакету Access, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , ссылающийся на политику назначения пакетов доступа и пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="d7d98-107">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="d7d98-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d7d98-108">Methods</span></span>

| <span data-ttu-id="d7d98-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d7d98-109">Method</span></span>       | <span data-ttu-id="d7d98-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d7d98-110">Return Type</span></span> | <span data-ttu-id="d7d98-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d98-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d7d98-112">Список Акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="d7d98-112">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="d7d98-113">Коллекция [акцесспаккаже](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="d7d98-113">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="d7d98-114">Получение списка объектов **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="d7d98-114">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="d7d98-115">Создание Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="d7d98-115">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="d7d98-116">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="d7d98-116">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="d7d98-117">Создание нового объекта **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="d7d98-117">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="d7d98-118">Получение Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="d7d98-118">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="d7d98-119">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="d7d98-119">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="d7d98-120">Чтение свойств и связей объекта **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="d7d98-120">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="d7d98-121">Удаление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="d7d98-121">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="d7d98-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="d7d98-122">None</span></span> | <span data-ttu-id="d7d98-123">Удаление **акцесспаккаже**.</span><span class="sxs-lookup"><span data-stu-id="d7d98-123">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="d7d98-124">Список Акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="d7d98-124">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="d7d98-125">Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="d7d98-125">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="d7d98-126">Получение списка объектов **акцесспаккажересаурцеролескопе** для этого пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d7d98-126">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="d7d98-127">Создание Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="d7d98-127">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="d7d98-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="d7d98-128">None</span></span> | <span data-ttu-id="d7d98-129">Создайте новый объект **акцесспаккажересаурцеролескопе** для этого пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d7d98-129">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="d7d98-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7d98-130">Properties</span></span>

| <span data-ttu-id="d7d98-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7d98-131">Property</span></span>     | <span data-ttu-id="d7d98-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d98-132">Type</span></span>        | <span data-ttu-id="d7d98-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d98-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7d98-134">каталогид</span><span class="sxs-lookup"><span data-stu-id="d7d98-134">catalogId</span></span>|<span data-ttu-id="d7d98-135">String</span><span class="sxs-lookup"><span data-stu-id="d7d98-135">String</span></span>|<span data-ttu-id="d7d98-136">Идентификатор каталога пакетов доступа, на который ссылается этот пакет Access.</span><span class="sxs-lookup"><span data-stu-id="d7d98-136">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="d7d98-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d98-137">Read-only.</span></span>|
|<span data-ttu-id="d7d98-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="d7d98-138">createdBy</span></span>|<span data-ttu-id="d7d98-139">String</span><span class="sxs-lookup"><span data-stu-id="d7d98-139">String</span></span>|<span data-ttu-id="d7d98-140">Имя участника-пользователя или идентификатор субъекта, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="d7d98-140">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="d7d98-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d98-141">Read-only.</span></span>|
|<span data-ttu-id="d7d98-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7d98-142">createdDateTime</span></span>|<span data-ttu-id="d7d98-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7d98-143">DateTimeOffset</span></span>|<span data-ttu-id="d7d98-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d7d98-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d7d98-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d7d98-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d7d98-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d98-146">Read-only.</span></span>|
|<span data-ttu-id="d7d98-147">description</span><span class="sxs-lookup"><span data-stu-id="d7d98-147">description</span></span>|<span data-ttu-id="d7d98-148">String</span><span class="sxs-lookup"><span data-stu-id="d7d98-148">String</span></span>|<span data-ttu-id="d7d98-149">Описание пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d7d98-149">The description of the access package.</span></span>|
|<span data-ttu-id="d7d98-150">displayName</span><span class="sxs-lookup"><span data-stu-id="d7d98-150">displayName</span></span>|<span data-ttu-id="d7d98-151">Строка</span><span class="sxs-lookup"><span data-stu-id="d7d98-151">String</span></span>|<span data-ttu-id="d7d98-152">Отображаемое имя пакета Access.</span><span class="sxs-lookup"><span data-stu-id="d7d98-152">The display name of the access package.</span></span>|
|<span data-ttu-id="d7d98-153">id</span><span class="sxs-lookup"><span data-stu-id="d7d98-153">id</span></span>|<span data-ttu-id="d7d98-154">String</span><span class="sxs-lookup"><span data-stu-id="d7d98-154">String</span></span>| <span data-ttu-id="d7d98-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d98-155">Read-only.</span></span>|
|<span data-ttu-id="d7d98-156">Скрытый</span><span class="sxs-lookup"><span data-stu-id="d7d98-156">isHidden</span></span>|<span data-ttu-id="d7d98-157">Логический</span><span class="sxs-lookup"><span data-stu-id="d7d98-157">Boolean</span></span>|<span data-ttu-id="d7d98-158">Указывает, является ли пакет доступа скрытым от запрашивающего.</span><span class="sxs-lookup"><span data-stu-id="d7d98-158">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="d7d98-159">исролескопесвисибле</span><span class="sxs-lookup"><span data-stu-id="d7d98-159">isRoleScopesVisible</span></span>|<span data-ttu-id="d7d98-160">Логический</span><span class="sxs-lookup"><span data-stu-id="d7d98-160">Boolean</span></span>|<span data-ttu-id="d7d98-161">Указывает, видимы ли области ролей.</span><span class="sxs-lookup"><span data-stu-id="d7d98-161">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="d7d98-162">модифиедби</span><span class="sxs-lookup"><span data-stu-id="d7d98-162">modifiedBy</span></span>|<span data-ttu-id="d7d98-163">String</span><span class="sxs-lookup"><span data-stu-id="d7d98-163">String</span></span>|<span data-ttu-id="d7d98-164">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="d7d98-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="d7d98-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d98-165">Read-only.</span></span>|
|<span data-ttu-id="d7d98-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7d98-166">modifiedDateTime</span></span>|<span data-ttu-id="d7d98-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7d98-167">DateTimeOffset</span></span>|<span data-ttu-id="d7d98-168">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d7d98-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d7d98-169">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d7d98-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d7d98-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d98-170">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d7d98-171">Отношения</span><span class="sxs-lookup"><span data-stu-id="d7d98-171">Relationships</span></span>

| <span data-ttu-id="d7d98-172">Связь</span><span class="sxs-lookup"><span data-stu-id="d7d98-172">Relationship</span></span> | <span data-ttu-id="d7d98-173">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d98-173">Type</span></span>        | <span data-ttu-id="d7d98-174">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d98-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d7d98-175">акцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="d7d98-175">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="d7d98-176">Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d7d98-176">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="d7d98-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d98-177">Read-only.</span></span> <span data-ttu-id="d7d98-178">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d7d98-178">Nullable.</span></span>|
|<span data-ttu-id="d7d98-179">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="d7d98-179">accessPackageCatalog</span></span>|[<span data-ttu-id="d7d98-180">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="d7d98-180">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="d7d98-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7d98-181">Read-only.</span></span> <span data-ttu-id="d7d98-182">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d7d98-182">Nullable.</span></span>|
|<span data-ttu-id="d7d98-183">акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="d7d98-183">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="d7d98-184">Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="d7d98-184">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="d7d98-185">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d7d98-185">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7d98-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7d98-186">JSON representation</span></span>

<span data-ttu-id="d7d98-187">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7d98-187">The following is a JSON representation of the resource.</span></span>

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
