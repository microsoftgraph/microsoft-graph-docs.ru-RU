---
title: Тип ресурса accessPackageResource
description: Ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом, роли которого можно использовать в одном или более пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2137d5452ddef86580504577614a042398a1b9ad
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158599"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="6471a-103">Тип ресурса accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="6471a-103">accessPackageResource resource type</span></span>

<span data-ttu-id="6471a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6471a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6471a-105">В [azure AD Entitlement Management](entitlementmanagement-root.md)ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="6471a-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog.</span></span> <span data-ttu-id="6471a-106">Роли для ресурса пакета доступа можно использовать в одном или более пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="6471a-106">The roles for the access package resource can be used in one or more access packages.</span></span>  <span data-ttu-id="6471a-107">Чтобы запросить связывание ресурса с каталогом пакетов доступа или удалить ресурс из каталога, создайте [accessPackageResourceRequest.](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="6471a-107">To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6471a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6471a-108">Methods</span></span>

| <span data-ttu-id="6471a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6471a-109">Method</span></span>       | <span data-ttu-id="6471a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6471a-110">Return Type</span></span> | <span data-ttu-id="6471a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6471a-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6471a-112">Список ресурсов accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="6471a-112">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="6471a-113">[Коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="6471a-113">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="6471a-114">Получить список объектов accessPackageResource в каталоге.</span><span class="sxs-lookup"><span data-stu-id="6471a-114">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="6471a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="6471a-115">Properties</span></span>

| <span data-ttu-id="6471a-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="6471a-116">Property</span></span>     | <span data-ttu-id="6471a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="6471a-117">Type</span></span>        | <span data-ttu-id="6471a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="6471a-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6471a-119">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="6471a-119">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="6471a-120">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="6471a-120">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="6471a-121">Содержит сведения о среде для ресурса.</span><span class="sxs-lookup"><span data-stu-id="6471a-121">Contains the environment information for the resource.</span></span> <span data-ttu-id="6471a-122">Это можно сделать с помощью `@odata.bind` аннотации или источника *среды.*</span><span class="sxs-lookup"><span data-stu-id="6471a-122">This can be set using either the `@odata.bind` annotation or the environment's *originId*.</span></span>|
|<span data-ttu-id="6471a-123">addedBy</span><span class="sxs-lookup"><span data-stu-id="6471a-123">addedBy</span></span>|<span data-ttu-id="6471a-124">String</span><span class="sxs-lookup"><span data-stu-id="6471a-124">String</span></span>|<span data-ttu-id="6471a-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6471a-125">Read-only.</span></span>|
|<span data-ttu-id="6471a-126">addedOn</span><span class="sxs-lookup"><span data-stu-id="6471a-126">addedOn</span></span>|<span data-ttu-id="6471a-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6471a-127">DateTimeOffset</span></span>|<span data-ttu-id="6471a-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6471a-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6471a-130">description</span><span class="sxs-lookup"><span data-stu-id="6471a-130">description</span></span>|<span data-ttu-id="6471a-131">String</span><span class="sxs-lookup"><span data-stu-id="6471a-131">String</span></span>|<span data-ttu-id="6471a-132">Описание ресурса.</span><span class="sxs-lookup"><span data-stu-id="6471a-132">A description for the resource.</span></span>|
|<span data-ttu-id="6471a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6471a-133">displayName</span></span>|<span data-ttu-id="6471a-134">String</span><span class="sxs-lookup"><span data-stu-id="6471a-134">String</span></span>|<span data-ttu-id="6471a-135">Отображаемого имени ресурса, например имя приложения, имя группы или имя сайта.</span><span class="sxs-lookup"><span data-stu-id="6471a-135">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="6471a-136">id</span><span class="sxs-lookup"><span data-stu-id="6471a-136">id</span></span>|<span data-ttu-id="6471a-137">String</span><span class="sxs-lookup"><span data-stu-id="6471a-137">String</span></span>| <span data-ttu-id="6471a-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6471a-138">Read-only.</span></span>|
|<span data-ttu-id="6471a-139">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="6471a-139">isPendingOnboarding</span></span>|<span data-ttu-id="6471a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="6471a-140">Boolean</span></span>|<span data-ttu-id="6471a-141">Имеет true, если ресурс еще не доступен для назначения.</span><span class="sxs-lookup"><span data-stu-id="6471a-141">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="6471a-142">originId</span><span class="sxs-lookup"><span data-stu-id="6471a-142">originId</span></span>|<span data-ttu-id="6471a-143">String</span><span class="sxs-lookup"><span data-stu-id="6471a-143">String</span></span>|<span data-ttu-id="6471a-144">Уникальный идентификатор ресурса в системе источника.</span><span class="sxs-lookup"><span data-stu-id="6471a-144">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="6471a-145">В случае группы Azure AD это идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="6471a-145">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="6471a-146">originSystem</span><span class="sxs-lookup"><span data-stu-id="6471a-146">originSystem</span></span>|<span data-ttu-id="6471a-147">String</span><span class="sxs-lookup"><span data-stu-id="6471a-147">String</span></span>|<span data-ttu-id="6471a-148">Тип ресурса в системе источника, например `SharePointOnline` , или `AadApplication` `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="6471a-148">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="6471a-149">resourceType</span><span class="sxs-lookup"><span data-stu-id="6471a-149">resourceType</span></span>|<span data-ttu-id="6471a-150">String</span><span class="sxs-lookup"><span data-stu-id="6471a-150">String</span></span>|<span data-ttu-id="6471a-151">Тип ресурса, например, подключенное к Azure AD приложение `Application` или сайт `SharePoint Online Site` SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="6471a-151">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="6471a-152">url</span><span class="sxs-lookup"><span data-stu-id="6471a-152">url</span></span>|<span data-ttu-id="6471a-153">String</span><span class="sxs-lookup"><span data-stu-id="6471a-153">String</span></span>|<span data-ttu-id="6471a-154">Уникальный локатор ресурса, например URL-адрес для регистрации пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="6471a-154">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6471a-155">Связи</span><span class="sxs-lookup"><span data-stu-id="6471a-155">Relationships</span></span>

| <span data-ttu-id="6471a-156">Связь</span><span class="sxs-lookup"><span data-stu-id="6471a-156">Relationship</span></span> | <span data-ttu-id="6471a-157">Тип</span><span class="sxs-lookup"><span data-stu-id="6471a-157">Type</span></span>        | <span data-ttu-id="6471a-158">Описание</span><span class="sxs-lookup"><span data-stu-id="6471a-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6471a-159">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="6471a-159">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="6471a-160">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="6471a-160">accessPackageResourceEnvironment</span></span>](accesspackageresourceenvironment.md)| <span data-ttu-id="6471a-161">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6471a-161">Nullable.</span></span>|
|<span data-ttu-id="6471a-162">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="6471a-162">accessPackageResourceRoles</span></span>|<span data-ttu-id="6471a-163">[Коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="6471a-163">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="6471a-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6471a-164">Read-only.</span></span> <span data-ttu-id="6471a-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6471a-165">Nullable.</span></span>|
|<span data-ttu-id="6471a-166">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="6471a-166">accessPackageResourceScopes</span></span>|<span data-ttu-id="6471a-167">[Коллекция accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="6471a-167">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="6471a-p106">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6471a-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6471a-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6471a-170">JSON representation</span></span>

<span data-ttu-id="6471a-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6471a-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
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
