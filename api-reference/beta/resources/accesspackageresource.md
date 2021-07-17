---
title: тип ресурса accessPackageResource
description: Ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом ролей, которые можно использовать в одном или более пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 14bbbe23fca77f8fef06a2cb546cd0b1fdcc1949
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467115"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="2dc85-103">тип ресурса accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="2dc85-103">accessPackageResource resource type</span></span>

<span data-ttu-id="2dc85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dc85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dc85-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)ресурс пакета доступа является ссылкой на ресурс, связанный с каталогом пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="2dc85-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog.</span></span> <span data-ttu-id="2dc85-106">Роли для ресурса пакета доступа можно использовать в одном или более пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="2dc85-106">The roles for the access package resource can be used in one or more access packages.</span></span>  <span data-ttu-id="2dc85-107">Чтобы попросить связать ресурс с каталогом пакетов доступа или удалить его из каталога, создайте [accessPackageResourceRequest](accesspackageresourcerequest.md).</span><span class="sxs-lookup"><span data-stu-id="2dc85-107">To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2dc85-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2dc85-108">Methods</span></span>

| <span data-ttu-id="2dc85-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2dc85-109">Method</span></span>       | <span data-ttu-id="2dc85-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2dc85-110">Return Type</span></span> | <span data-ttu-id="2dc85-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc85-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2dc85-112">Ресурсы accessPackageCatalog списка</span><span class="sxs-lookup"><span data-stu-id="2dc85-112">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="2dc85-113">[коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="2dc85-113">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="2dc85-114">Извлечение списка объектов accessPackageResource в каталоге.</span><span class="sxs-lookup"><span data-stu-id="2dc85-114">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="2dc85-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dc85-115">Properties</span></span>

| <span data-ttu-id="2dc85-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dc85-116">Property</span></span>     | <span data-ttu-id="2dc85-117">Тип</span><span class="sxs-lookup"><span data-stu-id="2dc85-117">Type</span></span>        | <span data-ttu-id="2dc85-118">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc85-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2dc85-119">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="2dc85-119">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="2dc85-120">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="2dc85-120">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="2dc85-121">Содержит сведения об среде для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2dc85-121">Contains the environment information for the resource.</span></span> <span data-ttu-id="2dc85-122">Это можно установить с помощью `@odata.bind` аннотации или *originId среды.*</span><span class="sxs-lookup"><span data-stu-id="2dc85-122">This can be set using either the `@odata.bind` annotation or the environment's *originId*.</span></span>|
|<span data-ttu-id="2dc85-123">addedBy</span><span class="sxs-lookup"><span data-stu-id="2dc85-123">addedBy</span></span>|<span data-ttu-id="2dc85-124">String</span><span class="sxs-lookup"><span data-stu-id="2dc85-124">String</span></span>|<span data-ttu-id="2dc85-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2dc85-125">Read-only.</span></span>|
|<span data-ttu-id="2dc85-126">addedOn</span><span class="sxs-lookup"><span data-stu-id="2dc85-126">addedOn</span></span>|<span data-ttu-id="2dc85-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dc85-127">DateTimeOffset</span></span>|<span data-ttu-id="2dc85-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2dc85-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2dc85-129">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="2dc85-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2dc85-130">description</span><span class="sxs-lookup"><span data-stu-id="2dc85-130">description</span></span>|<span data-ttu-id="2dc85-131">String</span><span class="sxs-lookup"><span data-stu-id="2dc85-131">String</span></span>|<span data-ttu-id="2dc85-132">Описание ресурса.</span><span class="sxs-lookup"><span data-stu-id="2dc85-132">A description for the resource.</span></span>|
|<span data-ttu-id="2dc85-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2dc85-133">displayName</span></span>|<span data-ttu-id="2dc85-134">String</span><span class="sxs-lookup"><span data-stu-id="2dc85-134">String</span></span>|<span data-ttu-id="2dc85-135">Отображает имя ресурса, например имя приложения, имя группы или имя сайта.</span><span class="sxs-lookup"><span data-stu-id="2dc85-135">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="2dc85-136">id</span><span class="sxs-lookup"><span data-stu-id="2dc85-136">id</span></span>|<span data-ttu-id="2dc85-137">String</span><span class="sxs-lookup"><span data-stu-id="2dc85-137">String</span></span>| <span data-ttu-id="2dc85-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2dc85-138">Read-only.</span></span>|
|<span data-ttu-id="2dc85-139">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="2dc85-139">isPendingOnboarding</span></span>|<span data-ttu-id="2dc85-140">Логический</span><span class="sxs-lookup"><span data-stu-id="2dc85-140">Boolean</span></span>|<span data-ttu-id="2dc85-141">True, если ресурс еще не доступен для назначения.</span><span class="sxs-lookup"><span data-stu-id="2dc85-141">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="2dc85-142">OriginId</span><span class="sxs-lookup"><span data-stu-id="2dc85-142">originId</span></span>|<span data-ttu-id="2dc85-143">String</span><span class="sxs-lookup"><span data-stu-id="2dc85-143">String</span></span>|<span data-ttu-id="2dc85-144">Уникальный идентификатор ресурса в системе происхождения.</span><span class="sxs-lookup"><span data-stu-id="2dc85-144">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="2dc85-145">В случае группы Azure AD это идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="2dc85-145">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="2dc85-146">originSystem</span><span class="sxs-lookup"><span data-stu-id="2dc85-146">originSystem</span></span>|<span data-ttu-id="2dc85-147">String</span><span class="sxs-lookup"><span data-stu-id="2dc85-147">String</span></span>|<span data-ttu-id="2dc85-148">Тип ресурса в системе происхождения, например `SharePointOnline` , `AadApplication` или `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="2dc85-148">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="2dc85-149">resourceType</span><span class="sxs-lookup"><span data-stu-id="2dc85-149">resourceType</span></span>|<span data-ttu-id="2dc85-150">String</span><span class="sxs-lookup"><span data-stu-id="2dc85-150">String</span></span>|<span data-ttu-id="2dc85-151">Тип ресурса, например, подключенное приложение `Application` Azure AD или веб-SharePoint `SharePoint Online Site` Online.</span><span class="sxs-lookup"><span data-stu-id="2dc85-151">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="2dc85-152">url</span><span class="sxs-lookup"><span data-stu-id="2dc85-152">url</span></span>|<span data-ttu-id="2dc85-153">String</span><span class="sxs-lookup"><span data-stu-id="2dc85-153">String</span></span>|<span data-ttu-id="2dc85-154">Уникальный локатор ресурсов для ресурса, например URL-адрес для подписания пользователя в приложение.</span><span class="sxs-lookup"><span data-stu-id="2dc85-154">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dc85-155">Связи</span><span class="sxs-lookup"><span data-stu-id="2dc85-155">Relationships</span></span>

| <span data-ttu-id="2dc85-156">Связь</span><span class="sxs-lookup"><span data-stu-id="2dc85-156">Relationship</span></span> | <span data-ttu-id="2dc85-157">Тип</span><span class="sxs-lookup"><span data-stu-id="2dc85-157">Type</span></span>        | <span data-ttu-id="2dc85-158">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc85-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2dc85-159">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="2dc85-159">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="2dc85-160">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="2dc85-160">accessPackageResourceEnvironment</span></span>](accesspackageresourceenvironment.md)| <span data-ttu-id="2dc85-161">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2dc85-161">Nullable.</span></span> <span data-ttu-id="2dc85-162">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="2dc85-162">Supports `$expand`.</span></span>|
|<span data-ttu-id="2dc85-163">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="2dc85-163">accessPackageResourceRoles</span></span>|<span data-ttu-id="2dc85-164">[коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="2dc85-164">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="2dc85-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2dc85-165">Read-only.</span></span> <span data-ttu-id="2dc85-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2dc85-166">Nullable.</span></span> <span data-ttu-id="2dc85-167">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="2dc85-167">Supports `$expand`.</span></span>|
|<span data-ttu-id="2dc85-168">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="2dc85-168">accessPackageResourceScopes</span></span>|<span data-ttu-id="2dc85-169">[коллекция accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="2dc85-169">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="2dc85-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2dc85-170">Read-only.</span></span> <span data-ttu-id="2dc85-171">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2dc85-171">Nullable.</span></span> <span data-ttu-id="2dc85-172">Поддерживает `$expand`.</span><span class="sxs-lookup"><span data-stu-id="2dc85-172">Supports `$expand`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dc85-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2dc85-173">JSON representation</span></span>

<span data-ttu-id="2dc85-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dc85-174">The following is a JSON representation of the resource.</span></span>

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
