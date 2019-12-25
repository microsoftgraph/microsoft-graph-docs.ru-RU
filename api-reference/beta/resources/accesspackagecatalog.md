---
title: Тип ресурса Акцесспаккажекаталог
description: Каталог пакетов Access — это контейнер для пакетов Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c8fde3b6ead60cada5e663b2150ba463187b22b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870420"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="43554-103">Тип ресурса Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="43554-103">accessPackageCatalog resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43554-104">В [управлении обслуживанием Azure AD](entitlementmanagement-root.md)каталог пакетов Access — это контейнер для одного или нескольких пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="43554-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="43554-105">Каталог пакетов Access также может иметь связанные ресурсы, которые используются в этих пакетах доступа для предоставления доступа.</span><span class="sxs-lookup"><span data-stu-id="43554-105">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="43554-106">Методы</span><span class="sxs-lookup"><span data-stu-id="43554-106">Methods</span></span>

| <span data-ttu-id="43554-107">Метод</span><span class="sxs-lookup"><span data-stu-id="43554-107">Method</span></span>       | <span data-ttu-id="43554-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="43554-108">Return Type</span></span> | <span data-ttu-id="43554-109">Описание</span><span class="sxs-lookup"><span data-stu-id="43554-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="43554-110">Список Акцесспаккажекаталогс</span><span class="sxs-lookup"><span data-stu-id="43554-110">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="43554-111">Коллекция [акцесспаккажекаталог](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="43554-111">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="43554-112">Получение списка объектов акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="43554-112">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="43554-113">Создание Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="43554-113">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="43554-114">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="43554-114">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="43554-115">Создание нового объекта Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="43554-115">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="43554-116">Получение Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="43554-116">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="43554-117">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="43554-117">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="43554-118">Чтение свойств и связей объекта Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="43554-118">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="43554-119">Удаление Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="43554-119">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="43554-120">Удаление Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="43554-120">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="43554-121">Список ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="43554-121">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="43554-122">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="43554-122">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="43554-123">Получение списка объектов Акцесспаккажересаурце в каталоге.</span><span class="sxs-lookup"><span data-stu-id="43554-123">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="43554-124">Список ролей ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="43554-124">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="43554-125">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="43554-125">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="43554-126">Получение списка объектов Акцесспаккажересаурцероле для ресурсов в каталоге.</span><span class="sxs-lookup"><span data-stu-id="43554-126">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="43554-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="43554-127">Properties</span></span>

| <span data-ttu-id="43554-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="43554-128">Property</span></span>     | <span data-ttu-id="43554-129">Тип</span><span class="sxs-lookup"><span data-stu-id="43554-129">Type</span></span>        | <span data-ttu-id="43554-130">Описание</span><span class="sxs-lookup"><span data-stu-id="43554-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="43554-131">каталогстатус</span><span class="sxs-lookup"><span data-stu-id="43554-131">catalogStatus</span></span>|<span data-ttu-id="43554-132">String</span><span class="sxs-lookup"><span data-stu-id="43554-132">String</span></span>|<span data-ttu-id="43554-133">Имеет значение `Published` , если пакеты доступа доступны для управления.</span><span class="sxs-lookup"><span data-stu-id="43554-133">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="43554-134">каталогтипе</span><span class="sxs-lookup"><span data-stu-id="43554-134">catalogType</span></span>|<span data-ttu-id="43554-135">String</span><span class="sxs-lookup"><span data-stu-id="43554-135">String</span></span>|<span data-ttu-id="43554-136">Один из `UserManaged` или `ServiceDefault`.</span><span class="sxs-lookup"><span data-stu-id="43554-136">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="43554-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="43554-137">createdBy</span></span>|<span data-ttu-id="43554-138">String</span><span class="sxs-lookup"><span data-stu-id="43554-138">String</span></span>|<span data-ttu-id="43554-139">Имя участника-пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="43554-139">UPN of the user who created this resource.</span></span> <span data-ttu-id="43554-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43554-140">Read-only.</span></span>|
|<span data-ttu-id="43554-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43554-141">createdDateTime</span></span>|<span data-ttu-id="43554-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43554-142">DateTimeOffset</span></span>|<span data-ttu-id="43554-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="43554-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="43554-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="43554-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="43554-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43554-145">Read-only.</span></span>|
|<span data-ttu-id="43554-146">description</span><span class="sxs-lookup"><span data-stu-id="43554-146">description</span></span>|<span data-ttu-id="43554-147">String</span><span class="sxs-lookup"><span data-stu-id="43554-147">String</span></span>|<span data-ttu-id="43554-148">Описание каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="43554-148">The description of the access package catalog.</span></span>|
|<span data-ttu-id="43554-149">displayName</span><span class="sxs-lookup"><span data-stu-id="43554-149">displayName</span></span>|<span data-ttu-id="43554-150">Строка</span><span class="sxs-lookup"><span data-stu-id="43554-150">String</span></span>|<span data-ttu-id="43554-151">Отображаемое имя каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="43554-151">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="43554-152">id</span><span class="sxs-lookup"><span data-stu-id="43554-152">id</span></span>|<span data-ttu-id="43554-153">String</span><span class="sxs-lookup"><span data-stu-id="43554-153">String</span></span>| <span data-ttu-id="43554-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43554-154">Read-only.</span></span>|
|<span data-ttu-id="43554-155">исекстерналливисибле</span><span class="sxs-lookup"><span data-stu-id="43554-155">isExternallyVisible</span></span>|<span data-ttu-id="43554-156">Логический</span><span class="sxs-lookup"><span data-stu-id="43554-156">Boolean</span></span>|<span data-ttu-id="43554-157">Указывает, могут ли пользователи за пресети клиента запрашивать пакеты доступа в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="43554-157">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="43554-158">модифиедби</span><span class="sxs-lookup"><span data-stu-id="43554-158">modifiedBy</span></span>|<span data-ttu-id="43554-159">String</span><span class="sxs-lookup"><span data-stu-id="43554-159">String</span></span>|<span data-ttu-id="43554-160">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="43554-160">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="43554-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43554-161">Read-only.</span></span>|
|<span data-ttu-id="43554-162">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43554-162">modifiedDateTime</span></span>|<span data-ttu-id="43554-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43554-163">DateTimeOffset</span></span>|<span data-ttu-id="43554-164">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="43554-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="43554-165">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="43554-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="43554-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43554-166">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="43554-167">Отношения</span><span class="sxs-lookup"><span data-stu-id="43554-167">Relationships</span></span>

| <span data-ttu-id="43554-168">Связь</span><span class="sxs-lookup"><span data-stu-id="43554-168">Relationship</span></span> | <span data-ttu-id="43554-169">Тип</span><span class="sxs-lookup"><span data-stu-id="43554-169">Type</span></span>        | <span data-ttu-id="43554-170">Описание</span><span class="sxs-lookup"><span data-stu-id="43554-170">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="43554-171">акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="43554-171">accessPackages</span></span>|<span data-ttu-id="43554-172">Коллекция [акцесспаккаже](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="43554-172">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="43554-173">Пакеты Access в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="43554-173">The access packages in this catalog.</span></span> <span data-ttu-id="43554-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="43554-174">Read-only.</span></span> <span data-ttu-id="43554-175">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="43554-175">Nullable.</span></span>|
|<span data-ttu-id="43554-176">акцесспаккажересаурцес</span><span class="sxs-lookup"><span data-stu-id="43554-176">accessPackageResources</span></span>|<span data-ttu-id="43554-177">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="43554-177">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="43554-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="43554-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43554-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43554-180">JSON representation</span></span>

<span data-ttu-id="43554-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43554-181">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "baseType": "",
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
