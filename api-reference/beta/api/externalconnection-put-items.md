---
title: Создание Екстерналитем
description: Создание нового Екстерналитем.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 298a5bc01b3891831e1a8fd6774d721dc977b940
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869794"
---
# <a name="create-externalitem"></a><span data-ttu-id="f5b21-103">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f5b21-103">Create externalItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5b21-104">Создание нового [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="f5b21-104">Create a new [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

<span data-ttu-id="f5b21-105">Этот API можно использовать для создания настраиваемого элемента или файла.</span><span class="sxs-lookup"><span data-stu-id="f5b21-105">This API can be used to create a custom item or a file.</span></span> <span data-ttu-id="f5b21-106">Укажите тип, который вы создаете, включив `@odata.type` свойство в текст JSON.</span><span class="sxs-lookup"><span data-stu-id="f5b21-106">Specify the type you are creating by including the `@odata.type` property in the JSON body.</span></span> <span data-ttu-id="f5b21-107">В содержащем [екстерналконнектион](../resources/externalconnection.md) должна быть зарегистрирована [схема](../resources/schema.md) соответствующего типа.</span><span class="sxs-lookup"><span data-stu-id="f5b21-107">The containing [externalConnection](../resources/externalconnection.md) must have a [schema](../resources/schema.md) registered of the corresponding type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="f5b21-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b21-108">Permissions</span></span>

<span data-ttu-id="f5b21-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5b21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5b21-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b21-111">Permission type</span></span>                        | <span data-ttu-id="f5b21-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5b21-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f5b21-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5b21-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5b21-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b21-114">Not supported.</span></span> |
| <span data-ttu-id="f5b21-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5b21-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5b21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b21-116">Not supported.</span></span> |
| <span data-ttu-id="f5b21-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f5b21-117">Application</span></span>                            | <span data-ttu-id="f5b21-118">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b21-118">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5b21-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5b21-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="f5b21-120">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="f5b21-120">Path parameters</span></span>

| <span data-ttu-id="f5b21-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="f5b21-121">Parameter</span></span>     | <span data-ttu-id="f5b21-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f5b21-122">Type</span></span>   | <span data-ttu-id="f5b21-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b21-123">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="f5b21-124">ИД подключения</span><span class="sxs-lookup"><span data-stu-id="f5b21-124">connection-id</span></span> | <span data-ttu-id="f5b21-125">string</span><span class="sxs-lookup"><span data-stu-id="f5b21-125">string</span></span> | <span data-ttu-id="f5b21-126">`id` Свойство содержащего [екстерналконнектион](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="f5b21-126">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="f5b21-127">item-id</span><span class="sxs-lookup"><span data-stu-id="f5b21-127">item-id</span></span>       | <span data-ttu-id="f5b21-128">string</span><span class="sxs-lookup"><span data-stu-id="f5b21-128">string</span></span> | <span data-ttu-id="f5b21-129">Предоставляемое `id` разработчиком свойство [екстерналитем](../resources/externalitem.md) или [екстерналфиле](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="f5b21-129">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> <span data-ttu-id="f5b21-130">Если такой `id`элемент уже не существует, создается новый элемент.</span><span class="sxs-lookup"><span data-stu-id="f5b21-130">If no item already exists with this `id`, a new item is created.</span></span> <span data-ttu-id="f5b21-131">Если такой `id`элемент уже существует, он перезаписывается объектом, отправленным в теле.</span><span class="sxs-lookup"><span data-stu-id="f5b21-131">If an item already exists with this `id`, it is overwritten by the object sent in the body.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f5b21-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5b21-132">Request headers</span></span>

| <span data-ttu-id="f5b21-133">Имя</span><span class="sxs-lookup"><span data-stu-id="f5b21-133">Name</span></span>          | <span data-ttu-id="f5b21-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b21-134">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="f5b21-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5b21-135">Authorization</span></span> | <span data-ttu-id="f5b21-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b21-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f5b21-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5b21-138">Content-Type</span></span>  | <span data-ttu-id="f5b21-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b21-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5b21-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5b21-141">Request body</span></span>

