---
title: Тип ресурса Акцесспаккажересаурце
description: Ресурс пакета Access — это ссылка на ресурс, связанный с каталогом, в котором находятся роли, которые можно использовать в одном или нескольких пакетах доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e964a8ce2e9bd4165a29037a56ec4f95fe969422
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938928"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="5ac6c-103">Тип ресурса Акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="5ac6c-103">accessPackageResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ac6c-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)ресурс пакета Access — это ссылка на ресурс, связанный с каталогом, роли, для которых можно использовать один или несколько пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with a catalog the roles for which can be used in one or more access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="5ac6c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5ac6c-105">Methods</span></span>

| <span data-ttu-id="5ac6c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5ac6c-106">Method</span></span>       | <span data-ttu-id="5ac6c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5ac6c-107">Return Type</span></span> | <span data-ttu-id="5ac6c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5ac6c-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5ac6c-109">Список ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="5ac6c-109">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="5ac6c-110">Коллекция [акцесспаккажересаурце](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="5ac6c-110">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="5ac6c-111">Получение списка объектов акцесспаккажересаурце.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-111">Retrieve a list of accesspackageresource objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="5ac6c-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ac6c-112">Properties</span></span>

| <span data-ttu-id="5ac6c-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ac6c-113">Property</span></span>     | <span data-ttu-id="5ac6c-114">Тип</span><span class="sxs-lookup"><span data-stu-id="5ac6c-114">Type</span></span>        | <span data-ttu-id="5ac6c-115">Описание</span><span class="sxs-lookup"><span data-stu-id="5ac6c-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5ac6c-116">аддедби</span><span class="sxs-lookup"><span data-stu-id="5ac6c-116">addedBy</span></span>|<span data-ttu-id="5ac6c-117">String</span><span class="sxs-lookup"><span data-stu-id="5ac6c-117">String</span></span>|<span data-ttu-id="5ac6c-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-118">Read-only.</span></span>|
|<span data-ttu-id="5ac6c-119">аддедон</span><span class="sxs-lookup"><span data-stu-id="5ac6c-119">addedOn</span></span>|<span data-ttu-id="5ac6c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ac6c-120">DateTimeOffset</span></span>|<span data-ttu-id="5ac6c-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5ac6c-123">description</span><span class="sxs-lookup"><span data-stu-id="5ac6c-123">description</span></span>|<span data-ttu-id="5ac6c-124">String</span><span class="sxs-lookup"><span data-stu-id="5ac6c-124">String</span></span>|<span data-ttu-id="5ac6c-125">Описание ресурса.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-125">A description for the resource.</span></span>|
|<span data-ttu-id="5ac6c-126">displayName</span><span class="sxs-lookup"><span data-stu-id="5ac6c-126">displayName</span></span>|<span data-ttu-id="5ac6c-127">Строка</span><span class="sxs-lookup"><span data-stu-id="5ac6c-127">String</span></span>|<span data-ttu-id="5ac6c-128">Отображаемое имя ресурса, например имя приложения, имя группы или имя сайта.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-128">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="5ac6c-129">id</span><span class="sxs-lookup"><span data-stu-id="5ac6c-129">id</span></span>|<span data-ttu-id="5ac6c-130">String</span><span class="sxs-lookup"><span data-stu-id="5ac6c-130">String</span></span>| <span data-ttu-id="5ac6c-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-131">Read-only.</span></span>|
|<span data-ttu-id="5ac6c-132">испендингонбоардинг</span><span class="sxs-lookup"><span data-stu-id="5ac6c-132">isPendingOnboarding</span></span>|<span data-ttu-id="5ac6c-133">Логический</span><span class="sxs-lookup"><span data-stu-id="5ac6c-133">Boolean</span></span>|<span data-ttu-id="5ac6c-134">Значение true, если ресурс пока недоступен для назначения.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-134">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="5ac6c-135">оригинид</span><span class="sxs-lookup"><span data-stu-id="5ac6c-135">originId</span></span>|<span data-ttu-id="5ac6c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="5ac6c-136">String</span></span>|<span data-ttu-id="5ac6c-137">Уникальный идентификатор ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-137">The unique identifier of the resource in the origin system.</span></span> |
|<span data-ttu-id="5ac6c-138">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="5ac6c-138">originSystem</span></span>|<span data-ttu-id="5ac6c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="5ac6c-139">String</span></span>|<span data-ttu-id="5ac6c-140">Тип ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-140">The type of the resource in the origin system.</span></span>|
|<span data-ttu-id="5ac6c-141">Ресурса</span><span class="sxs-lookup"><span data-stu-id="5ac6c-141">resourceType</span></span>|<span data-ttu-id="5ac6c-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5ac6c-142">String</span></span>|<span data-ttu-id="5ac6c-143">Тип ресурса, например, `Application` если это приложение, подключенное к Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-143">The type of the resource, such as `Application` if it is an Azure AD connected application.</span></span>|
|<span data-ttu-id="5ac6c-144">url</span><span class="sxs-lookup"><span data-stu-id="5ac6c-144">url</span></span>|<span data-ttu-id="5ac6c-145">String</span><span class="sxs-lookup"><span data-stu-id="5ac6c-145">String</span></span>|<span data-ttu-id="5ac6c-146">Уникальный указатель ресурсов для ресурса, например URL-адрес для подписания пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-146">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ac6c-147">Связи</span><span class="sxs-lookup"><span data-stu-id="5ac6c-147">Relationships</span></span>

| <span data-ttu-id="5ac6c-148">Связь</span><span class="sxs-lookup"><span data-stu-id="5ac6c-148">Relationship</span></span> | <span data-ttu-id="5ac6c-149">Тип</span><span class="sxs-lookup"><span data-stu-id="5ac6c-149">Type</span></span>        | <span data-ttu-id="5ac6c-150">Описание</span><span class="sxs-lookup"><span data-stu-id="5ac6c-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5ac6c-151">акцесспаккажересаурцеролес</span><span class="sxs-lookup"><span data-stu-id="5ac6c-151">accessPackageResourceRoles</span></span>|<span data-ttu-id="5ac6c-152">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="5ac6c-152">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="5ac6c-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-153">Read-only.</span></span> <span data-ttu-id="5ac6c-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-154">Nullable.</span></span>|
|<span data-ttu-id="5ac6c-155">акцесспаккажересаурцескопес</span><span class="sxs-lookup"><span data-stu-id="5ac6c-155">accessPackageResourceScopes</span></span>|<span data-ttu-id="5ac6c-156">Коллекция [акцесспаккажересаурцескопе](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="5ac6c-156">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="5ac6c-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ac6c-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ac6c-159">JSON representation</span></span>

<span data-ttu-id="5ac6c-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ac6c-160">The following is a JSON representation of the resource.</span></span>

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
