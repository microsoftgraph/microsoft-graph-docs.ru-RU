---
title: Тип ресурса Акцесспаккажересаурце
description: Ресурс пакета Access — это ссылка на ресурс, связанный с каталогом, в котором находятся роли, которые можно использовать в одном или нескольких пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0567ca9347b560b14ae96da4914a8801f9183019
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870976"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="3d3ab-103">Тип ресурса Акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="3d3ab-103">accessPackageResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d3ab-104">В разделе [Управление обслуживанием Azure AD](entitlementmanagement-root.md)ресурс пакета Access — это ссылка на ресурс, связанный с каталогом пакетов Access, роли, которые можно использовать в одном или нескольких пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog, the roles for which can be used in one or more access packages.</span></span>  <span data-ttu-id="3d3ab-105">Чтобы запросить сопоставление ресурса с каталогом пакетов Access, создайте [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md).</span><span class="sxs-lookup"><span data-stu-id="3d3ab-105">To request to associate a resource with an access package catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3d3ab-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3d3ab-106">Methods</span></span>

| <span data-ttu-id="3d3ab-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3d3ab-107">Method</span></span>       | <span data-ttu-id="3d3ab-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3d3ab-108">Return Type</span></span> | <span data-ttu-id="3d3ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3ab-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3d3ab-110">Список ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="3d3ab-110">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="3d3ab-111">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="3d3ab-111">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="3d3ab-112">Получение списка объектов Акцесспаккажересаурце в каталоге.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-112">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="3d3ab-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d3ab-113">Properties</span></span>

| <span data-ttu-id="3d3ab-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d3ab-114">Property</span></span>     | <span data-ttu-id="3d3ab-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3d3ab-115">Type</span></span>        | <span data-ttu-id="3d3ab-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3ab-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d3ab-117">аддедби</span><span class="sxs-lookup"><span data-stu-id="3d3ab-117">addedBy</span></span>|<span data-ttu-id="3d3ab-118">String</span><span class="sxs-lookup"><span data-stu-id="3d3ab-118">String</span></span>|<span data-ttu-id="3d3ab-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-119">Read-only.</span></span>|
|<span data-ttu-id="3d3ab-120">аддедон</span><span class="sxs-lookup"><span data-stu-id="3d3ab-120">addedOn</span></span>|<span data-ttu-id="3d3ab-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d3ab-121">DateTimeOffset</span></span>|<span data-ttu-id="3d3ab-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3d3ab-124">description</span><span class="sxs-lookup"><span data-stu-id="3d3ab-124">description</span></span>|<span data-ttu-id="3d3ab-125">String</span><span class="sxs-lookup"><span data-stu-id="3d3ab-125">String</span></span>|<span data-ttu-id="3d3ab-126">Описание ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-126">A description for the resource.</span></span>|
|<span data-ttu-id="3d3ab-127">displayName</span><span class="sxs-lookup"><span data-stu-id="3d3ab-127">displayName</span></span>|<span data-ttu-id="3d3ab-128">Строка</span><span class="sxs-lookup"><span data-stu-id="3d3ab-128">String</span></span>|<span data-ttu-id="3d3ab-129">Отображаемое имя ресурса, например имя приложения, имя группы или имя сайта.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-129">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="3d3ab-130">id</span><span class="sxs-lookup"><span data-stu-id="3d3ab-130">id</span></span>|<span data-ttu-id="3d3ab-131">String</span><span class="sxs-lookup"><span data-stu-id="3d3ab-131">String</span></span>| <span data-ttu-id="3d3ab-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-132">Read-only.</span></span>|
|<span data-ttu-id="3d3ab-133">испендингонбоардинг</span><span class="sxs-lookup"><span data-stu-id="3d3ab-133">isPendingOnboarding</span></span>|<span data-ttu-id="3d3ab-134">Логический</span><span class="sxs-lookup"><span data-stu-id="3d3ab-134">Boolean</span></span>|<span data-ttu-id="3d3ab-135">Значение true, если ресурс пока недоступен для назначения.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-135">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="3d3ab-136">оригинид</span><span class="sxs-lookup"><span data-stu-id="3d3ab-136">originId</span></span>|<span data-ttu-id="3d3ab-137">String</span><span class="sxs-lookup"><span data-stu-id="3d3ab-137">String</span></span>|<span data-ttu-id="3d3ab-138">Уникальный идентификатор ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-138">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="3d3ab-139">В случае группы Azure AD это идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-139">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="3d3ab-140">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="3d3ab-140">originSystem</span></span>|<span data-ttu-id="3d3ab-141">String</span><span class="sxs-lookup"><span data-stu-id="3d3ab-141">String</span></span>|<span data-ttu-id="3d3ab-142">Тип ресурса в исходной системе, например `SharePointOnline` или. `AadGroup`</span><span class="sxs-lookup"><span data-stu-id="3d3ab-142">The type of the resource in the origin system, such as `SharePointOnline` or `AadGroup`.</span></span>|
|<span data-ttu-id="3d3ab-143">Ресурса</span><span class="sxs-lookup"><span data-stu-id="3d3ab-143">resourceType</span></span>|<span data-ttu-id="3d3ab-144">String</span><span class="sxs-lookup"><span data-stu-id="3d3ab-144">String</span></span>|<span data-ttu-id="3d3ab-145">Тип ресурса, например, `Application` если это приложение, подключаемое к Azure AD, или `SharePoint Online Site` сайт SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-145">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="3d3ab-146">url</span><span class="sxs-lookup"><span data-stu-id="3d3ab-146">url</span></span>|<span data-ttu-id="3d3ab-147">String</span><span class="sxs-lookup"><span data-stu-id="3d3ab-147">String</span></span>|<span data-ttu-id="3d3ab-148">Уникальный указатель ресурсов для ресурса, например URL-адрес для подписания пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-148">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d3ab-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="3d3ab-149">Relationships</span></span>

| <span data-ttu-id="3d3ab-150">Связь</span><span class="sxs-lookup"><span data-stu-id="3d3ab-150">Relationship</span></span> | <span data-ttu-id="3d3ab-151">Тип</span><span class="sxs-lookup"><span data-stu-id="3d3ab-151">Type</span></span>        | <span data-ttu-id="3d3ab-152">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3ab-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d3ab-153">акцесспаккажересаурцеролес</span><span class="sxs-lookup"><span data-stu-id="3d3ab-153">accessPackageResourceRoles</span></span>|<span data-ttu-id="3d3ab-154">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="3d3ab-154">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="3d3ab-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-155">Read-only.</span></span> <span data-ttu-id="3d3ab-156">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-156">Nullable.</span></span>|
|<span data-ttu-id="3d3ab-157">акцесспаккажересаурцескопес</span><span class="sxs-lookup"><span data-stu-id="3d3ab-157">accessPackageResourceScopes</span></span>|<span data-ttu-id="3d3ab-158">Коллекция [акцесспаккажересаурцескопе](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="3d3ab-158">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="3d3ab-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d3ab-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d3ab-161">JSON representation</span></span>

<span data-ttu-id="3d3ab-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d3ab-162">The following is a JSON representation of the resource.</span></span>

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
