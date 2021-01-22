---
title: Тип ресурса accessPackageResource
description: Ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом, роли которого можно использовать в одном или более пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e34b850b19836eeb19cc63232c7af822512bfee4
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934830"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="327aa-103">Тип ресурса accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="327aa-103">accessPackageResource resource type</span></span>

<span data-ttu-id="327aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="327aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="327aa-105">В управлении правами [Azure AD](entitlementmanagement-root.md)ресурс пакета доступа — это ссылка на ресурс, связанный с каталогом пакетов доступа, роли для которого можно использовать в одном или более пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="327aa-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog, the roles for which can be used in one or more access packages.</span></span>  <span data-ttu-id="327aa-106">Чтобы запросить связывание ресурса с каталогом пакетов доступа или удалить ресурс из каталога, создайте [accessPackageResourceRequest.](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="327aa-106">To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="327aa-107">Методы</span><span class="sxs-lookup"><span data-stu-id="327aa-107">Methods</span></span>

| <span data-ttu-id="327aa-108">Метод</span><span class="sxs-lookup"><span data-stu-id="327aa-108">Method</span></span>       | <span data-ttu-id="327aa-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="327aa-109">Return Type</span></span> | <span data-ttu-id="327aa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="327aa-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="327aa-111">Список ресурсов accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="327aa-111">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="327aa-112">[Коллекция accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="327aa-112">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="327aa-113">Получить список объектов accessPackageResource в каталоге.</span><span class="sxs-lookup"><span data-stu-id="327aa-113">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="327aa-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="327aa-114">Properties</span></span>

| <span data-ttu-id="327aa-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="327aa-115">Property</span></span>     | <span data-ttu-id="327aa-116">Тип</span><span class="sxs-lookup"><span data-stu-id="327aa-116">Type</span></span>        | <span data-ttu-id="327aa-117">Описание</span><span class="sxs-lookup"><span data-stu-id="327aa-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="327aa-118">addedBy</span><span class="sxs-lookup"><span data-stu-id="327aa-118">addedBy</span></span>|<span data-ttu-id="327aa-119">String</span><span class="sxs-lookup"><span data-stu-id="327aa-119">String</span></span>|<span data-ttu-id="327aa-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="327aa-120">Read-only.</span></span>|
|<span data-ttu-id="327aa-121">addedOn</span><span class="sxs-lookup"><span data-stu-id="327aa-121">addedOn</span></span>|<span data-ttu-id="327aa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="327aa-122">DateTimeOffset</span></span>|<span data-ttu-id="327aa-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="327aa-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="327aa-125">description</span><span class="sxs-lookup"><span data-stu-id="327aa-125">description</span></span>|<span data-ttu-id="327aa-126">String</span><span class="sxs-lookup"><span data-stu-id="327aa-126">String</span></span>|<span data-ttu-id="327aa-127">Описание ресурса.</span><span class="sxs-lookup"><span data-stu-id="327aa-127">A description for the resource.</span></span>|
|<span data-ttu-id="327aa-128">displayName</span><span class="sxs-lookup"><span data-stu-id="327aa-128">displayName</span></span>|<span data-ttu-id="327aa-129">String</span><span class="sxs-lookup"><span data-stu-id="327aa-129">String</span></span>|<span data-ttu-id="327aa-130">Отображаемого имени ресурса, например имя приложения, имя группы или имя сайта.</span><span class="sxs-lookup"><span data-stu-id="327aa-130">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="327aa-131">id</span><span class="sxs-lookup"><span data-stu-id="327aa-131">id</span></span>|<span data-ttu-id="327aa-132">String</span><span class="sxs-lookup"><span data-stu-id="327aa-132">String</span></span>| <span data-ttu-id="327aa-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="327aa-133">Read-only.</span></span>|
|<span data-ttu-id="327aa-134">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="327aa-134">isPendingOnboarding</span></span>|<span data-ttu-id="327aa-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="327aa-135">Boolean</span></span>|<span data-ttu-id="327aa-136">Имеет true, если ресурс еще не доступен для назначения.</span><span class="sxs-lookup"><span data-stu-id="327aa-136">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="327aa-137">originId</span><span class="sxs-lookup"><span data-stu-id="327aa-137">originId</span></span>|<span data-ttu-id="327aa-138">String</span><span class="sxs-lookup"><span data-stu-id="327aa-138">String</span></span>|<span data-ttu-id="327aa-139">Уникальный идентификатор ресурса в системе источника.</span><span class="sxs-lookup"><span data-stu-id="327aa-139">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="327aa-140">В случае группы Azure AD это идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="327aa-140">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="327aa-141">originSystem</span><span class="sxs-lookup"><span data-stu-id="327aa-141">originSystem</span></span>|<span data-ttu-id="327aa-142">String</span><span class="sxs-lookup"><span data-stu-id="327aa-142">String</span></span>|<span data-ttu-id="327aa-143">Тип ресурса в системе источника, например `SharePointOnline` , или `AadApplication` `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="327aa-143">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="327aa-144">resourceType</span><span class="sxs-lookup"><span data-stu-id="327aa-144">resourceType</span></span>|<span data-ttu-id="327aa-145">String</span><span class="sxs-lookup"><span data-stu-id="327aa-145">String</span></span>|<span data-ttu-id="327aa-146">Тип ресурса, например, подключенное к Azure AD приложение `Application` или сайт `SharePoint Online Site` SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="327aa-146">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="327aa-147">url</span><span class="sxs-lookup"><span data-stu-id="327aa-147">url</span></span>|<span data-ttu-id="327aa-148">String</span><span class="sxs-lookup"><span data-stu-id="327aa-148">String</span></span>|<span data-ttu-id="327aa-149">Уникальный локатор ресурса, например URL-адрес для регистрации пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="327aa-149">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="327aa-150">Связи</span><span class="sxs-lookup"><span data-stu-id="327aa-150">Relationships</span></span>

| <span data-ttu-id="327aa-151">Связь</span><span class="sxs-lookup"><span data-stu-id="327aa-151">Relationship</span></span> | <span data-ttu-id="327aa-152">Тип</span><span class="sxs-lookup"><span data-stu-id="327aa-152">Type</span></span>        | <span data-ttu-id="327aa-153">Описание</span><span class="sxs-lookup"><span data-stu-id="327aa-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="327aa-154">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="327aa-154">accessPackageResourceRoles</span></span>|<span data-ttu-id="327aa-155">[Коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="327aa-155">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="327aa-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="327aa-156">Read-only.</span></span> <span data-ttu-id="327aa-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="327aa-157">Nullable.</span></span>|
|<span data-ttu-id="327aa-158">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="327aa-158">accessPackageResourceScopes</span></span>|<span data-ttu-id="327aa-159">[Коллекция accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="327aa-159">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="327aa-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="327aa-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="327aa-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="327aa-162">JSON representation</span></span>

<span data-ttu-id="327aa-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="327aa-163">The following is a JSON representation of the resource.</span></span>

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


