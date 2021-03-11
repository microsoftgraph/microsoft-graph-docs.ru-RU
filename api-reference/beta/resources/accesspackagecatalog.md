---
title: тип ресурса accessPackageCatalog
description: Каталог пакетов доступа — это контейнер для пакетов доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 87c2541179cd94472eadab692544a40a1d8b81b7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720433"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="320b2-103">тип ресурса accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="320b2-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="320b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="320b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="320b2-105">В [управлении правами Azure AD](entitlementmanagement-root.md)каталог пакетов доступа — это контейнер для пакетов с нулевым или более доступом.</span><span class="sxs-lookup"><span data-stu-id="320b2-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="320b2-106">Каталог пакетов доступа также может иметь связанные ресурсы, которые используются в этих пакетах доступа для обеспечения доступа.</span><span class="sxs-lookup"><span data-stu-id="320b2-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="320b2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="320b2-107">Methods</span></span>

| <span data-ttu-id="320b2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="320b2-108">Method</span></span>       | <span data-ttu-id="320b2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="320b2-109">Return Type</span></span> | <span data-ttu-id="320b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="320b2-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="320b2-111">Список accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="320b2-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="320b2-112">[коллекция accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="320b2-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="320b2-113">Извлечение списка объектов accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="320b2-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="320b2-114">Создание accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="320b2-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="320b2-115">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="320b2-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="320b2-116">Создайте новый объект accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="320b2-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="320b2-117">Получить accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="320b2-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="320b2-118">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="320b2-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="320b2-119">Чтение свойств и связей объекта accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="320b2-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="320b2-120">Обновление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="320b2-120">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="320b2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="320b2-121">None</span></span> | <span data-ttu-id="320b2-122">Обновление свойств объекта accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="320b2-122">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="320b2-123">Удаление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="320b2-123">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="320b2-124">Удаление accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="320b2-124">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="320b2-125">Ресурсы accessPackageCatalog списка</span><span class="sxs-lookup"><span data-stu-id="320b2-125">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="320b2-126">[коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="320b2-126">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="320b2-127">Извлечение списка объектов accessPackageResource в каталоге.</span><span class="sxs-lookup"><span data-stu-id="320b2-127">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="320b2-128">Роли ресурсов accessPackageCatalog в списке</span><span class="sxs-lookup"><span data-stu-id="320b2-128">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="320b2-129">[коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="320b2-129">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="320b2-130">Извлечение списка объектов accessPackageResourceRole для ресурсов в каталоге.</span><span class="sxs-lookup"><span data-stu-id="320b2-130">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="320b2-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="320b2-131">Properties</span></span>

| <span data-ttu-id="320b2-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="320b2-132">Property</span></span>     | <span data-ttu-id="320b2-133">Тип</span><span class="sxs-lookup"><span data-stu-id="320b2-133">Type</span></span>        | <span data-ttu-id="320b2-134">Описание</span><span class="sxs-lookup"><span data-stu-id="320b2-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="320b2-135">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="320b2-135">catalogStatus</span></span>|<span data-ttu-id="320b2-136">String</span><span class="sxs-lookup"><span data-stu-id="320b2-136">String</span></span>|<span data-ttu-id="320b2-137">Имеет `Published` значение, если пакеты доступа доступны для управления.</span><span class="sxs-lookup"><span data-stu-id="320b2-137">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="320b2-138">catalogType</span><span class="sxs-lookup"><span data-stu-id="320b2-138">catalogType</span></span>|<span data-ttu-id="320b2-139">String</span><span class="sxs-lookup"><span data-stu-id="320b2-139">String</span></span>|<span data-ttu-id="320b2-140">Один `UserManaged` из или `ServiceDefault` .</span><span class="sxs-lookup"><span data-stu-id="320b2-140">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="320b2-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="320b2-141">createdBy</span></span>|<span data-ttu-id="320b2-142">String</span><span class="sxs-lookup"><span data-stu-id="320b2-142">String</span></span>|<span data-ttu-id="320b2-143">UPN пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="320b2-143">UPN of the user who created this resource.</span></span> <span data-ttu-id="320b2-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="320b2-144">Read-only.</span></span>|
|<span data-ttu-id="320b2-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="320b2-145">createdDateTime</span></span>|<span data-ttu-id="320b2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="320b2-146">DateTimeOffset</span></span>|<span data-ttu-id="320b2-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="320b2-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="320b2-148">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="320b2-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="320b2-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="320b2-149">Read-only.</span></span>|
|<span data-ttu-id="320b2-150">description</span><span class="sxs-lookup"><span data-stu-id="320b2-150">description</span></span>|<span data-ttu-id="320b2-151">String</span><span class="sxs-lookup"><span data-stu-id="320b2-151">String</span></span>|<span data-ttu-id="320b2-152">Описание каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="320b2-152">The description of the access package catalog.</span></span>|
|<span data-ttu-id="320b2-153">displayName</span><span class="sxs-lookup"><span data-stu-id="320b2-153">displayName</span></span>|<span data-ttu-id="320b2-154">String</span><span class="sxs-lookup"><span data-stu-id="320b2-154">String</span></span>|<span data-ttu-id="320b2-155">Отображение имени каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="320b2-155">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="320b2-156">id</span><span class="sxs-lookup"><span data-stu-id="320b2-156">id</span></span>|<span data-ttu-id="320b2-157">String</span><span class="sxs-lookup"><span data-stu-id="320b2-157">String</span></span>| <span data-ttu-id="320b2-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="320b2-158">Read-only.</span></span>|
|<span data-ttu-id="320b2-159">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="320b2-159">isExternallyVisible</span></span>|<span data-ttu-id="320b2-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="320b2-160">Boolean</span></span>|<span data-ttu-id="320b2-161">Могут ли пакеты доступа в этом каталоге запрашиваться пользователями за пределами клиента.</span><span class="sxs-lookup"><span data-stu-id="320b2-161">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="320b2-162">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="320b2-162">modifiedBy</span></span>|<span data-ttu-id="320b2-163">String</span><span class="sxs-lookup"><span data-stu-id="320b2-163">String</span></span>|<span data-ttu-id="320b2-164">UpN пользователя, который в последний раз изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="320b2-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="320b2-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="320b2-165">Read-only.</span></span>|
|<span data-ttu-id="320b2-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="320b2-166">modifiedDateTime</span></span>|<span data-ttu-id="320b2-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="320b2-167">DateTimeOffset</span></span>|<span data-ttu-id="320b2-168">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="320b2-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="320b2-169">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="320b2-169">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="320b2-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="320b2-170">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="320b2-171">Связи</span><span class="sxs-lookup"><span data-stu-id="320b2-171">Relationships</span></span>

| <span data-ttu-id="320b2-172">Связь</span><span class="sxs-lookup"><span data-stu-id="320b2-172">Relationship</span></span> | <span data-ttu-id="320b2-173">Тип</span><span class="sxs-lookup"><span data-stu-id="320b2-173">Type</span></span>        | <span data-ttu-id="320b2-174">Описание</span><span class="sxs-lookup"><span data-stu-id="320b2-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="320b2-175">accessPackages</span><span class="sxs-lookup"><span data-stu-id="320b2-175">accessPackages</span></span>|<span data-ttu-id="320b2-176">[коллекция accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="320b2-176">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="320b2-177">Пакеты доступа в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="320b2-177">The access packages in this catalog.</span></span> <span data-ttu-id="320b2-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="320b2-178">Read-only.</span></span> <span data-ttu-id="320b2-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="320b2-179">Nullable.</span></span>|
|<span data-ttu-id="320b2-180">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="320b2-180">accessPackageResources</span></span>|<span data-ttu-id="320b2-181">[коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="320b2-181">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="320b2-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="320b2-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="320b2-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="320b2-184">JSON representation</span></span>

<span data-ttu-id="320b2-185">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="320b2-185">The following is a JSON representation of the resource.</span></span>

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


