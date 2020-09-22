---
title: Обновление екстерналитем
description: Обновление свойств объекта екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 411d64b5ec6afdd5f994c64faceb4e5fc9a2c637
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192212"
---
# <a name="update-externalitem"></a><span data-ttu-id="8d0d4-103">Обновление екстерналитем</span><span class="sxs-lookup"><span data-stu-id="8d0d4-103">Update externalitem</span></span>

<span data-ttu-id="8d0d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d0d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d0d4-105">Обновление свойств объекта [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d4-105">Update the properties of an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="8d0d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d0d4-106">Permissions</span></span>

<span data-ttu-id="8d0d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d0d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d0d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d0d4-109">Permission type</span></span>                        | <span data-ttu-id="8d0d4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d0d4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d0d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d0d4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d0d4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-112">Not supported.</span></span> |
| <span data-ttu-id="8d0d4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d0d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d0d4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-114">Not supported.</span></span> |
| <span data-ttu-id="8d0d4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d0d4-115">Application</span></span>                            | <span data-ttu-id="8d0d4-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d0d4-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d0d4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d0d4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="8d0d4-118">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="8d0d4-118">Path parameters</span></span>

| <span data-ttu-id="8d0d4-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="8d0d4-119">Parameter</span></span>     | <span data-ttu-id="8d0d4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8d0d4-120">Type</span></span>   | <span data-ttu-id="8d0d4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8d0d4-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="8d0d4-122">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="8d0d4-122">connection-id</span></span> | <span data-ttu-id="8d0d4-123">string</span><span class="sxs-lookup"><span data-stu-id="8d0d4-123">string</span></span> | <span data-ttu-id="8d0d4-124">`id`Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="8d0d4-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="8d0d4-125">item-id</span><span class="sxs-lookup"><span data-stu-id="8d0d4-125">item-id</span></span>       | <span data-ttu-id="8d0d4-126">string</span><span class="sxs-lookup"><span data-stu-id="8d0d4-126">string</span></span> | <span data-ttu-id="8d0d4-127">Предоставляемое разработчиком `id` свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d4-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8d0d4-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d0d4-128">Request headers</span></span>

| <span data-ttu-id="8d0d4-129">Имя</span><span class="sxs-lookup"><span data-stu-id="8d0d4-129">Name</span></span>          | <span data-ttu-id="8d0d4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8d0d4-130">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="8d0d4-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d0d4-131">Authorization</span></span> | <span data-ttu-id="8d0d4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8d0d4-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d0d4-134">Content-Type</span></span>  | <span data-ttu-id="8d0d4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d0d4-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d0d4-137">Request body</span></span>

<span data-ttu-id="8d0d4-138">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-138">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8d0d4-139">Существующие свойства (за исключением свойств внутри `properties` объекта), не включенных в текст запроса, сохраняют свои предыдущие значения или пересчитываются в зависимости от изменений значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-139">Existing properties (excluding properties inside the `properties` object) that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8d0d4-140">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-140">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="8d0d4-141">Могут быть обновлены перечисленные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-141">The following properties can be updated.</span></span>

| <span data-ttu-id="8d0d4-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d0d4-142">Property</span></span>   | <span data-ttu-id="8d0d4-143">Тип</span><span class="sxs-lookup"><span data-stu-id="8d0d4-143">Type</span></span>                                  | <span data-ttu-id="8d0d4-144">Описание</span><span class="sxs-lookup"><span data-stu-id="8d0d4-144">Description</span></span>               |
|:-----------|:--------------------------------------|:--------------------------|
| <span data-ttu-id="8d0d4-145">списки</span><span class="sxs-lookup"><span data-stu-id="8d0d4-145">acl</span></span>        | <span data-ttu-id="8d0d4-146">Коллекция [списков управления доступом](../resources/acl.md)</span><span class="sxs-lookup"><span data-stu-id="8d0d4-146">[acl](../resources/acl.md) collection</span></span> | <span data-ttu-id="8d0d4-147">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-147">An array of access control entries.</span></span> <span data-ttu-id="8d0d4-148">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-148">Each entry specifies the access granted to a user or group.</span></span> |
| <span data-ttu-id="8d0d4-149">содержимое</span><span class="sxs-lookup"><span data-stu-id="8d0d4-149">content</span></span>    | [<span data-ttu-id="8d0d4-150">екстерналитемконтент</span><span class="sxs-lookup"><span data-stu-id="8d0d4-150">externalItemContent</span></span>](../resources/externalitemcontent.md) | <span data-ttu-id="8d0d4-151">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-151">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="8d0d4-152">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-152">The text in this property is full-text indexed.</span></span> |
| <span data-ttu-id="8d0d4-153">properties</span><span class="sxs-lookup"><span data-stu-id="8d0d4-153">properties</span></span> | <span data-ttu-id="8d0d4-154">Объект</span><span class="sxs-lookup"><span data-stu-id="8d0d4-154">Object</span></span>                                | <span data-ttu-id="8d0d4-155">Контейнер свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-155">A property bag with the properties of the item.</span></span> <span data-ttu-id="8d0d4-156">Свойства должны соответствовать [схеме](../resources/schema.md) , определенной для [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="8d0d4-156">The properties MUST conform to the [schema](../resources/schema.md) defined for the [externalConnection](../resources/externalconnection.md).</span></span> |

### <a name="updating-the-acl-collection"></a><span data-ttu-id="8d0d4-157">Обновление коллекции ACL</span><span class="sxs-lookup"><span data-stu-id="8d0d4-157">Updating the acl collection</span></span>

<span data-ttu-id="8d0d4-158">Если `acl` свойство включено в запрос на обновление, существующая коллекция списков ACL перезаписывается коллекцией, включенной в запрос.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-158">If the `acl` property is included in an update request, the existing ACL collection is overwritten with the collection included in the request.</span></span>

### <a name="updating-the-properties-object"></a><span data-ttu-id="8d0d4-159">Обновление объекта Properties</span><span class="sxs-lookup"><span data-stu-id="8d0d4-159">Updating the properties object</span></span>

<span data-ttu-id="8d0d4-160">Если `properties` свойство включено в запрос на обновление, существующий контейнер свойств перезаписывается значением, включенным в запрос.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-160">If the `properties` property is included in an update request, the existing property bag is overwritten with the value included in the request.</span></span>

## <a name="response"></a><span data-ttu-id="8d0d4-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d0d4-161">Response</span></span>

<span data-ttu-id="8d0d4-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [екстерналитем](../resources/externalitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-162">If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d0d4-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d0d4-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d0d4-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d0d4-164">Request</span></span>

<span data-ttu-id="8d0d4-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d0d4-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d0d4-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="8d0d4-167">C#</span><span class="sxs-lookup"><span data-stu-id="8d0d4-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d0d4-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d0d4-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d0d4-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d0d4-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="8d0d4-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d0d4-170">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="8d0d4-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d0d4-171">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "TSP228082938",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_externalitem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->


