---
title: Тип ресурса Акцесспаккаже
description: Пакет Access определяет коллекции ролей ресурсов и политики, которые могут получить доступ к этим ресурсам для одного или нескольких пользователей.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e4d7565cdb16eb2a6a0abb7a33344c70490e2616
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939224"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="75722-103">Тип ресурса Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="75722-103">accessPackage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75722-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)пакет Access определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.</span><span class="sxs-lookup"><span data-stu-id="75722-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="75722-105">Каждый пакет Access ссылается на один каталог пакетов доступа и содержит ссылки на ресурсы из этого каталога с помощью областей ролей, определяющих доступ к пакету.</span><span class="sxs-lookup"><span data-stu-id="75722-105">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="75722-106">Пакет Access также содержит ссылки на политики назначения пакетов Access, каждый из которых определяет, кто может запрашивать или назначать назначение пакета Access.</span><span class="sxs-lookup"><span data-stu-id="75722-106">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="75722-107">Чтобы назначить пользователя пакету Access, [Создайте акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) , ссылающийся на политику назначения пакетов доступа и пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="75722-107">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="75722-108">Методы</span><span class="sxs-lookup"><span data-stu-id="75722-108">Methods</span></span>

| <span data-ttu-id="75722-109">Метод</span><span class="sxs-lookup"><span data-stu-id="75722-109">Method</span></span>       | <span data-ttu-id="75722-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="75722-110">Return Type</span></span> | <span data-ttu-id="75722-111">Описание</span><span class="sxs-lookup"><span data-stu-id="75722-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="75722-112">Список Акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="75722-112">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="75722-113">Коллекция [акцесспаккаже](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="75722-113">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="75722-114">Получение списка объектов **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="75722-114">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="75722-115">Создание Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="75722-115">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="75722-116">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="75722-116">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="75722-117">Создание нового объекта **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="75722-117">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="75722-118">Получение Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="75722-118">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="75722-119">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="75722-119">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="75722-120">Чтение свойств и связей объекта **акцесспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="75722-120">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="75722-121">Удаление Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="75722-121">Delete accessPackage</span></span>](../api/accesspackage-delete.md) | | <span data-ttu-id="75722-122">Удаление **акцесспаккаже**.</span><span class="sxs-lookup"><span data-stu-id="75722-122">Delete an **accesspackage**.</span></span> |

## <a name="properties"></a><span data-ttu-id="75722-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="75722-123">Properties</span></span>