<span data-ttu-id="f5b21-142">В тексте запроса добавьте представление объекта [екстерналитем](../resources/externalitem.md) или [ЕКСТЕРНАЛФИЛЕ](../resources/externalfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5b21-142">In the request body, supply a JSON representation of an [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md) object.</span></span> <span data-ttu-id="f5b21-143">Размер полезных данных не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="f5b21-143">The payload is limited to 4 MB.</span></span>

### <a name="creating-an-externalitem"></a><span data-ttu-id="f5b21-144">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f5b21-144">Creating an externalItem</span></span>

<span data-ttu-id="f5b21-145">При создании `externalItem`необходимо указать следующие поля: `@odata.type`, `acl`, и. `properties`</span><span class="sxs-lookup"><span data-stu-id="f5b21-145">When creating an `externalItem`, the following fields are required: `@odata.type`, `acl`, and `properties`.</span></span> <span data-ttu-id="f5b21-146">`properties` Объект должен содержать по крайней мере одно свойство.</span><span class="sxs-lookup"><span data-stu-id="f5b21-146">The `properties` object must contain at least one property.</span></span>

<span data-ttu-id="f5b21-147">Все `DateTime` свойства типа должны быть в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="f5b21-147">All `DateTime` type properties must be in ISO 8601 format.</span></span>

<span data-ttu-id="f5b21-148">Свойства в полезных `externalItem` данных должны использовать описатели типов в следующих сценариях:</span><span class="sxs-lookup"><span data-stu-id="f5b21-148">Properties on an `externalItem` should use type specifiers in the payload in the following scenarios:</span></span>

- <span data-ttu-id="f5b21-149">Для `String` свойств Type, если значение содержит символы, не входящие в набор ASCII.</span><span class="sxs-lookup"><span data-stu-id="f5b21-149">For `String` type properties, if the value contains non-ASCII characters.</span></span>

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- <span data-ttu-id="f5b21-150">Для всех типов коллекций.</span><span class="sxs-lookup"><span data-stu-id="f5b21-150">For all collection types.</span></span>

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > <span data-ttu-id="f5b21-151">При включении свойства типа `Collection(DateTime)`необходимо использовать описатель типа. `Collection(DateTimeOffset)`</span><span class="sxs-lookup"><span data-stu-id="f5b21-151">When including a property of type `Collection(DateTime)`, you must use the type specifier `Collection(DateTimeOffset)`.</span></span>

### <a name="creating-an-externalfile"></a><span data-ttu-id="f5b21-152">Создание Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="f5b21-152">Creating an externalFile</span></span>

<span data-ttu-id="f5b21-153">`externalFile`При создании необходимо указать следующие поля: `@odata.type`, `acl`, `name`и. `url`</span><span class="sxs-lookup"><span data-stu-id="f5b21-153">When creating an `externalFile`, the following fields are required: `@odata.type`, `acl`, `name`, and `url`.</span></span>

## <a name="response"></a><span data-ttu-id="f5b21-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5b21-154">Response</span></span>

<span data-ttu-id="f5b21-155">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f5b21-155">If successful, this method returns `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f5b21-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="f5b21-156">Examples</span></span>

### <a name="example-1-create-a-custom-item"></a><span data-ttu-id="f5b21-157">Пример 1: Создание настраиваемого элемента</span><span class="sxs-lookup"><span data-stu-id="f5b21-157">Example 1: Create a custom item</span></span>

#### <a name="request"></a><span data-ttu-id="f5b21-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5b21-158">Request</span></span>

<span data-ttu-id="f5b21-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5b21-159">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f5b21-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5b21-160">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f5b21-161">C#</span><span class="sxs-lookup"><span data-stu-id="f5b21-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5b21-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5b21-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f5b21-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5b21-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="f5b21-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b21-164">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f5b21-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f5b21-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

### <a name="example-2-create-a-file"></a><span data-ttu-id="f5b21-166">Пример 2: создание файла</span><span class="sxs-lookup"><span data-stu-id="f5b21-166">Example 2: Create a file</span></span>

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="f5b21-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5b21-167">Request</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f5b21-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5b21-168">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f5b21-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5b21-169">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f5b21-170">C#</span><span class="sxs-lookup"><span data-stu-id="f5b21-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalfile-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5b21-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5b21-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalfile-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f5b21-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5b21-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalfile-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="f5b21-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b21-173">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f5b21-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5b21-174">The following is an example of the response.</span></span>

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
