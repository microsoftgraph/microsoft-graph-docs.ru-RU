---
title: тип ресурса accessPackageResourceRequest
description: Запрос ресурса пакета доступа — это запрос на добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или более пакетах доступа каталога.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ea0d6ae14d93fbc691af4713cf40452a890d1891
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722190"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="0bd3e-103">тип ресурса accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="0bd3e-103">accessPackageResourceRequest resource type</span></span>

<span data-ttu-id="0bd3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bd3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bd3e-105">В управлении правами [Azure AD](entitlementmanagement-root.md)запрос ресурсов пакета доступа — это запрос на добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или несколько пакетах доступа каталога или удалить ресурс из каталога, который больше не требуется пакетам доступа.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages, or to remove a resource from a catalog that is no longer needed by the access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="0bd3e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0bd3e-106">Methods</span></span>

| <span data-ttu-id="0bd3e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0bd3e-107">Method</span></span>       | <span data-ttu-id="0bd3e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0bd3e-108">Return Type</span></span> | <span data-ttu-id="0bd3e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0bd3e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0bd3e-110">Список accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="0bd3e-110">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="0bd3e-111">[коллекция accessPackageResourceRequest](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="0bd3e-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="0bd3e-112">Извлечение списка **объектов accessPackageResourceRequest.**</span><span class="sxs-lookup"><span data-stu-id="0bd3e-112">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="0bd3e-113">Создание accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="0bd3e-113">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="0bd3e-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0bd3e-114">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="0bd3e-115">Создание нового **объекта accessPackageResourceRequest.**</span><span class="sxs-lookup"><span data-stu-id="0bd3e-115">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0bd3e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bd3e-116">Properties</span></span>

| <span data-ttu-id="0bd3e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bd3e-117">Property</span></span>     | <span data-ttu-id="0bd3e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="0bd3e-118">Type</span></span>        | <span data-ttu-id="0bd3e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0bd3e-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0bd3e-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="0bd3e-120">catalogId</span></span>|<span data-ttu-id="0bd3e-121">String</span><span class="sxs-lookup"><span data-stu-id="0bd3e-121">String</span></span>|<span data-ttu-id="0bd3e-122">Уникальный ID каталога пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-122">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="0bd3e-123">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0bd3e-123">expirationDateTime</span></span>|<span data-ttu-id="0bd3e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bd3e-124">DateTimeOffset</span></span>|<span data-ttu-id="0bd3e-125">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0bd3e-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0bd3e-126">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-126">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="0bd3e-127">id</span><span class="sxs-lookup"><span data-stu-id="0bd3e-127">id</span></span>|<span data-ttu-id="0bd3e-128">String</span><span class="sxs-lookup"><span data-stu-id="0bd3e-128">String</span></span>| <span data-ttu-id="0bd3e-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-129">Read-only.</span></span>|
|<span data-ttu-id="0bd3e-130">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="0bd3e-130">isValidationOnly</span></span>|<span data-ttu-id="0bd3e-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bd3e-131">Boolean</span></span>|<span data-ttu-id="0bd3e-132">Если установлено, ресурс не добавляется.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-132">If set, does not add the resource.</span></span>|
|<span data-ttu-id="0bd3e-133">обоснование</span><span class="sxs-lookup"><span data-stu-id="0bd3e-133">justification</span></span>|<span data-ttu-id="0bd3e-134">String</span><span class="sxs-lookup"><span data-stu-id="0bd3e-134">String</span></span>|<span data-ttu-id="0bd3e-135">Обоснование запроса для добавления или удаления ресурса.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-135">The requestor's justification for adding or removing the resource.</span></span>|
|<span data-ttu-id="0bd3e-136">requestState</span><span class="sxs-lookup"><span data-stu-id="0bd3e-136">requestState</span></span>|<span data-ttu-id="0bd3e-137">String</span><span class="sxs-lookup"><span data-stu-id="0bd3e-137">String</span></span>| <span data-ttu-id="0bd3e-138">Результат того, удалось ли службе добавить ресурс в каталог.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-138">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="0bd3e-139">Значение, если `Delivered` ресурс был добавлен или удален.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-139">The value is `Delivered` if the resource was added or removed.</span></span> <span data-ttu-id="0bd3e-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-140">Read-Only.</span></span>|
|<span data-ttu-id="0bd3e-141">requestStatus</span><span class="sxs-lookup"><span data-stu-id="0bd3e-141">requestStatus</span></span>|<span data-ttu-id="0bd3e-142">String</span><span class="sxs-lookup"><span data-stu-id="0bd3e-142">String</span></span>|<span data-ttu-id="0bd3e-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-143">Read-only.</span></span>|
|<span data-ttu-id="0bd3e-144">requestType</span><span class="sxs-lookup"><span data-stu-id="0bd3e-144">requestType</span></span>|<span data-ttu-id="0bd3e-145">String</span><span class="sxs-lookup"><span data-stu-id="0bd3e-145">String</span></span>|<span data-ttu-id="0bd3e-146">Используйте для добавления ресурса, если вызываемая является администратором или владельцем ресурса, или `AdminAdd` `AdminRemove` для удаления ресурса.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-146">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner, or `AdminRemove` to remove a resource.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0bd3e-147">Связи</span><span class="sxs-lookup"><span data-stu-id="0bd3e-147">Relationships</span></span>

| <span data-ttu-id="0bd3e-148">Связь</span><span class="sxs-lookup"><span data-stu-id="0bd3e-148">Relationship</span></span> | <span data-ttu-id="0bd3e-149">Тип</span><span class="sxs-lookup"><span data-stu-id="0bd3e-149">Type</span></span>        | <span data-ttu-id="0bd3e-150">Описание</span><span class="sxs-lookup"><span data-stu-id="0bd3e-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0bd3e-151">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="0bd3e-151">accessPackageResource</span></span>|[<span data-ttu-id="0bd3e-152">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="0bd3e-152">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="0bd3e-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-153">Nullable.</span></span>|
|<span data-ttu-id="0bd3e-154">запросчик</span><span class="sxs-lookup"><span data-stu-id="0bd3e-154">requestor</span></span>|[<span data-ttu-id="0bd3e-155">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="0bd3e-155">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="0bd3e-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bd3e-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bd3e-158">JSON representation</span></span>

<span data-ttu-id="0bd3e-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bd3e-159">The following is a JSON representation of the resource.</span></span>

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


