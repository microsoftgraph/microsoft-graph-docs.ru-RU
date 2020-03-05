---
author: JeremyKelley
ms.author: jeremyke
title: Получение пакета
description: Получение пакета элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 191157efb35b50ecff358d7902a7a6c42a6fb7a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441034"
---
# <a name="get-bundle"></a><span data-ttu-id="1d5cc-103">Получение пакета</span><span class="sxs-lookup"><span data-stu-id="1d5cc-103">Get bundle</span></span>

<span data-ttu-id="1d5cc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1d5cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d5cc-105">Получение метаданных для [пакета][] на основе уникального идентификатора пакета.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-105">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d5cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d5cc-106">Permissions</span></span>

<span data-ttu-id="1d5cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d5cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d5cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d5cc-109">Permission type</span></span>      | <span data-ttu-id="1d5cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d5cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d5cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d5cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d5cc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-112">Not supported.</span></span>                             |
|<span data-ttu-id="1d5cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d5cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d5cc-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d5cc-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d5cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d5cc-115">Application</span></span>          | <span data-ttu-id="1d5cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="1d5cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d5cc-117">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="1d5cc-118">Так как пакеты являются элементами, вы можете использовать коллекцию **Items** для возвращения метаданных пакета.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-118">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="1d5cc-119">Кроме того, вы можете **использовать коллекцию** Collections, чтобы убедиться, что вы получаете пакет в ответе.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-119">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="1d5cc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d5cc-120">Optional query parameters</span></span>

<span data-ttu-id="1d5cc-121">Чтобы ограничить форму объектов, возвращаемых в результате вызова, вы можете использовать [параметры запросов OData][odata-parameters].</span><span class="sxs-lookup"><span data-stu-id="1d5cc-121">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d5cc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d5cc-122">Request headers</span></span>
| <span data-ttu-id="1d5cc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1d5cc-123">Name</span></span>          | <span data-ttu-id="1d5cc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1d5cc-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="1d5cc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d5cc-125">Authorization</span></span> | <span data-ttu-id="1d5cc-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-126">Bearer \{token\}.</span></span> <span data-ttu-id="1d5cc-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-127">Required.</span></span> |
| <span data-ttu-id="1d5cc-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="1d5cc-128">if-none-match</span></span> | <span data-ttu-id="1d5cc-129">тегом.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-129">eTag.</span></span> <span data-ttu-id="1d5cc-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-130">Optional.</span></span> <span data-ttu-id="1d5cc-131">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-131">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="1d5cc-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d5cc-132">Request body</span></span>

<span data-ttu-id="1d5cc-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-133">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d5cc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d5cc-134">Response</span></span>

<span data-ttu-id="1d5cc-135">В случае успешного выполнения этот метод возвращает объект [driveItem][driveItem] resource with the [bundle][bundle] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-135">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="1d5cc-136">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-136">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="1d5cc-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="1d5cc-137">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="1d5cc-138">Пример 1: получение пакета</span><span class="sxs-lookup"><span data-stu-id="1d5cc-138">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="1d5cc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d5cc-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1d5cc-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d5cc-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="1d5cc-141">C#</span><span class="sxs-lookup"><span data-stu-id="1d5cc-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d5cc-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d5cc-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d5cc-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d5cc-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1d5cc-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d5cc-144">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
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

<span data-ttu-id="1d5cc-145">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1d5cc-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-146">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="1d5cc-147">Пример 2: получение пакета и его дочерних элементов в едином вызове</span><span class="sxs-lookup"><span data-stu-id="1d5cc-147">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="1d5cc-148">Можно использовать параметр строки [`expand`](/graph/query-parameters) запроса, чтобы включить дочерние элементы пакета в тот же вызов, что и получение метаданных пакета.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-148">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="1d5cc-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d5cc-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1d5cc-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d5cc-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="c"></a>[<span data-ttu-id="1d5cc-151">C#</span><span class="sxs-lookup"><span data-stu-id="1d5cc-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d5cc-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d5cc-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d5cc-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d5cc-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1d5cc-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d5cc-154">Response</span></span>

<span data-ttu-id="1d5cc-155">Этот вызов возвратит метаданные пакета и список дочерних элементов набора.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-155">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="1d5cc-156">Если у пакета нет дочерних элементов, он возвратит пустую коллекцию.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-156">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="1d5cc-157">Если количество дочерних элементов в пакете превышает размер страницы по умолчанию, свойство **Children@odata. nextLink** будет возвращено с URL-адресом, который можно использовать для запроса следующей страницы дочерних элементов в пакете.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-157">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
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

<span data-ttu-id="1d5cc-158">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-158">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1d5cc-159">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d5cc-159">All the properties will be returned from an actual call.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters


<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about a bundle and its children in OneDrive",
  "keywords": "retrieve,item,bundle,metadata",
  "section": "documentation",
  "tocPath": "Bundles/Get Bundle Metadata"
} -->
