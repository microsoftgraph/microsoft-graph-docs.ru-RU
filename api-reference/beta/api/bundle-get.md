---
author: JeremyKelley
title: Получить пакет
description: Получить пакет driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b6f1619bbb169a92841d3999c43603860c0038fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047793"
---
# <a name="get-bundle"></a><span data-ttu-id="74d0f-103">Получить пакет</span><span class="sxs-lookup"><span data-stu-id="74d0f-103">Get bundle</span></span>

<span data-ttu-id="74d0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74d0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74d0f-105">Извлечение метаданных для [пакета][] на основе уникального ID пакета.</span><span class="sxs-lookup"><span data-stu-id="74d0f-105">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="74d0f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74d0f-106">Permissions</span></span>

<span data-ttu-id="74d0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74d0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74d0f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74d0f-109">Permission type</span></span>      | <span data-ttu-id="74d0f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74d0f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74d0f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74d0f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="74d0f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74d0f-112">Not supported.</span></span>                             |
|<span data-ttu-id="74d0f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74d0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74d0f-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74d0f-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="74d0f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74d0f-115">Application</span></span>          | <span data-ttu-id="74d0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74d0f-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="74d0f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74d0f-117">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="74d0f-118">Так как пакеты являются элементами, можно использовать **коллекцию** элементов для возврата метаданных о пакете.</span><span class="sxs-lookup"><span data-stu-id="74d0f-118">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="74d0f-119">Вы также можете использовать коллекцию **пакетов** в качестве удобства, чтобы убедиться, что вы получаете пакет в ответ.</span><span class="sxs-lookup"><span data-stu-id="74d0f-119">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="74d0f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="74d0f-120">Optional query parameters</span></span>

<span data-ttu-id="74d0f-121">Чтобы ограничить форму объектов, возвращаемых в результате вызова, вы можете использовать [параметры запросов OData][odata-parameters].</span><span class="sxs-lookup"><span data-stu-id="74d0f-121">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74d0f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74d0f-122">Request headers</span></span>
| <span data-ttu-id="74d0f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="74d0f-123">Name</span></span>          | <span data-ttu-id="74d0f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="74d0f-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="74d0f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74d0f-125">Authorization</span></span> | <span data-ttu-id="74d0f-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74d0f-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="74d0f-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="74d0f-128">if-none-match</span></span> | <span data-ttu-id="74d0f-129">eTag.</span><span class="sxs-lookup"><span data-stu-id="74d0f-129">eTag.</span></span> <span data-ttu-id="74d0f-130">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="74d0f-130">Optional.</span></span> <span data-ttu-id="74d0f-131">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="74d0f-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="74d0f-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74d0f-132">Request body</span></span>

<span data-ttu-id="74d0f-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74d0f-133">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="74d0f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="74d0f-134">Response</span></span>

<span data-ttu-id="74d0f-135">В случае успешной работы этот метод возвращает [driveItem][driveItem] resource with the [bundle][bundle] в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="74d0f-135">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="74d0f-136">Дополнительные сведения о возвращении ошибок см. в статье [Отклики с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="74d0f-136">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="74d0f-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="74d0f-137">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="74d0f-138">Пример 1. Получить пакет</span><span class="sxs-lookup"><span data-stu-id="74d0f-138">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="74d0f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="74d0f-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="74d0f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="74d0f-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="74d0f-141">C#</span><span class="sxs-lookup"><span data-stu-id="74d0f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74d0f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74d0f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74d0f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74d0f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74d0f-144">Java</span><span class="sxs-lookup"><span data-stu-id="74d0f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-metadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="74d0f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="74d0f-145">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "My Photo Album Bundle",
  "eTag": "etag",
  "cTag": "etag",
  "createdBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "createdDateTime": "datetime",
  "lastModifiedBy": { "user": { "id": "1234", "displayName": "Ryan Gregg" } },
  "lastModifiedDateTime": "datetime",
  "size": 1234,
  "webUrl": "http://onedrive.com/...",
  "bundle": {
    "childCount": 4,
     "album": { }
  }
}
```

<span data-ttu-id="74d0f-146">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74d0f-146">The response object shown here might be shortened for readability.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="74d0f-147">Пример 2. Получить пакет и его детей в одном вызове</span><span class="sxs-lookup"><span data-stu-id="74d0f-147">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="74d0f-148">Параметр строки запроса можно использовать для включения детей пакета в тот же вызов, что и для запроса метаданных [`expand`](/graph/query-parameters) пакета.</span><span class="sxs-lookup"><span data-stu-id="74d0f-148">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="74d0f-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="74d0f-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="74d0f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="74d0f-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="c"></a>[<span data-ttu-id="74d0f-151">C#</span><span class="sxs-lookup"><span data-stu-id="74d0f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74d0f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74d0f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74d0f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74d0f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74d0f-154">Java</span><span class="sxs-lookup"><span data-stu-id="74d0f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-and-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="74d0f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="74d0f-155">Response</span></span>

<span data-ttu-id="74d0f-156">Этот вызов возвращает метаданные пакета и список детей пакета.</span><span class="sxs-lookup"><span data-stu-id="74d0f-156">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="74d0f-157">Если в пакете нет детей, он возвращает пустую коллекцию.</span><span class="sxs-lookup"><span data-stu-id="74d0f-157">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="74d0f-158">Если количество детей в пакете больше размера страницы по умолчанию, **свойство children@odata.nextLink** возвращается с URL-адресом, который можно использовать для запроса следующей страницы детей в пакете.</span><span class="sxs-lookup"><span data-stu-id="74d0f-158">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "101230100alkc",
  "name": "My Cool Day at the Beach",
  "children": [
    { "id": "120100abab", "name": "image1.jpg", "file": {} },
    { "id": "120100abo1", "name": "image2.jpg", "file": {} }
  ],
  "children@odata.nextLink": "https://api.onedrive.com/v1.0/..."
}
```

<span data-ttu-id="74d0f-159">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74d0f-159">The response object shown here might be shortened for readability.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Get Bundle Metadata"
} -->


