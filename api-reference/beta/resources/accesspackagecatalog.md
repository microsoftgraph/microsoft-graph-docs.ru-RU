---
title: тип ресурса accessPackageCatalog
description: Каталог пакетов доступа — это контейнер для пакетов доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 051657b5c8c7edb51a4c2c5c3a15bf3740052b86
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351099"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="5cc02-103">тип ресурса accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5cc02-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="5cc02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cc02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cc02-105">В [управлении правами Azure AD](entitlementmanagement-root.md)каталог пакетов доступа — это контейнер для пакетов с нулевым или более доступом.</span><span class="sxs-lookup"><span data-stu-id="5cc02-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span> <span data-ttu-id="5cc02-106">Каталог пакетов доступа также может иметь связанные ресурсы, которые используются в этих пакетах доступа для обеспечения доступа.</span><span class="sxs-lookup"><span data-stu-id="5cc02-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span> <span data-ttu-id="5cc02-107">Чтобы просмотреть или изменить членство ролей в [](unifiedroleassignment.md) каталоге, используйте API назначений ролей с поставщиком управления правами RBAC.</span><span class="sxs-lookup"><span data-stu-id="5cc02-107">To view or change the membership of catalog-scoped roles, use the [role assignments](unifiedroleassignment.md) API with the entitlement management RBAC provider.</span></span>



## <a name="methods"></a><span data-ttu-id="5cc02-108">Методы</span><span class="sxs-lookup"><span data-stu-id="5cc02-108">Methods</span></span>

