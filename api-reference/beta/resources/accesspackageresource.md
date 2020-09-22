---
title: Тип ресурса Акцесспаккажересаурце
description: Ресурс пакета Access — это ссылка на ресурс, связанный с каталогом, в котором находятся роли, которые можно использовать в одном или нескольких пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6c37ff0de7f733b67eda0541418ca4b42aa57352
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089835"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="cb67a-103">Тип ресурса Акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="cb67a-103">accessPackageResource resource type</span></span>

<span data-ttu-id="cb67a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb67a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb67a-105">В разделе [Управление обслуживанием Azure AD](entitlementmanagement-root.md)ресурс пакета Access — это ссылка на ресурс, связанный с каталогом пакетов Access, роли, которые можно использовать в одном или нескольких пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="cb67a-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog, the roles for which can be used in one or more access packages.</span></span>  <span data-ttu-id="cb67a-106">Чтобы запросить сопоставление ресурса с каталогом пакетов Access, создайте [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md).</span><span class="sxs-lookup"><span data-stu-id="cb67a-106">To request to associate a resource with an access package catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cb67a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="cb67a-107">Methods</span></span>

| <span data-ttu-id="cb67a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="cb67a-108">Method</span></span>       | <span data-ttu-id="cb67a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cb67a-109">Return Type</span></span> | <span data-ttu-id="cb67a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cb67a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cb67a-111">Список ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="cb67a-111">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="cb67a-112">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="cb67a-112">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="cb67a-113">Получение списка объектов Акцесспаккажересаурце в каталоге.</span><span class="sxs-lookup"><span data-stu-id="cb67a-113">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb67a-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb67a-114">Properties</span></span>

| <span data-ttu-id="cb67a-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb67a-115">Property</span></span>     | <span data-ttu-id="cb67a-116">Тип</span><span class="sxs-lookup"><span data-stu-id="cb67a-116">Type</span></span>        | <span data-ttu-id="cb67a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="cb67a-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb67a-118">аддедби</span><span class="sxs-lookup"><span data-stu-id="cb67a-118">addedBy</span></span>|<span data-ttu-id="cb67a-119">String</span><span class="sxs-lookup"><span data-stu-id="cb67a-119">String</span></span>|<span data-ttu-id="cb67a-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb67a-120">Read-only.</span></span>|
|<span data-ttu-id="cb67a-121">аддедон</span><span class="sxs-lookup"><span data-stu-id="cb67a-121">addedOn</span></span>|<span data-ttu-id="cb67a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb67a-122">DateTimeOffset</span></span>|<span data-ttu-id="cb67a-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cb67a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cb67a-125">description</span><span class="sxs-lookup"><span data-stu-id="cb67a-125">description</span></span>|<span data-ttu-id="cb67a-126">Строка</span><span class="sxs-lookup"><span data-stu-id="cb67a-126">String</span></span>|<span data-ttu-id="cb67a-127">Описание ресурса.</span><span class="sxs-lookup"><span data-stu-id="cb67a-127">A description for the resource.</span></span>|
|<span data-ttu-id="cb67a-128">displayName</span><span class="sxs-lookup"><span data-stu-id="cb67a-128">displayName</span></span>|<span data-ttu-id="cb67a-129">Строка</span><span class="sxs-lookup"><span data-stu-id="cb67a-129">String</span></span>|<span data-ttu-id="cb67a-130">Отображаемое имя ресурса, например имя приложения, имя группы или имя сайта.</span><span class="sxs-lookup"><span data-stu-id="cb67a-130">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="cb67a-131">id</span><span class="sxs-lookup"><span data-stu-id="cb67a-131">id</span></span>|<span data-ttu-id="cb67a-132">String</span><span class="sxs-lookup"><span data-stu-id="cb67a-132">String</span></span>| <span data-ttu-id="cb67a-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb67a-133">Read-only.</span></span>|
|<span data-ttu-id="cb67a-134">испендингонбоардинг</span><span class="sxs-lookup"><span data-stu-id="cb67a-134">isPendingOnboarding</span></span>|<span data-ttu-id="cb67a-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb67a-135">Boolean</span></span>|<span data-ttu-id="cb67a-136">Значение true, если ресурс пока недоступен для назначения.</span><span class="sxs-lookup"><span data-stu-id="cb67a-136">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="cb67a-137">оригинид</span><span class="sxs-lookup"><span data-stu-id="cb67a-137">originId</span></span>|<span data-ttu-id="cb67a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="cb67a-138">String</span></span>|<span data-ttu-id="cb67a-139">Уникальный идентификатор ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="cb67a-139">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="cb67a-140">В случае группы Azure AD это идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="cb67a-140">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="cb67a-141">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="cb67a-141">originSystem</span></span>|<span data-ttu-id="cb67a-142">Строка</span><span class="sxs-lookup"><span data-stu-id="cb67a-142">String</span></span>|<span data-ttu-id="cb67a-143">Тип ресурса в исходной системе, например `SharePointOnline` , `AadApplication` или `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="cb67a-143">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="cb67a-144">Ресурса</span><span class="sxs-lookup"><span data-stu-id="cb67a-144">resourceType</span></span>|<span data-ttu-id="cb67a-145">Строка</span><span class="sxs-lookup"><span data-stu-id="cb67a-145">String</span></span>|<span data-ttu-id="cb67a-146">Тип ресурса, например, `Application` если это приложение, подключаемое к Azure AD, или `SharePoint Online Site` сайт SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="cb67a-146">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="cb67a-147">url</span><span class="sxs-lookup"><span data-stu-id="cb67a-147">url</span></span>|<span data-ttu-id="cb67a-148">String</span><span class="sxs-lookup"><span data-stu-id="cb67a-148">String</span></span>|<span data-ttu-id="cb67a-149">Уникальный указатель ресурсов для ресурса, например URL-адрес для подписания пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="cb67a-149">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb67a-150">Связи</span><span class="sxs-lookup"><span data-stu-id="cb67a-150">Relationships</span></span>

| <span data-ttu-id="cb67a-151">Связь</span><span class="sxs-lookup"><span data-stu-id="cb67a-151">Relationship</span></span> | <span data-ttu-id="cb67a-152">Тип</span><span class="sxs-lookup"><span data-stu-id="cb67a-152">Type</span></span>        | <span data-ttu-id="cb67a-153">Описание</span><span class="sxs-lookup"><span data-stu-id="cb67a-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb67a-154">акцесспаккажересаурцеролес</span><span class="sxs-lookup"><span data-stu-id="cb67a-154">accessPackageResourceRoles</span></span>|<span data-ttu-id="cb67a-155">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="cb67a-155">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="cb67a-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb67a-156">Read-only.</span></span> <span data-ttu-id="cb67a-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="cb67a-157">Nullable.</span></span>|
|<span data-ttu-id="cb67a-158">акцесспаккажересаурцескопес</span><span class="sxs-lookup"><span data-stu-id="cb67a-158">accessPackageResourceScopes</span></span>|<span data-ttu-id="cb67a-159">Коллекция [акцесспаккажересаурцескопе](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="cb67a-159">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="cb67a-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="cb67a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb67a-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb67a-162">JSON representation</span></span>

<span data-ttu-id="cb67a-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb67a-163">The following is a JSON representation of the resource.</span></span>

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


