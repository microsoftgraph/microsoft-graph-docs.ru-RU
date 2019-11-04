---
title: Тип ресурса Акцесспаккажекаталог
description: Каталог пакетов Access — это контейнер для пакетов Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d95037bdf1e377f8981f99a06670957d838a2c92
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938935"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="a3a28-103">Тип ресурса Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="a3a28-103">accessPackageCatalog resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a28-104">В [управлении обслуживанием Azure AD](entitlementmanagement-root.md)каталог пакетов Access — это контейнер для одного или нескольких пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="a3a28-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="a3a28-105">Каталог пакетов Access также может иметь связанные ресурсы, которые используются в этих пакетах доступа для предоставления доступа.</span><span class="sxs-lookup"><span data-stu-id="a3a28-105">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="a3a28-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a3a28-106">Methods</span></span>

| <span data-ttu-id="a3a28-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a3a28-107">Method</span></span>       | <span data-ttu-id="a3a28-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3a28-108">Return Type</span></span> | <span data-ttu-id="a3a28-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a28-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a3a28-110">Список Акцесспаккажекаталогс</span><span class="sxs-lookup"><span data-stu-id="a3a28-110">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="a3a28-111">Коллекция [акцесспаккажекаталог](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="a3a28-111">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="a3a28-112">Получение списка объектов акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="a3a28-112">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="a3a28-113">Создание Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="a3a28-113">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="a3a28-114">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="a3a28-114">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="a3a28-115">Создание нового объекта Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="a3a28-115">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="a3a28-116">Получение Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="a3a28-116">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="a3a28-117">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="a3a28-117">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="a3a28-118">Чтение свойств и связей объекта Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="a3a28-118">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="a3a28-119">Удаление Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="a3a28-119">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="a3a28-120">Удаление Акцесспаккажекаталог.</span><span class="sxs-lookup"><span data-stu-id="a3a28-120">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="a3a28-121">Список ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="a3a28-121">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="a3a28-122">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="a3a28-122">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="a3a28-123">Получение списка объектов Акцесспаккажересаурце.</span><span class="sxs-lookup"><span data-stu-id="a3a28-123">Retrieve a list of accessPackageResource objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="a3a28-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3a28-124">Properties</span></span>

| <span data-ttu-id="a3a28-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3a28-125">Property</span></span>     | <span data-ttu-id="a3a28-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a3a28-126">Type</span></span>        | <span data-ttu-id="a3a28-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a28-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a3a28-128">каталогстатус</span><span class="sxs-lookup"><span data-stu-id="a3a28-128">catalogStatus</span></span>|<span data-ttu-id="a3a28-129">Строка</span><span class="sxs-lookup"><span data-stu-id="a3a28-129">String</span></span>|<span data-ttu-id="a3a28-130">Имеет значение `Published` , если пакеты доступа доступны для управления.</span><span class="sxs-lookup"><span data-stu-id="a3a28-130">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="a3a28-131">каталогтипе</span><span class="sxs-lookup"><span data-stu-id="a3a28-131">catalogType</span></span>|<span data-ttu-id="a3a28-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a3a28-132">String</span></span>|<span data-ttu-id="a3a28-133">Один из `UserManaged` или `ServiceDefault`.</span><span class="sxs-lookup"><span data-stu-id="a3a28-133">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="a3a28-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="a3a28-134">createdBy</span></span>|<span data-ttu-id="a3a28-135">Строка</span><span class="sxs-lookup"><span data-stu-id="a3a28-135">String</span></span>|<span data-ttu-id="a3a28-136">Имя участника-пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="a3a28-136">UPN of the user who created this resource.</span></span> <span data-ttu-id="a3a28-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3a28-137">Read-only.</span></span>|
|<span data-ttu-id="a3a28-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3a28-138">createdDateTime</span></span>|<span data-ttu-id="a3a28-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3a28-139">DateTimeOffset</span></span>|<span data-ttu-id="a3a28-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a3a28-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a3a28-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a3a28-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a3a28-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3a28-142">Read-only.</span></span>|
|<span data-ttu-id="a3a28-143">description</span><span class="sxs-lookup"><span data-stu-id="a3a28-143">description</span></span>|<span data-ttu-id="a3a28-144">String</span><span class="sxs-lookup"><span data-stu-id="a3a28-144">String</span></span>|<span data-ttu-id="a3a28-145">Описание каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="a3a28-145">The description of the access package catalog.</span></span>|
|<span data-ttu-id="a3a28-146">displayName</span><span class="sxs-lookup"><span data-stu-id="a3a28-146">displayName</span></span>|<span data-ttu-id="a3a28-147">Строка</span><span class="sxs-lookup"><span data-stu-id="a3a28-147">String</span></span>|<span data-ttu-id="a3a28-148">Отображаемое имя каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="a3a28-148">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="a3a28-149">id</span><span class="sxs-lookup"><span data-stu-id="a3a28-149">id</span></span>|<span data-ttu-id="a3a28-150">String</span><span class="sxs-lookup"><span data-stu-id="a3a28-150">String</span></span>| <span data-ttu-id="a3a28-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3a28-151">Read-only.</span></span>|
|<span data-ttu-id="a3a28-152">исекстерналливисибле</span><span class="sxs-lookup"><span data-stu-id="a3a28-152">isExternallyVisible</span></span>|<span data-ttu-id="a3a28-153">Логический</span><span class="sxs-lookup"><span data-stu-id="a3a28-153">Boolean</span></span>|<span data-ttu-id="a3a28-154">Указывает, могут ли пользователи за пресети клиента запрашивать пакеты доступа в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="a3a28-154">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="a3a28-155">модифиедби</span><span class="sxs-lookup"><span data-stu-id="a3a28-155">modifiedBy</span></span>|<span data-ttu-id="a3a28-156">Строка</span><span class="sxs-lookup"><span data-stu-id="a3a28-156">String</span></span>|<span data-ttu-id="a3a28-157">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="a3a28-157">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="a3a28-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3a28-158">Read-only.</span></span>|
|<span data-ttu-id="a3a28-159">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3a28-159">modifiedDateTime</span></span>|<span data-ttu-id="a3a28-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3a28-160">DateTimeOffset</span></span>|<span data-ttu-id="a3a28-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a3a28-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a3a28-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a3a28-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a3a28-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3a28-163">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="a3a28-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="a3a28-164">Relationships</span></span>

| <span data-ttu-id="a3a28-165">Связь</span><span class="sxs-lookup"><span data-stu-id="a3a28-165">Relationship</span></span> | <span data-ttu-id="a3a28-166">Тип</span><span class="sxs-lookup"><span data-stu-id="a3a28-166">Type</span></span>        | <span data-ttu-id="a3a28-167">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a28-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a3a28-168">акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="a3a28-168">accessPackages</span></span>|<span data-ttu-id="a3a28-169">Коллекция [акцесспаккаже](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="a3a28-169">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="a3a28-170">Пакеты Access в этом каталоге.</span><span class="sxs-lookup"><span data-stu-id="a3a28-170">The access packages in this catalog.</span></span> <span data-ttu-id="a3a28-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3a28-171">Read-only.</span></span> <span data-ttu-id="a3a28-172">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a3a28-172">Nullable.</span></span>|
|<span data-ttu-id="a3a28-173">акцесспаккажересаурцес</span><span class="sxs-lookup"><span data-stu-id="a3a28-173">accessPackageResources</span></span>|<span data-ttu-id="a3a28-174">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="a3a28-174">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="a3a28-p107">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a3a28-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3a28-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3a28-177">JSON representation</span></span>

<span data-ttu-id="a3a28-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3a28-178">The following is a JSON representation of the resource.</span></span>

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