| <span data-ttu-id="5cc02-109">Метод</span><span class="sxs-lookup"><span data-stu-id="5cc02-109">Method</span></span>       | <span data-ttu-id="5cc02-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5cc02-110">Return Type</span></span> | <span data-ttu-id="5cc02-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5cc02-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5cc02-112">Список accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="5cc02-112">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="5cc02-113">[коллекция accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="5cc02-113">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="5cc02-114">Извлечение списка объектов accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="5cc02-114">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="5cc02-115">Создание accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5cc02-115">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="5cc02-116">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5cc02-116">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="5cc02-117">Создайте новый объект accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="5cc02-117">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="5cc02-118">Получить accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5cc02-118">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="5cc02-119">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5cc02-119">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="5cc02-120">Чтение свойств и связей объекта accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="5cc02-120">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="5cc02-121">Обновление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5cc02-121">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="5cc02-122">Нет</span><span class="sxs-lookup"><span data-stu-id="5cc02-122">None</span></span> | <span data-ttu-id="5cc02-123">Обновление свойств объекта accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="5cc02-123">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="5cc02-124">Удаление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="5cc02-124">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="5cc02-125">Удаление accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="5cc02-125">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="5cc02-126">Ресурсы accessPackageCatalog списка</span><span class="sxs-lookup"><span data-stu-id="5cc02-126">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="5cc02-127">[коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="5cc02-127">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="5cc02-128">Извлечение списка объектов accessPackageResource в каталоге.</span><span class="sxs-lookup"><span data-stu-id="5cc02-128">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="5cc02-129">Роли ресурсов accessPackageCatalog в списке</span><span class="sxs-lookup"><span data-stu-id="5cc02-129">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="5cc02-130">[коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="5cc02-130">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="5cc02-131">Извлечение списка объектов accessPackageResourceRole для ресурсов в каталоге.</span><span class="sxs-lookup"><span data-stu-id="5cc02-131">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="5cc02-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cc02-132">Properties</span></span>

| <span data-ttu-id="5cc02-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cc02-133">Property</span></span>     | <span data-ttu-id="5cc02-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5cc02-134">Type</span></span>        | <span data-ttu-id="5cc02-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5cc02-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cc02-136">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="5cc02-136">catalogStatus</span></span>|<span data-ttu-id="5cc02-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5cc02-137">String</span></span>|<span data-ttu-id="5cc02-138">Имеет `Published` значение, если пакеты доступа доступны для управления.</span><span class="sxs-lookup"><span data-stu-id="5cc02-138">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="5cc02-139">catalogType</span><span class="sxs-lookup"><span data-stu-id="5cc02-139">catalogType</span></span>|<span data-ttu-id="5cc02-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5cc02-140">String</span></span>|<span data-ttu-id="5cc02-141">Один `UserManaged` из или `ServiceDefault` .</span><span class="sxs-lookup"><span data-stu-id="5cc02-141">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="5cc02-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="5cc02-142">createdBy</span></span>|<span data-ttu-id="5cc02-143">String</span><span class="sxs-lookup"><span data-stu-id="5cc02-143">String</span></span>|<span data-ttu-id="5cc02-144">UPN пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="5cc02-144">UPN of the user who created this resource.</span></span> <span data-ttu-id="5cc02-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cc02-145">Read-only.</span></span>|
|<span data-ttu-id="5cc02-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc02-146">createdDateTime</span></span>|<span data-ttu-id="5cc02-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cc02-147">DateTimeOffset</span></span>|<span data-ttu-id="5cc02-148">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5cc02-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cc02-149">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5cc02-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5cc02-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cc02-150">Read-only.</span></span>|
|<span data-ttu-id="5cc02-151">description</span><span class="sxs-lookup"><span data-stu-id="5cc02-151">description</span></span>|<span data-ttu-id="5cc02-152">Строка</span><span class="sxs-lookup"><span data-stu-id="5cc02-152">String</span></span>|<span data-ttu-id="5cc02-153">Описание каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="5cc02-153">The description of the access package catalog.</span></span>|
|<span data-ttu-id="5cc02-154">displayName</span><span class="sxs-lookup"><span data-stu-id="5cc02-154">displayName</span></span>|<span data-ttu-id="5cc02-155">Строка</span><span class="sxs-lookup"><span data-stu-id="5cc02-155">String</span></span>|<span data-ttu-id="5cc02-156">Отображение имени каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="5cc02-156">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="5cc02-157">id</span><span class="sxs-lookup"><span data-stu-id="5cc02-157">id</span></span>|<span data-ttu-id="5cc02-158">String</span><span class="sxs-lookup"><span data-stu-id="5cc02-158">String</span></span>| <span data-ttu-id="5cc02-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cc02-159">Read-only.</span></span>|
|<span data-ttu-id="5cc02-160">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="5cc02-160">isExternallyVisible</span></span>|<span data-ttu-id="5cc02-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cc02-161">Boolean</span></span>|<span data-ttu-id="5cc02-162">Могут ли пакеты доступа в этом каталоге запрашиваться пользователями за пределами клиента.</span><span class="sxs-lookup"><span data-stu-id="5cc02-162">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="5cc02-163">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="5cc02-163">modifiedBy</span></span>|<span data-ttu-id="5cc02-164">Строка</span><span class="sxs-lookup"><span data-stu-id="5cc02-164">String</span></span>|<span data-ttu-id="5cc02-165">UpN пользователя, который в последний раз изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="5cc02-165">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="5cc02-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cc02-166">Read-only.</span></span>|
|<span data-ttu-id="5cc02-167">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc02-167">modifiedDateTime</span></span>|<span data-ttu-id="5cc02-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cc02-168">DateTimeOffset</span></span>|<span data-ttu-id="5cc02-169">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5cc02-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cc02-170">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5cc02-170">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5cc02-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cc02-171">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="5cc02-172">Связи</span><span class="sxs-lookup"><span data-stu-id="5cc02-172">Relationships</span></span>

| <span data-ttu-id="5cc02-173">Связь</span><span class="sxs-lookup"><span data-stu-id="5cc02-173">Relationship</span></span> | <span data-ttu-id="5cc02-174">Тип</span><span class="sxs-lookup"><span data-stu-id="5cc02-174">Type</span></span>        | <span data-ttu-id="5cc02-175">Описание</span><span class="sxs-lookup"><span data-stu-id="5cc02-175">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5cc02-176">accessPackages</span><span class="sxs-lookup"><span data-stu-id="5cc02-176">accessPackages</span></span>|<span data-ttu-id="5cc02-177">[коллекция accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="5cc02-177">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="5cc02-178">Пакеты доступа в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="5cc02-178">The access packages in this catalog.</span></span> <span data-ttu-id="5cc02-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cc02-179">Read-only.</span></span> <span data-ttu-id="5cc02-180">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5cc02-180">Nullable.</span></span>|
|<span data-ttu-id="5cc02-181">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="5cc02-181">accessPackageResources</span></span>|<span data-ttu-id="5cc02-182">[коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="5cc02-182">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="5cc02-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5cc02-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5cc02-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cc02-185">JSON representation</span></span>

<span data-ttu-id="5cc02-186">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cc02-186">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package catalog",
    "displayName":"Access package catalog for testing",
    "isExternallyVisible":false,
    "catalogType":"UserManaged",
    "catalogStatus":"Published",
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
  "description": "accessPackageCatalog resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

