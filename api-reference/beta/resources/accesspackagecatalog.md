---
title: Тип ресурса accessPackageCatalog
description: Каталог пакетов доступа — это контейнер для пакетов доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97c683ca47f453efdcd267839b3a2239a400db66
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158634"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="794f0-103">Тип ресурса accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="794f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="794f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="794f0-105">В [службе управления правами Azure AD](entitlementmanagement-root.md)каталог пакетов доступа является контейнером для пакетов доступа с нуля или более.</span><span class="sxs-lookup"><span data-stu-id="794f0-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="794f0-106">Каталог пакетов доступа также может иметь связанные ресурсы, которые используются в этих пакетах доступа для предоставления доступа.</span><span class="sxs-lookup"><span data-stu-id="794f0-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="794f0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="794f0-107">Methods</span></span>

| <span data-ttu-id="794f0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="794f0-108">Method</span></span>       | <span data-ttu-id="794f0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="794f0-109">Return Type</span></span> | <span data-ttu-id="794f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="794f0-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="794f0-111">Список accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="794f0-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="794f0-112">[Коллекция accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="794f0-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="794f0-113">Получить список объектов accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="794f0-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="794f0-114">Создание accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="794f0-115">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="794f0-116">Создание объекта accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="794f0-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="794f0-117">Get accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="794f0-118">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="794f0-119">Чтение свойств и связей объекта accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="794f0-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="794f0-120">Обновление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-120">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="794f0-121">Нет</span><span class="sxs-lookup"><span data-stu-id="794f0-121">None</span></span> | <span data-ttu-id="794f0-122">Обновление свойств объекта accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="794f0-122">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="794f0-123">Удаление accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-123">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="794f0-124">Удаление accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="794f0-124">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="794f0-125">Список ресурсов accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-125">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="794f0-126">[Коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="794f0-126">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="794f0-127">Получить список объектов accessPackageResource в каталоге.</span><span class="sxs-lookup"><span data-stu-id="794f0-127">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="794f0-128">Список ролей ресурсов accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="794f0-128">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="794f0-129">[Коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="794f0-129">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="794f0-130">Получить список объектов accessPackageResourceRole для ресурсов в каталоге.</span><span class="sxs-lookup"><span data-stu-id="794f0-130">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="794f0-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="794f0-131">Properties</span></span>

| <span data-ttu-id="794f0-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="794f0-132">Property</span></span>     | <span data-ttu-id="794f0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="794f0-133">Type</span></span>        | <span data-ttu-id="794f0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="794f0-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="794f0-135">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="794f0-135">catalogStatus</span></span>|<span data-ttu-id="794f0-136">String</span><span class="sxs-lookup"><span data-stu-id="794f0-136">String</span></span>|<span data-ttu-id="794f0-137">Имеет `Published` значение, если пакеты доступа доступны для управления.</span><span class="sxs-lookup"><span data-stu-id="794f0-137">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="794f0-138">catalogType</span><span class="sxs-lookup"><span data-stu-id="794f0-138">catalogType</span></span>|<span data-ttu-id="794f0-139">String</span><span class="sxs-lookup"><span data-stu-id="794f0-139">String</span></span>|<span data-ttu-id="794f0-140">Один из `UserManaged` или `ServiceDefault` .</span><span class="sxs-lookup"><span data-stu-id="794f0-140">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="794f0-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="794f0-141">createdBy</span></span>|<span data-ttu-id="794f0-142">String</span><span class="sxs-lookup"><span data-stu-id="794f0-142">String</span></span>|<span data-ttu-id="794f0-143">Имя пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="794f0-143">UPN of the user who created this resource.</span></span> <span data-ttu-id="794f0-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="794f0-144">Read-only.</span></span>|
|<span data-ttu-id="794f0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="794f0-145">createdDateTime</span></span>|<span data-ttu-id="794f0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="794f0-146">DateTimeOffset</span></span>|<span data-ttu-id="794f0-147">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="794f0-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="794f0-148">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="794f0-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="794f0-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="794f0-149">Read-only.</span></span>|
|<span data-ttu-id="794f0-150">description</span><span class="sxs-lookup"><span data-stu-id="794f0-150">description</span></span>|<span data-ttu-id="794f0-151">String</span><span class="sxs-lookup"><span data-stu-id="794f0-151">String</span></span>|<span data-ttu-id="794f0-152">Описание каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="794f0-152">The description of the access package catalog.</span></span>|
|<span data-ttu-id="794f0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="794f0-153">displayName</span></span>|<span data-ttu-id="794f0-154">String</span><span class="sxs-lookup"><span data-stu-id="794f0-154">String</span></span>|<span data-ttu-id="794f0-155">Отображаемого имени каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="794f0-155">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="794f0-156">id</span><span class="sxs-lookup"><span data-stu-id="794f0-156">id</span></span>|<span data-ttu-id="794f0-157">String</span><span class="sxs-lookup"><span data-stu-id="794f0-157">String</span></span>| <span data-ttu-id="794f0-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="794f0-158">Read-only.</span></span>|
|<span data-ttu-id="794f0-159">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="794f0-159">isExternallyVisible</span></span>|<span data-ttu-id="794f0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="794f0-160">Boolean</span></span>|<span data-ttu-id="794f0-161">Могут ли пользователи за пределами клиента запрашивать пакеты доступа в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="794f0-161">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="794f0-162">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="794f0-162">modifiedBy</span></span>|<span data-ttu-id="794f0-163">String</span><span class="sxs-lookup"><span data-stu-id="794f0-163">String</span></span>|<span data-ttu-id="794f0-164">Имя пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="794f0-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="794f0-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="794f0-165">Read-only.</span></span>|
|<span data-ttu-id="794f0-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="794f0-166">modifiedDateTime</span></span>|<span data-ttu-id="794f0-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="794f0-167">DateTimeOffset</span></span>|<span data-ttu-id="794f0-168">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="794f0-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="794f0-169">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="794f0-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="794f0-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="794f0-170">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="794f0-171">Связи</span><span class="sxs-lookup"><span data-stu-id="794f0-171">Relationships</span></span>

| <span data-ttu-id="794f0-172">Связь</span><span class="sxs-lookup"><span data-stu-id="794f0-172">Relationship</span></span> | <span data-ttu-id="794f0-173">Тип</span><span class="sxs-lookup"><span data-stu-id="794f0-173">Type</span></span>        | <span data-ttu-id="794f0-174">Описание</span><span class="sxs-lookup"><span data-stu-id="794f0-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="794f0-175">accessPackages</span><span class="sxs-lookup"><span data-stu-id="794f0-175">accessPackages</span></span>|<span data-ttu-id="794f0-176">[Коллекция accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="794f0-176">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="794f0-177">Пакеты доступа в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="794f0-177">The access packages in this catalog.</span></span> <span data-ttu-id="794f0-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="794f0-178">Read-only.</span></span> <span data-ttu-id="794f0-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="794f0-179">Nullable.</span></span>|
|<span data-ttu-id="794f0-180">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="794f0-180">accessPackageResources</span></span>|<span data-ttu-id="794f0-181">[Коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="794f0-181">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="794f0-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="794f0-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="794f0-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="794f0-184">JSON representation</span></span>

<span data-ttu-id="794f0-185">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="794f0-185">The following is a JSON representation of the resource.</span></span>

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


