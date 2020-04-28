---
title: Тип ресурса Акцесспаккажересаурцерекуест
description: Запрос ресурса пакета Access — это запрос на Добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или нескольких пакетах доступа каталога.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74cc7815d4df22c1914f525ed0451b778c7777d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508522"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="3e7da-103">Тип ресурса Акцесспаккажересаурцерекуест</span><span class="sxs-lookup"><span data-stu-id="3e7da-103">accessPackageResourceRequest resource type</span></span>

<span data-ttu-id="3e7da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e7da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e7da-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)запрос ресурса пакета Access является запросом на Добавление ресурса к каталогу, чтобы роли ресурса можно было использовать в одном или нескольких пакетах доступа каталога.</span><span class="sxs-lookup"><span data-stu-id="3e7da-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="3e7da-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3e7da-106">Methods</span></span>

| <span data-ttu-id="3e7da-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3e7da-107">Method</span></span>       | <span data-ttu-id="3e7da-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3e7da-108">Return Type</span></span> | <span data-ttu-id="3e7da-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3e7da-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3e7da-110">Список Акцесспаккажересаурцерекуестс</span><span class="sxs-lookup"><span data-stu-id="3e7da-110">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="3e7da-111">Коллекция [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="3e7da-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="3e7da-112">Получение списка объектов **акцесспаккажересаурцерекуест** .</span><span class="sxs-lookup"><span data-stu-id="3e7da-112">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="3e7da-113">Создание Акцесспаккажересаурцерекуест</span><span class="sxs-lookup"><span data-stu-id="3e7da-113">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="3e7da-114">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="3e7da-114">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="3e7da-115">Создание нового объекта **акцесспаккажересаурцерекуест** .</span><span class="sxs-lookup"><span data-stu-id="3e7da-115">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3e7da-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e7da-116">Properties</span></span>

| <span data-ttu-id="3e7da-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e7da-117">Property</span></span>     | <span data-ttu-id="3e7da-118">Тип</span><span class="sxs-lookup"><span data-stu-id="3e7da-118">Type</span></span>        | <span data-ttu-id="3e7da-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3e7da-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e7da-120">каталогид</span><span class="sxs-lookup"><span data-stu-id="3e7da-120">catalogId</span></span>|<span data-ttu-id="3e7da-121">String</span><span class="sxs-lookup"><span data-stu-id="3e7da-121">String</span></span>|<span data-ttu-id="3e7da-122">Уникальный идентификатор каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="3e7da-122">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="3e7da-123">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3e7da-123">expirationDateTime</span></span>|<span data-ttu-id="3e7da-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e7da-124">DateTimeOffset</span></span>|<span data-ttu-id="3e7da-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3e7da-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e7da-127">id</span><span class="sxs-lookup"><span data-stu-id="3e7da-127">id</span></span>|<span data-ttu-id="3e7da-128">String</span><span class="sxs-lookup"><span data-stu-id="3e7da-128">String</span></span>| <span data-ttu-id="3e7da-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e7da-129">Read-only.</span></span>|
|<span data-ttu-id="3e7da-130">исвалидатиононли</span><span class="sxs-lookup"><span data-stu-id="3e7da-130">isValidationOnly</span></span>|<span data-ttu-id="3e7da-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e7da-131">Boolean</span></span>|<span data-ttu-id="3e7da-132">Если этот параметр установлен, ресурс не добавляется.</span><span class="sxs-lookup"><span data-stu-id="3e7da-132">If set, does not add the resource.</span></span>|
|<span data-ttu-id="3e7da-133">текста</span><span class="sxs-lookup"><span data-stu-id="3e7da-133">justification</span></span>|<span data-ttu-id="3e7da-134">String</span><span class="sxs-lookup"><span data-stu-id="3e7da-134">String</span></span>|<span data-ttu-id="3e7da-135">Обоснование запрашивающей стороны для добавления ресурса.</span><span class="sxs-lookup"><span data-stu-id="3e7da-135">The requestor's justification for adding the resource.</span></span>|
|<span data-ttu-id="3e7da-136">рекуестстате</span><span class="sxs-lookup"><span data-stu-id="3e7da-136">requestState</span></span>|<span data-ttu-id="3e7da-137">String</span><span class="sxs-lookup"><span data-stu-id="3e7da-137">String</span></span>| <span data-ttu-id="3e7da-138">Результат того, удалось ли службе добавить ресурс в каталог.</span><span class="sxs-lookup"><span data-stu-id="3e7da-138">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="3e7da-139">Значение, `Delivered` если ресурс был добавлен.</span><span class="sxs-lookup"><span data-stu-id="3e7da-139">The value is `Delivered` if the resource was added.</span></span> <span data-ttu-id="3e7da-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e7da-140">Read-Only.</span></span>|
|<span data-ttu-id="3e7da-141">рекуестстатус</span><span class="sxs-lookup"><span data-stu-id="3e7da-141">requestStatus</span></span>|<span data-ttu-id="3e7da-142">String</span><span class="sxs-lookup"><span data-stu-id="3e7da-142">String</span></span>|<span data-ttu-id="3e7da-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e7da-143">Read-only.</span></span>|
|<span data-ttu-id="3e7da-144">requestType</span><span class="sxs-lookup"><span data-stu-id="3e7da-144">requestType</span></span>|<span data-ttu-id="3e7da-145">String</span><span class="sxs-lookup"><span data-stu-id="3e7da-145">String</span></span>|<span data-ttu-id="3e7da-146">Используйте `AdminAdd` для добавления ресурса, если вызывающий абонент является администратором или владельцем ресурса.</span><span class="sxs-lookup"><span data-stu-id="3e7da-146">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3e7da-147">Связи</span><span class="sxs-lookup"><span data-stu-id="3e7da-147">Relationships</span></span>

| <span data-ttu-id="3e7da-148">Связь</span><span class="sxs-lookup"><span data-stu-id="3e7da-148">Relationship</span></span> | <span data-ttu-id="3e7da-149">Тип</span><span class="sxs-lookup"><span data-stu-id="3e7da-149">Type</span></span>        | <span data-ttu-id="3e7da-150">Описание</span><span class="sxs-lookup"><span data-stu-id="3e7da-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e7da-151">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="3e7da-151">accessPackageResource</span></span>|[<span data-ttu-id="3e7da-152">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="3e7da-152">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="3e7da-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3e7da-153">Nullable.</span></span>|
|<span data-ttu-id="3e7da-154">опросчика</span><span class="sxs-lookup"><span data-stu-id="3e7da-154">requestor</span></span>|[<span data-ttu-id="3e7da-155">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="3e7da-155">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="3e7da-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3e7da-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e7da-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e7da-158">JSON representation</span></span>

<span data-ttu-id="3e7da-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e7da-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "baseType": "",
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
