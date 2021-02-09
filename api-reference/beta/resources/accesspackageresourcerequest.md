---
title: Тип ресурса accessPackageResourceRequest
description: Запрос на доступ к пакету доступа — это запрос на добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или более пакетах доступа каталога.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 16198df73c51b1b5f7cb7f8c7748da4816800890
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158585"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="524a9-103">Тип ресурса accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="524a9-103">accessPackageResourceRequest resource type</span></span>

<span data-ttu-id="524a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="524a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="524a9-105">В управлении правами [Azure AD](entitlementmanagement-root.md)запрос на доступ к пакету доступа — это запрос на добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или более пакетах доступа каталога, или удалить ресурс из каталога, который больше не нужен пакетам доступа.</span><span class="sxs-lookup"><span data-stu-id="524a9-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages, or to remove a resource from a catalog that is no longer needed by the access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="524a9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="524a9-106">Methods</span></span>

| <span data-ttu-id="524a9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="524a9-107">Method</span></span>       | <span data-ttu-id="524a9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="524a9-108">Return Type</span></span> | <span data-ttu-id="524a9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="524a9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="524a9-110">Список accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="524a9-110">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="524a9-111">[Коллекция accessPackageResourceRequest](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="524a9-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="524a9-112">Получить список объектов **accessPackageResourceRequest.**</span><span class="sxs-lookup"><span data-stu-id="524a9-112">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="524a9-113">Создание accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="524a9-113">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="524a9-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="524a9-114">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="524a9-115">Создание объекта **accessPackageResourceRequest.**</span><span class="sxs-lookup"><span data-stu-id="524a9-115">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="524a9-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="524a9-116">Properties</span></span>

| <span data-ttu-id="524a9-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="524a9-117">Property</span></span>     | <span data-ttu-id="524a9-118">Тип</span><span class="sxs-lookup"><span data-stu-id="524a9-118">Type</span></span>        | <span data-ttu-id="524a9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="524a9-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="524a9-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="524a9-120">catalogId</span></span>|<span data-ttu-id="524a9-121">String</span><span class="sxs-lookup"><span data-stu-id="524a9-121">String</span></span>|<span data-ttu-id="524a9-122">Уникальный ИД каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="524a9-122">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="524a9-123">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="524a9-123">expirationDateTime</span></span>|<span data-ttu-id="524a9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="524a9-124">DateTimeOffset</span></span>|<span data-ttu-id="524a9-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="524a9-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="524a9-127">id</span><span class="sxs-lookup"><span data-stu-id="524a9-127">id</span></span>|<span data-ttu-id="524a9-128">String</span><span class="sxs-lookup"><span data-stu-id="524a9-128">String</span></span>| <span data-ttu-id="524a9-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="524a9-129">Read-only.</span></span>|
|<span data-ttu-id="524a9-130">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="524a9-130">isValidationOnly</span></span>|<span data-ttu-id="524a9-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="524a9-131">Boolean</span></span>|<span data-ttu-id="524a9-132">Если этот набор за установлен, ресурс не добавляется.</span><span class="sxs-lookup"><span data-stu-id="524a9-132">If set, does not add the resource.</span></span>|
|<span data-ttu-id="524a9-133">обоснование</span><span class="sxs-lookup"><span data-stu-id="524a9-133">justification</span></span>|<span data-ttu-id="524a9-134">String</span><span class="sxs-lookup"><span data-stu-id="524a9-134">String</span></span>|<span data-ttu-id="524a9-135">Обоснование запросителя для добавления или удаления ресурса.</span><span class="sxs-lookup"><span data-stu-id="524a9-135">The requestor's justification for adding or removing the resource.</span></span>|
|<span data-ttu-id="524a9-136">requestState</span><span class="sxs-lookup"><span data-stu-id="524a9-136">requestState</span></span>|<span data-ttu-id="524a9-137">String</span><span class="sxs-lookup"><span data-stu-id="524a9-137">String</span></span>| <span data-ttu-id="524a9-138">Результат того, удалось ли службе добавить ресурс в каталог.</span><span class="sxs-lookup"><span data-stu-id="524a9-138">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="524a9-139">Значением является `Delivered` то, был ли добавлен или удален ресурс.</span><span class="sxs-lookup"><span data-stu-id="524a9-139">The value is `Delivered` if the resource was added or removed.</span></span> <span data-ttu-id="524a9-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="524a9-140">Read-Only.</span></span>|
|<span data-ttu-id="524a9-141">requestStatus</span><span class="sxs-lookup"><span data-stu-id="524a9-141">requestStatus</span></span>|<span data-ttu-id="524a9-142">String</span><span class="sxs-lookup"><span data-stu-id="524a9-142">String</span></span>|<span data-ttu-id="524a9-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="524a9-143">Read-only.</span></span>|
|<span data-ttu-id="524a9-144">requestType</span><span class="sxs-lookup"><span data-stu-id="524a9-144">requestType</span></span>|<span data-ttu-id="524a9-145">String</span><span class="sxs-lookup"><span data-stu-id="524a9-145">String</span></span>|<span data-ttu-id="524a9-146">Используется для добавления ресурса, если вызываемая является администратором или владельцем ресурса, или `AdminAdd` `AdminRemove` для удаления ресурса.</span><span class="sxs-lookup"><span data-stu-id="524a9-146">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner, or `AdminRemove` to remove a resource.</span></span> |

## <a name="relationships"></a><span data-ttu-id="524a9-147">Связи</span><span class="sxs-lookup"><span data-stu-id="524a9-147">Relationships</span></span>

| <span data-ttu-id="524a9-148">Связь</span><span class="sxs-lookup"><span data-stu-id="524a9-148">Relationship</span></span> | <span data-ttu-id="524a9-149">Тип</span><span class="sxs-lookup"><span data-stu-id="524a9-149">Type</span></span>        | <span data-ttu-id="524a9-150">Описание</span><span class="sxs-lookup"><span data-stu-id="524a9-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="524a9-151">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="524a9-151">accessPackageResource</span></span>|[<span data-ttu-id="524a9-152">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="524a9-152">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="524a9-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="524a9-153">Nullable.</span></span>|
|<span data-ttu-id="524a9-154">requestor</span><span class="sxs-lookup"><span data-stu-id="524a9-154">requestor</span></span>|[<span data-ttu-id="524a9-155">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="524a9-155">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="524a9-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="524a9-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="524a9-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="524a9-158">JSON representation</span></span>

<span data-ttu-id="524a9-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="524a9-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "keyProperty": "id"
}-->

```json
{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "expirationDateTime": "String (timestamp)",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "String",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


