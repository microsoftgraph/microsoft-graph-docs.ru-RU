---
title: Тип ресурса Акцесспаккажекаталог
description: Каталог пакетов Access — это контейнер для пакетов Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 66b7939541ba57dafc3be852c82c89781fc82381
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508536"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="30731-103">Тип ресурса Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="30731-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="30731-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30731-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30731-105">В [управлении обслуживанием Azure AD](entitlementmanagement-root.md)каталог пакетов Access — это контейнер для одного или нескольких пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="30731-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="30731-106">Каталог пакетов Access также может иметь связанные ресурсы, которые используются в этих пакетах доступа для предоставления доступа.</span><span class="sxs-lookup"><span data-stu-id="30731-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="30731-107">Методы</span><span class="sxs-lookup"><span data-stu-id="30731-107">Methods</span></span>

| <span data-ttu-id="30731-108">Метод</span><span class="sxs-lookup"><span data-stu-id="30731-108">Method</span></span>       | <span data-ttu-id="30731-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="30731-109">Return Type</span></span> | <span data-ttu-id="30731-110">Описание</span><span class="sxs-lookup"><span data-stu-id="30731-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="30731-111">Список Акцесспаккажекаталогс</span><span class="sxs-lookup"><span data-stu-id="30731-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="30731-112">Коллекция [акцесспаккажекаталог](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="30731-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="30731-113">Получение списка объектов акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="30731-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="30731-114">Создание Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="30731-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="30731-115">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="30731-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="30731-116">Создание нового объекта Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="30731-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="30731-117">Получение Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="30731-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="30731-118">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="30731-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="30731-119">Чтение свойств и связей объекта Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="30731-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="30731-120">Удаление Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="30731-120">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="30731-121">Удаление Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="30731-121">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="30731-122">Список ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="30731-122">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="30731-123">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="30731-123">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="30731-124">Получение списка объектов Акцесспаккажересаурце в каталоге.</span><span class="sxs-lookup"><span data-stu-id="30731-124">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="30731-125">Список ролей ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="30731-125">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="30731-126">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="30731-126">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="30731-127">Получение списка объектов Акцесспаккажересаурцероле для ресурсов в каталоге.</span><span class="sxs-lookup"><span data-stu-id="30731-127">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="30731-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="30731-128">Properties</span></span>

| <span data-ttu-id="30731-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="30731-129">Property</span></span>     | <span data-ttu-id="30731-130">Тип</span><span class="sxs-lookup"><span data-stu-id="30731-130">Type</span></span>        | <span data-ttu-id="30731-131">Описание</span><span class="sxs-lookup"><span data-stu-id="30731-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="30731-132">каталогстатус</span><span class="sxs-lookup"><span data-stu-id="30731-132">catalogStatus</span></span>|<span data-ttu-id="30731-133">Строка</span><span class="sxs-lookup"><span data-stu-id="30731-133">String</span></span>|<span data-ttu-id="30731-134">Имеет значение, `Published` Если пакеты доступа доступны для управления.</span><span class="sxs-lookup"><span data-stu-id="30731-134">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="30731-135">каталогтипе</span><span class="sxs-lookup"><span data-stu-id="30731-135">catalogType</span></span>|<span data-ttu-id="30731-136">Строка</span><span class="sxs-lookup"><span data-stu-id="30731-136">String</span></span>|<span data-ttu-id="30731-137">Один из `UserManaged` или `ServiceDefault` .</span><span class="sxs-lookup"><span data-stu-id="30731-137">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="30731-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="30731-138">createdBy</span></span>|<span data-ttu-id="30731-139">Строка</span><span class="sxs-lookup"><span data-stu-id="30731-139">String</span></span>|<span data-ttu-id="30731-140">Имя участника-пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="30731-140">UPN of the user who created this resource.</span></span> <span data-ttu-id="30731-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30731-141">Read-only.</span></span>|
|<span data-ttu-id="30731-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30731-142">createdDateTime</span></span>|<span data-ttu-id="30731-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30731-143">DateTimeOffset</span></span>|<span data-ttu-id="30731-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="30731-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30731-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="30731-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="30731-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30731-146">Read-only.</span></span>|
|<span data-ttu-id="30731-147">description</span><span class="sxs-lookup"><span data-stu-id="30731-147">description</span></span>|<span data-ttu-id="30731-148">String</span><span class="sxs-lookup"><span data-stu-id="30731-148">String</span></span>|<span data-ttu-id="30731-149">Описание каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="30731-149">The description of the access package catalog.</span></span>|
|<span data-ttu-id="30731-150">displayName</span><span class="sxs-lookup"><span data-stu-id="30731-150">displayName</span></span>|<span data-ttu-id="30731-151">Строка</span><span class="sxs-lookup"><span data-stu-id="30731-151">String</span></span>|<span data-ttu-id="30731-152">Отображаемое имя каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="30731-152">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="30731-153">id</span><span class="sxs-lookup"><span data-stu-id="30731-153">id</span></span>|<span data-ttu-id="30731-154">String</span><span class="sxs-lookup"><span data-stu-id="30731-154">String</span></span>| <span data-ttu-id="30731-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30731-155">Read-only.</span></span>|
|<span data-ttu-id="30731-156">исекстерналливисибле</span><span class="sxs-lookup"><span data-stu-id="30731-156">isExternallyVisible</span></span>|<span data-ttu-id="30731-157">Логическое</span><span class="sxs-lookup"><span data-stu-id="30731-157">Boolean</span></span>|<span data-ttu-id="30731-158">Указывает, могут ли пользователи за пресети клиента запрашивать пакеты доступа в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="30731-158">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="30731-159">модифиедби</span><span class="sxs-lookup"><span data-stu-id="30731-159">modifiedBy</span></span>|<span data-ttu-id="30731-160">Строка</span><span class="sxs-lookup"><span data-stu-id="30731-160">String</span></span>|<span data-ttu-id="30731-161">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="30731-161">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="30731-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30731-162">Read-only.</span></span>|
|<span data-ttu-id="30731-163">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30731-163">modifiedDateTime</span></span>|<span data-ttu-id="30731-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30731-164">DateTimeOffset</span></span>|<span data-ttu-id="30731-165">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="30731-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30731-166">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="30731-166">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="30731-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30731-167">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="30731-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="30731-168">Relationships</span></span>

| <span data-ttu-id="30731-169">Связь</span><span class="sxs-lookup"><span data-stu-id="30731-169">Relationship</span></span> | <span data-ttu-id="30731-170">Тип</span><span class="sxs-lookup"><span data-stu-id="30731-170">Type</span></span>        | <span data-ttu-id="30731-171">Описание</span><span class="sxs-lookup"><span data-stu-id="30731-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="30731-172">акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="30731-172">accessPackages</span></span>|<span data-ttu-id="30731-173">Коллекция [акцесспаккаже](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="30731-173">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="30731-174">Пакеты Access в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="30731-174">The access packages in this catalog.</span></span> <span data-ttu-id="30731-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30731-175">Read-only.</span></span> <span data-ttu-id="30731-176">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="30731-176">Nullable.</span></span>|
|<span data-ttu-id="30731-177">акцесспаккажересаурцес</span><span class="sxs-lookup"><span data-stu-id="30731-177">accessPackageResources</span></span>|<span data-ttu-id="30731-178">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="30731-178">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="30731-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="30731-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30731-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30731-181">JSON representation</span></span>

<span data-ttu-id="30731-182">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30731-182">The following is a JSON representation of the resource.</span></span>

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
