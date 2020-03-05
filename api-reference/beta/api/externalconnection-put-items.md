---
title: Создание Екстерналитем
description: Создание нового Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 8b75e3753555e840b042e8876f91e27ed77b4a76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422056"
---
# <a name="create-externalitem"></a><span data-ttu-id="fa09c-103">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="fa09c-103">Create externalItem</span></span>

<span data-ttu-id="fa09c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fa09c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa09c-105">Создание нового [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="fa09c-105">Create a new [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

<span data-ttu-id="fa09c-106">Этот API можно использовать для создания настраиваемого элемента или файла.</span><span class="sxs-lookup"><span data-stu-id="fa09c-106">This API can be used to create a custom item or a file.</span></span> <span data-ttu-id="fa09c-107">Укажите тип, который вы создаете, включив `@odata.type` свойство в текст JSON.</span><span class="sxs-lookup"><span data-stu-id="fa09c-107">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="fa09c-108">В содержащем [екстерналконнектион](../resources/externalconnection.md) должна быть зарегистрирована [схема](../resources/schema.md) соответствующего типа.</span><span class="sxs-lookup"><span data-stu-id="fa09c-108">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="fa09c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa09c-109">Permissions</span></span>

<span data-ttu-id="fa09c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa09c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa09c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa09c-112">Permission type</span></span>                        | <span data-ttu-id="fa09c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa09c-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa09c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa09c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa09c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa09c-115">Not supported.</span></span> |
| <span data-ttu-id="fa09c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa09c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa09c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa09c-117">Not supported.</span></span> |
| <span data-ttu-id="fa09c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa09c-118">Application</span></span>                            | <span data-ttu-id="fa09c-119">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa09c-119">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa09c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa09c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="fa09c-121">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="fa09c-121">Path parameters</span></span>

| <span data-ttu-id="fa09c-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="fa09c-122">Parameter</span></span>     | <span data-ttu-id="fa09c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fa09c-123">Type</span></span>   | <span data-ttu-id="fa09c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fa09c-124">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="fa09c-125">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="fa09c-125">connection-id</span></span> | <span data-ttu-id="fa09c-126">строка</span><span class="sxs-lookup"><span data-stu-id="fa09c-126">string</span></span> | <span data-ttu-id="fa09c-127">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="fa09c-127">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="fa09c-128">item-id</span><span class="sxs-lookup"><span data-stu-id="fa09c-128">item-id</span></span>       | <span data-ttu-id="fa09c-129">строка</span><span class="sxs-lookup"><span data-stu-id="fa09c-129">string</span></span> | <span data-ttu-id="fa09c-130">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="fa09c-130">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> <span data-ttu-id="fa09c-131">Если такой `id`элемент уже не существует, создается новый элемент.</span><span class="sxs-lookup"><span data-stu-id="fa09c-131">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="fa09c-132">Если такой `id`элемент уже существует, он перезаписывается объектом, отправленным в теле.</span><span class="sxs-lookup"><span data-stu-id="fa09c-132">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fa09c-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa09c-133">Request headers</span></span>

| <span data-ttu-id="fa09c-134">Имя</span><span class="sxs-lookup"><span data-stu-id="fa09c-134">Name</span></span>          | <span data-ttu-id="fa09c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="fa09c-135">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="fa09c-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa09c-136">Authorization</span></span> | <span data-ttu-id="fa09c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa09c-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="fa09c-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa09c-139">Content-Type</span></span>  | <span data-ttu-id="fa09c-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa09c-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa09c-142">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa09c-142">Request body</span></span>

<span data-ttu-id="fa09c-143">В тексте запроса добавьте представление объекта [екстерналитем](../resources/externalitem.md) или [ЕКСТЕРНАЛФИЛЕ](../resources/externalfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa09c-143">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object.</span></span> <span data-ttu-id="fa09c-144">Размер полезных данных не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="fa09c-144">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="fa09c-145">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="fa09c-145">Creating an externalItem</span></span>

<span data-ttu-id="fa09c-146">При создании `externalItem`необходимо указать следующие поля: `@odata.type`, `acl`, и. `properties`</span><span class="sxs-lookup"><span data-stu-id="fa09c-146">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="fa09c-147">`properties` Объект должен содержать по крайней мере одно свойство.</span><span class="sxs-lookup"><span data-stu-id="fa09c-147">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="fa09c-148">Все `DateTime` свойства типа должны быть в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fa09c-148">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="fa09c-149">Свойства в полезных `externalItem` данных должны использовать описатели типов в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="fa09c-149">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="fa09c-150">Для `String` свойств Type, если значение содержит символы, не входящие в набор ASCII.</span><span class="sxs-lookup"><span data-stu-id="fa09c-150">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="fa09c-151">Для всех типов коллекций.</span><span class="sxs-lookup"><span data-stu-id="fa09c-151">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="fa09c-152">При включении свойства типа `Collection(DateTime)`необходимо использовать описатель типа. `Collection(DateTimeOffset)`</span><span class="sxs-lookup"><span data-stu-id="fa09c-152">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

### <a name="creating-an-externalfile"></a><span data-ttu-id="fa09c-153">Создание Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="fa09c-153">Creating an externalFile</span></span>

<span data-ttu-id="fa09c-154">`externalFile`При создании необходимо указать следующие поля: `@odata.type`, `acl`, `name`и. `url`</span><span class="sxs-lookup"><span data-stu-id="fa09c-154">When creating an `externalFile`, the following fields are required: `@odata.type`, `acl`, `name`, and `url`.</span></span>

## <a name="response"></a><span data-ttu-id="fa09c-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa09c-155">Response</span></span>

<span data-ttu-id="fa09c-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="fa09c-156">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fa09c-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa09c-157">Examples</span></span>

### <a name="example-1-create-a-custom-item"></a><span data-ttu-id="fa09c-158">Пример 1: Создание настраиваемого элемента</span><span class="sxs-lookup"><span data-stu-id="fa09c-158">Example 1: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="fa09c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa09c-159">Request</span></span>

<span data-ttu-id="fa09c-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa09c-160">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa09c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa09c-161">HTTP</span></span>](#tab/http)
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
  "content": "Textual content of the file"
}
```
# <a name="c"></a>[<span data-ttu-id="fa09c-162">C#</span><span class="sxs-lookup"><span data-stu-id="fa09c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa09c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa09c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa09c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa09c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="fa09c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa09c-165">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="fa09c-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa09c-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

### <a name="example-2-create-a-file"></a><span data-ttu-id="fa09c-167">Пример 2: создание файла</span><span class="sxs-lookup"><span data-stu-id="fa09c-167">Example 2: Create a file</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="fa09c-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa09c-168">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="fa09c-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa09c-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa09c-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa09c-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalfile_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosofiles/items/myFile01
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalFile",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ],
  "createdDateTime": "2019-01-31T03:44:19.0354159Z",
  "modifiedDateTime": "2019-01-31T03:44:19.0354159Z",
  "createdBy": "Pradeep Gupta",
  "lastModifiedBy": "Adele Vance",
  "title": "Enterprise Search Graph Ingestion API",
  "url": "file://filesrv02.corp.contoso.com/data/project/Enterprise Search.docx",
  "name": "Enterprise Search.docx",
  "extension": "docx",
  "size": 8676776,
  "content": "The quick brown fox jumps over the lazy dog."
}
```
# <a name="c"></a>[<span data-ttu-id="fa09c-171">C#</span><span class="sxs-lookup"><span data-stu-id="fa09c-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalfile-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa09c-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa09c-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalfile-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa09c-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa09c-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalfile-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="fa09c-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa09c-174">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="fa09c-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fa09c-175">The following is an example of the response.</span></span>

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
