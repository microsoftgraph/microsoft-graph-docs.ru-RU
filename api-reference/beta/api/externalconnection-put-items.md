---
title: Создание Екстерналитем
description: Создание нового Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7d6b7f1abf94aacd7732c7fb767a0220d6892abf
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718607"
---
# <a name="create-externalitem"></a><span data-ttu-id="b5f25-103">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="b5f25-103">Create externalItem</span></span>

<span data-ttu-id="b5f25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5f25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5f25-105">Создание нового [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="b5f25-105">Create a new [externalItem](../resources/externalitem.md).</span></span>

<span data-ttu-id="b5f25-106">Этот API можно использовать для создания настраиваемого элемента.</span><span class="sxs-lookup"><span data-stu-id="b5f25-106">This API can be used to create a custom item.</span></span> <span data-ttu-id="b5f25-107">Укажите тип, который вы создаете, включив `@odata.type` свойство в текст JSON.</span><span class="sxs-lookup"><span data-stu-id="b5f25-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="b5f25-108">В содержащем [екстерналконнектион](../resources/externalconnection.md) должна быть зарегистрирована [схема](../resources/schema.md) соответствующего типа.</span><span class="sxs-lookup"><span data-stu-id="b5f25-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="b5f25-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5f25-109">Permissions</span></span>

<span data-ttu-id="b5f25-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5f25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5f25-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5f25-112">Permission type</span></span>                        | <span data-ttu-id="b5f25-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5f25-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5f25-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5f25-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5f25-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5f25-115">Not supported.</span></span> |
| <span data-ttu-id="b5f25-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5f25-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5f25-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5f25-117">Not supported.</span></span> |
| <span data-ttu-id="b5f25-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5f25-118">Application</span></span>                            | <span data-ttu-id="b5f25-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5f25-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5f25-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5f25-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="b5f25-121">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="b5f25-121">Path parameters</span></span>

| <span data-ttu-id="b5f25-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="b5f25-122">Parameter</span></span>     | <span data-ttu-id="b5f25-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b5f25-123">Type</span></span>   | <span data-ttu-id="b5f25-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b5f25-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="b5f25-125">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="b5f25-125">connection-id</span></span> | <span data-ttu-id="b5f25-126">string</span><span class="sxs-lookup"><span data-stu-id="b5f25-126">string</span></span> | <span data-ttu-id="b5f25-127">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="b5f25-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="b5f25-128">item-id</span><span class="sxs-lookup"><span data-stu-id="b5f25-128">item-id</span></span>       | <span data-ttu-id="b5f25-129">string</span><span class="sxs-lookup"><span data-stu-id="b5f25-129">string</span></span> | <span data-ttu-id="b5f25-130">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="b5f25-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> <span data-ttu-id="b5f25-131">Если такой `id`элемент уже не существует, создается новый элемент.</span><span class="sxs-lookup"><span data-stu-id="b5f25-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="b5f25-132">Если такой `id`элемент уже существует, он перезаписывается объектом, отправленным в теле.</span><span class="sxs-lookup"><span data-stu-id="b5f25-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b5f25-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5f25-133">Request headers</span></span>

| <span data-ttu-id="b5f25-134">Имя</span><span class="sxs-lookup"><span data-stu-id="b5f25-134">Name</span></span>          | <span data-ttu-id="b5f25-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b5f25-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="b5f25-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5f25-136">Authorization</span></span> | <span data-ttu-id="b5f25-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5f25-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b5f25-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5f25-139">Content-Type</span></span>  | <span data-ttu-id="b5f25-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5f25-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5f25-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5f25-142">Request body</span></span>

<span data-ttu-id="b5f25-143">В тексте запроса добавьте представление объекта [екстерналитем](../resources/externalitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5f25-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) object.</span></span> <span data-ttu-id="b5f25-144">Размер полезных данных не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="b5f25-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="b5f25-145">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="b5f25-145">Creating an externalItem</span></span>

<span data-ttu-id="b5f25-146">При создании `externalItem`необходимо указать следующие поля: `@odata.type`, `acl`, и. `properties`</span><span class="sxs-lookup"><span data-stu-id="b5f25-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="b5f25-147">`properties` Объект должен содержать по крайней мере одно свойство.</span><span class="sxs-lookup"><span data-stu-id="b5f25-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="b5f25-148">Все `DateTime` свойства типа должны быть в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="b5f25-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="b5f25-149">Свойства в полезных `externalItem` данных должны использовать описатели типов в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="b5f25-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="b5f25-150">Для `String` свойств Type, если значение содержит символы, не входящие в набор ASCII.</span><span class="sxs-lookup"><span data-stu-id="b5f25-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="b5f25-151">Для всех типов коллекций.</span><span class="sxs-lookup"><span data-stu-id="b5f25-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="b5f25-152">При включении свойства типа `Collection(DateTime)`необходимо использовать описатель типа. `Collection(DateTimeOffset)`</span><span class="sxs-lookup"><span data-stu-id="b5f25-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

## <a name="response"></a><span data-ttu-id="b5f25-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5f25-153">Response</span></span>

<span data-ttu-id="b5f25-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="b5f25-154">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b5f25-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5f25-155">Examples</span></span>

### <a name="example-create-a-custom-item"></a><span data-ttu-id="b5f25-156">Пример: Создание настраиваемого элемента</span><span class="sxs-lookup"><span data-stu-id="b5f25-156">Example: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="b5f25-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5f25-157">Request</span></span>

<span data-ttu-id="b5f25-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5f25-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5f25-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5f25-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "deny",
      "identitySource": "Azure Active Directory"
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
# <a name="c"></a>[<span data-ttu-id="b5f25-160">C#</span><span class="sxs-lookup"><span data-stu-id="b5f25-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5f25-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5f25-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5f25-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5f25-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="b5f25-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5f25-163">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b5f25-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b5f25-164">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
