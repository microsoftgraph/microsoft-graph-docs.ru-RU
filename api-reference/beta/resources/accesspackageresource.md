---
title: Тип ресурса accessPackageResource
description: Ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом, роли которого можно использовать в одном или более пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 31499fda1d2d12f1e9868da6cf9e09fde38298cd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137475"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="46c70-103">Тип ресурса accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="46c70-103">accessPackageResource resource type</span></span>

<span data-ttu-id="46c70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46c70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46c70-105">В [azure AD Entitlement Management](entitlementmanagement-root.md)ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="46c70-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog.</span></span> <span data-ttu-id="46c70-106">Роли для ресурса пакета доступа можно использовать в одном или более пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="46c70-106">The roles for the access package resource can be used in one or more access packages.</span></span>  <span data-ttu-id="46c70-107">Чтобы запросить связывание ресурса с каталогом пакетов доступа или удалить ресурс из каталога, создайте [accessPackageResourceRequest.](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="46c70-107">To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="46c70-108">Методы</span><span class="sxs-lookup"><span data-stu-id="46c70-108">Methods</span></span>

| <span data-ttu-id="46c70-109">Метод</span><span class="sxs-lookup"><span data-stu-id="46c70-109">Method</span></span>       | <span data-ttu-id="46c70-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="46c70-110">Return Type</span></span> | <span data-ttu-id="46c70-111">Описание</span><span class="sxs-lookup"><span data-stu-id="46c70-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="46c70-112">Список ресурсов accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="46c70-112">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="46c70-113">[Коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="46c70-113">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="46c70-114">Получить список объектов accessPackageResource в каталоге.</span><span class="sxs-lookup"><span data-stu-id="46c70-114">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="46c70-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="46c70-115">Properties</span></span>

| <span data-ttu-id="46c70-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="46c70-116">Property</span></span>     | <span data-ttu-id="46c70-117">Тип</span><span class="sxs-lookup"><span data-stu-id="46c70-117">Type</span></span>        | <span data-ttu-id="46c70-118">Описание</span><span class="sxs-lookup"><span data-stu-id="46c70-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46c70-119">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="46c70-119">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="46c70-120">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="46c70-120">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="46c70-121">Содержит сведения о среде для ресурса.</span><span class="sxs-lookup"><span data-stu-id="46c70-121">Contains the environment information for the resource.</span></span> <span data-ttu-id="46c70-122">Это можно настроить с помощью `@odata.bind` аннотации или источника *среды.*</span><span class="sxs-lookup"><span data-stu-id="46c70-122">This can be set using either the `@odata.bind` annotation or the environment's *originId*.</span></span>|
|<span data-ttu-id="46c70-123">addedBy</span><span class="sxs-lookup"><span data-stu-id="46c70-123">addedBy</span></span>|<span data-ttu-id="46c70-124">String</span><span class="sxs-lookup"><span data-stu-id="46c70-124">String</span></span>|<span data-ttu-id="46c70-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46c70-125">Read-only.</span></span>|
|<span data-ttu-id="46c70-126">addedOn</span><span class="sxs-lookup"><span data-stu-id="46c70-126">addedOn</span></span>|<span data-ttu-id="46c70-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46c70-127">DateTimeOffset</span></span>|<span data-ttu-id="46c70-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="46c70-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="46c70-130">description</span><span class="sxs-lookup"><span data-stu-id="46c70-130">description</span></span>|<span data-ttu-id="46c70-131">Строка</span><span class="sxs-lookup"><span data-stu-id="46c70-131">String</span></span>|<span data-ttu-id="46c70-132">Описание ресурса.</span><span class="sxs-lookup"><span data-stu-id="46c70-132">A description for the resource.</span></span>|
|<span data-ttu-id="46c70-133">displayName</span><span class="sxs-lookup"><span data-stu-id="46c70-133">displayName</span></span>|<span data-ttu-id="46c70-134">Строка</span><span class="sxs-lookup"><span data-stu-id="46c70-134">String</span></span>|<span data-ttu-id="46c70-135">Отображаемого имени ресурса, например имя приложения, имя группы или имя сайта.</span><span class="sxs-lookup"><span data-stu-id="46c70-135">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="46c70-136">id</span><span class="sxs-lookup"><span data-stu-id="46c70-136">id</span></span>|<span data-ttu-id="46c70-137">String</span><span class="sxs-lookup"><span data-stu-id="46c70-137">String</span></span>| <span data-ttu-id="46c70-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46c70-138">Read-only.</span></span>|
|<span data-ttu-id="46c70-139">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="46c70-139">isPendingOnboarding</span></span>|<span data-ttu-id="46c70-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="46c70-140">Boolean</span></span>|<span data-ttu-id="46c70-141">Имеет true, если ресурс еще не доступен для назначения.</span><span class="sxs-lookup"><span data-stu-id="46c70-141">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="46c70-142">originId</span><span class="sxs-lookup"><span data-stu-id="46c70-142">originId</span></span>|<span data-ttu-id="46c70-143">Строка</span><span class="sxs-lookup"><span data-stu-id="46c70-143">String</span></span>|<span data-ttu-id="46c70-144">Уникальный идентификатор ресурса в системе источника.</span><span class="sxs-lookup"><span data-stu-id="46c70-144">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="46c70-145">В случае группы Azure AD это идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="46c70-145">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="46c70-146">originSystem</span><span class="sxs-lookup"><span data-stu-id="46c70-146">originSystem</span></span>|<span data-ttu-id="46c70-147">Строка</span><span class="sxs-lookup"><span data-stu-id="46c70-147">String</span></span>|<span data-ttu-id="46c70-148">Тип ресурса в системе источника, например `SharePointOnline` , или `AadApplication` `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="46c70-148">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="46c70-149">resourceType</span><span class="sxs-lookup"><span data-stu-id="46c70-149">resourceType</span></span>|<span data-ttu-id="46c70-150">Строка</span><span class="sxs-lookup"><span data-stu-id="46c70-150">String</span></span>|<span data-ttu-id="46c70-151">Тип ресурса, например, подключенное к Azure AD приложение `Application` или сайт `SharePoint Online Site` SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="46c70-151">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="46c70-152">url</span><span class="sxs-lookup"><span data-stu-id="46c70-152">url</span></span>|<span data-ttu-id="46c70-153">String</span><span class="sxs-lookup"><span data-stu-id="46c70-153">String</span></span>|<span data-ttu-id="46c70-154">Уникальный локатор ресурса, например URL-адрес для регистрации пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="46c70-154">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46c70-155">Связи</span><span class="sxs-lookup"><span data-stu-id="46c70-155">Relationships</span></span>

| <span data-ttu-id="46c70-156">Связь</span><span class="sxs-lookup"><span data-stu-id="46c70-156">Relationship</span></span> | <span data-ttu-id="46c70-157">Тип</span><span class="sxs-lookup"><span data-stu-id="46c70-157">Type</span></span>        | <span data-ttu-id="46c70-158">Описание</span><span class="sxs-lookup"><span data-stu-id="46c70-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46c70-159">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="46c70-159">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="46c70-160">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="46c70-160">accessPackageResourceEnvironment</span></span>](accesspackageresourceenvironment.md)| <span data-ttu-id="46c70-161">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="46c70-161">Nullable.</span></span>|
|<span data-ttu-id="46c70-162">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="46c70-162">accessPackageResourceRoles</span></span>|<span data-ttu-id="46c70-163">[Коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="46c70-163">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="46c70-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46c70-164">Read-only.</span></span> <span data-ttu-id="46c70-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="46c70-165">Nullable.</span></span>|
|<span data-ttu-id="46c70-166">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="46c70-166">accessPackageResourceScopes</span></span>|<span data-ttu-id="46c70-167">[Коллекция accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="46c70-167">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="46c70-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="46c70-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46c70-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46c70-170">JSON representation</span></span>

<span data-ttu-id="46c70-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46c70-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isPendingOnboarding": true,
  "originId": "String",
  "originSystem": "String",
  "resourceType": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