| <span data-ttu-id="75722-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="75722-124">Property</span></span>     | <span data-ttu-id="75722-125">Тип</span><span class="sxs-lookup"><span data-stu-id="75722-125">Type</span></span>        | <span data-ttu-id="75722-126">Описание</span><span class="sxs-lookup"><span data-stu-id="75722-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75722-127">каталогид</span><span class="sxs-lookup"><span data-stu-id="75722-127">catalogId</span></span>|<span data-ttu-id="75722-128">Строка</span><span class="sxs-lookup"><span data-stu-id="75722-128">String</span></span>|<span data-ttu-id="75722-129">Идентификатор каталога пакетов доступа, на который ссылается этот пакет Access.</span><span class="sxs-lookup"><span data-stu-id="75722-129">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="75722-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75722-130">Read-only.</span></span>|
|<span data-ttu-id="75722-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="75722-131">createdBy</span></span>|<span data-ttu-id="75722-132">Строка</span><span class="sxs-lookup"><span data-stu-id="75722-132">String</span></span>|<span data-ttu-id="75722-133">Имя участника-пользователя или идентификатор субъекта, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="75722-133">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="75722-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75722-134">Read-only.</span></span>|
|<span data-ttu-id="75722-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75722-135">createdDateTime</span></span>|<span data-ttu-id="75722-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75722-136">DateTimeOffset</span></span>|<span data-ttu-id="75722-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="75722-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75722-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="75722-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75722-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75722-139">Read-only.</span></span>|
|<span data-ttu-id="75722-140">description</span><span class="sxs-lookup"><span data-stu-id="75722-140">description</span></span>|<span data-ttu-id="75722-141">String</span><span class="sxs-lookup"><span data-stu-id="75722-141">String</span></span>|<span data-ttu-id="75722-142">Описание пакета Access.</span><span class="sxs-lookup"><span data-stu-id="75722-142">The description of the access package.</span></span>|
|<span data-ttu-id="75722-143">displayName</span><span class="sxs-lookup"><span data-stu-id="75722-143">displayName</span></span>|<span data-ttu-id="75722-144">Строка</span><span class="sxs-lookup"><span data-stu-id="75722-144">String</span></span>|<span data-ttu-id="75722-145">Отображаемое имя пакета Access.</span><span class="sxs-lookup"><span data-stu-id="75722-145">The display name of the access package.</span></span>|
|<span data-ttu-id="75722-146">id</span><span class="sxs-lookup"><span data-stu-id="75722-146">id</span></span>|<span data-ttu-id="75722-147">String</span><span class="sxs-lookup"><span data-stu-id="75722-147">String</span></span>| <span data-ttu-id="75722-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75722-148">Read-only.</span></span>|
|<span data-ttu-id="75722-149">Скрытый</span><span class="sxs-lookup"><span data-stu-id="75722-149">isHidden</span></span>|<span data-ttu-id="75722-150">Логический</span><span class="sxs-lookup"><span data-stu-id="75722-150">Boolean</span></span>|<span data-ttu-id="75722-151">Указывает, является ли пакет доступа скрытым от запрашивающего.</span><span class="sxs-lookup"><span data-stu-id="75722-151">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="75722-152">исролескопесвисибле</span><span class="sxs-lookup"><span data-stu-id="75722-152">isRoleScopesVisible</span></span>|<span data-ttu-id="75722-153">Логический</span><span class="sxs-lookup"><span data-stu-id="75722-153">Boolean</span></span>|<span data-ttu-id="75722-154">Указывает, видимы ли области ролей.</span><span class="sxs-lookup"><span data-stu-id="75722-154">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="75722-155">модифиедби</span><span class="sxs-lookup"><span data-stu-id="75722-155">modifiedBy</span></span>|<span data-ttu-id="75722-156">Строка</span><span class="sxs-lookup"><span data-stu-id="75722-156">String</span></span>|<span data-ttu-id="75722-157">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="75722-157">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="75722-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75722-158">Read-only.</span></span>|
|<span data-ttu-id="75722-159">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75722-159">modifiedDateTime</span></span>|<span data-ttu-id="75722-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75722-160">DateTimeOffset</span></span>|<span data-ttu-id="75722-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="75722-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75722-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="75722-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="75722-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75722-163">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="75722-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="75722-164">Relationships</span></span>

| <span data-ttu-id="75722-165">Связь</span><span class="sxs-lookup"><span data-stu-id="75722-165">Relationship</span></span> | <span data-ttu-id="75722-166">Тип</span><span class="sxs-lookup"><span data-stu-id="75722-166">Type</span></span>        | <span data-ttu-id="75722-167">Описание</span><span class="sxs-lookup"><span data-stu-id="75722-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75722-168">акцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="75722-168">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="75722-169">Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75722-169">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="75722-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75722-170">Read-only.</span></span> <span data-ttu-id="75722-171">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="75722-171">Nullable.</span></span>|
|<span data-ttu-id="75722-172">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="75722-172">accessPackageCatalog</span></span>|[<span data-ttu-id="75722-173">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="75722-173">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="75722-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75722-174">Read-only.</span></span> <span data-ttu-id="75722-175">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="75722-175">Nullable.</span></span>|
|<span data-ttu-id="75722-176">акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="75722-176">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="75722-177">Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="75722-177">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="75722-178">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="75722-178">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75722-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75722-179">JSON representation</span></span>

<span data-ttu-id="75722-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75722-180">The following is a JSON representation of the resource.</span></span>

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
