---
title: Тип ресурса Акцесспаккажересаурцерекуест
description: Запрос ресурса пакета Access — это запрос на Добавление ресурса в каталог, чтобы роли ресурса можно было использовать в одном или нескольких пакетах доступа каталога.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c109c2c28a9c4c9248adfbad4c94c9c50268f28f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871938"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="ada31-103">Тип ресурса Акцесспаккажересаурцерекуест</span><span class="sxs-lookup"><span data-stu-id="ada31-103">accessPackageResourceRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ada31-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)запрос ресурса пакета Access является запросом на Добавление ресурса к каталогу, чтобы роли ресурса можно было использовать в одном или нескольких пакетах доступа каталога.</span><span class="sxs-lookup"><span data-stu-id="ada31-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="ada31-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ada31-105">Methods</span></span>

| <span data-ttu-id="ada31-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ada31-106">Method</span></span>       | <span data-ttu-id="ada31-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ada31-107">Return Type</span></span> | <span data-ttu-id="ada31-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ada31-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ada31-109">Список Акцесспаккажересаурцерекуестс</span><span class="sxs-lookup"><span data-stu-id="ada31-109">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="ada31-110">Коллекция [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ada31-110">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="ada31-111">Получение списка объектов **акцесспаккажересаурцерекуест** .</span><span class="sxs-lookup"><span data-stu-id="ada31-111">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="ada31-112">Создание Акцесспаккажересаурцерекуест</span><span class="sxs-lookup"><span data-stu-id="ada31-112">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="ada31-113">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="ada31-113">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="ada31-114">Создание нового объекта **акцесспаккажересаурцерекуест** .</span><span class="sxs-lookup"><span data-stu-id="ada31-114">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ada31-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="ada31-115">Properties</span></span>

| <span data-ttu-id="ada31-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="ada31-116">Property</span></span>     | <span data-ttu-id="ada31-117">Тип</span><span class="sxs-lookup"><span data-stu-id="ada31-117">Type</span></span>        | <span data-ttu-id="ada31-118">Описание</span><span class="sxs-lookup"><span data-stu-id="ada31-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ada31-119">каталогид</span><span class="sxs-lookup"><span data-stu-id="ada31-119">catalogId</span></span>|<span data-ttu-id="ada31-120">String</span><span class="sxs-lookup"><span data-stu-id="ada31-120">String</span></span>|<span data-ttu-id="ada31-121">Уникальный идентификатор каталога пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="ada31-121">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="ada31-122">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ada31-122">expirationDateTime</span></span>|<span data-ttu-id="ada31-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ada31-123">DateTimeOffset</span></span>|<span data-ttu-id="ada31-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ada31-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ada31-126">id</span><span class="sxs-lookup"><span data-stu-id="ada31-126">id</span></span>|<span data-ttu-id="ada31-127">String</span><span class="sxs-lookup"><span data-stu-id="ada31-127">String</span></span>| <span data-ttu-id="ada31-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ada31-128">Read-only.</span></span>|
|<span data-ttu-id="ada31-129">исвалидатиононли</span><span class="sxs-lookup"><span data-stu-id="ada31-129">isValidationOnly</span></span>|<span data-ttu-id="ada31-130">Логический</span><span class="sxs-lookup"><span data-stu-id="ada31-130">Boolean</span></span>|<span data-ttu-id="ada31-131">Если этот параметр установлен, ресурс не добавляется.</span><span class="sxs-lookup"><span data-stu-id="ada31-131">If set, does not add the resource.</span></span>|
|<span data-ttu-id="ada31-132">текста</span><span class="sxs-lookup"><span data-stu-id="ada31-132">justification</span></span>|<span data-ttu-id="ada31-133">String</span><span class="sxs-lookup"><span data-stu-id="ada31-133">String</span></span>|<span data-ttu-id="ada31-134">Обоснование запрашивающей стороны для добавления ресурса.</span><span class="sxs-lookup"><span data-stu-id="ada31-134">The requestor's justification for adding the resource.</span></span>|
|<span data-ttu-id="ada31-135">рекуестстате</span><span class="sxs-lookup"><span data-stu-id="ada31-135">requestState</span></span>|<span data-ttu-id="ada31-136">String</span><span class="sxs-lookup"><span data-stu-id="ada31-136">String</span></span>| <span data-ttu-id="ada31-137">Результат того, удалось ли службе добавить ресурс в каталог.</span><span class="sxs-lookup"><span data-stu-id="ada31-137">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="ada31-138">Значение, `Delivered` если ресурс был добавлен.</span><span class="sxs-lookup"><span data-stu-id="ada31-138">The value is `Delivered` if the resource was added.</span></span> <span data-ttu-id="ada31-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ada31-139">Read-Only.</span></span>|
|<span data-ttu-id="ada31-140">рекуестстатус</span><span class="sxs-lookup"><span data-stu-id="ada31-140">requestStatus</span></span>|<span data-ttu-id="ada31-141">String</span><span class="sxs-lookup"><span data-stu-id="ada31-141">String</span></span>|<span data-ttu-id="ada31-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ada31-142">Read-only.</span></span>|
|<span data-ttu-id="ada31-143">requestType</span><span class="sxs-lookup"><span data-stu-id="ada31-143">requestType</span></span>|<span data-ttu-id="ada31-144">String</span><span class="sxs-lookup"><span data-stu-id="ada31-144">String</span></span>|<span data-ttu-id="ada31-145">Используйте `AdminAdd` для добавления ресурса, если вызывающий абонент является администратором или владельцем ресурса.</span><span class="sxs-lookup"><span data-stu-id="ada31-145">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ada31-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="ada31-146">Relationships</span></span>

| <span data-ttu-id="ada31-147">Связь</span><span class="sxs-lookup"><span data-stu-id="ada31-147">Relationship</span></span> | <span data-ttu-id="ada31-148">Тип</span><span class="sxs-lookup"><span data-stu-id="ada31-148">Type</span></span>        | <span data-ttu-id="ada31-149">Описание</span><span class="sxs-lookup"><span data-stu-id="ada31-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ada31-150">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="ada31-150">accessPackageResource</span></span>|[<span data-ttu-id="ada31-151">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="ada31-151">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="ada31-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ada31-152">Nullable.</span></span>|
|<span data-ttu-id="ada31-153">опросчика</span><span class="sxs-lookup"><span data-stu-id="ada31-153">requestor</span></span>|[<span data-ttu-id="ada31-154">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="ada31-154">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="ada31-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ada31-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ada31-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ada31-157">JSON representation</span></span>

<span data-ttu-id="ada31-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ada31-158">The following is a JSON representation of the resource.</span></span>

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
