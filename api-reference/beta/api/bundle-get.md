---
author: JeremyKelley
ms.author: jeremyke
title: Получение пакета
description: Получение пакета элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 55d24648a8cc69f196be4f5aa820fe619281ff4b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318000"
---
# <a name="get-bundle"></a><span data-ttu-id="28ba8-103">Получение пакета</span><span class="sxs-lookup"><span data-stu-id="28ba8-103">Get bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28ba8-104">Получение метаданных для [пакета][] на основе уникального идентификатора пакета.</span><span class="sxs-lookup"><span data-stu-id="28ba8-104">Retrieve the metadata for a [bundle][] based on the bundle's unique ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="28ba8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28ba8-105">Permissions</span></span>

<span data-ttu-id="28ba8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28ba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28ba8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28ba8-108">Permission type</span></span>      | <span data-ttu-id="28ba8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28ba8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28ba8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28ba8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28ba8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28ba8-111">Not supported.</span></span>                             |
|<span data-ttu-id="28ba8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28ba8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28ba8-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28ba8-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="28ba8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28ba8-114">Application</span></span>          | <span data-ttu-id="28ba8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28ba8-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="28ba8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28ba8-116">HTTP request</span></span>

```http
GET /drive/bundles/{bundle-id}
GET /drive/items/{bundle-id}
```

<span data-ttu-id="28ba8-117">Так как пакеты являются элементами, вы можете использовать коллекцию **Items** для возвращения метаданных пакета.</span><span class="sxs-lookup"><span data-stu-id="28ba8-117">Because bundles are items, you can use the **items** collection to return metadata about a bundle.</span></span>
<span data-ttu-id="28ba8-118">Кроме того, вы можете \*\*\*\* использовать коллекцию Collections, чтобы убедиться, что вы получаете пакет в ответе.</span><span class="sxs-lookup"><span data-stu-id="28ba8-118">You can also use the **bundles** collection as a convenience to ensure you're getting a bundle in response.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="28ba8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28ba8-119">Optional query parameters</span></span>

<span data-ttu-id="28ba8-120">Чтобы ограничить форму объектов, возвращаемых в результате вызова, вы можете использовать [параметры запросов OData][odata-parameters].</span><span class="sxs-lookup"><span data-stu-id="28ba8-120">You can use the [OData query parameters][odata-parameters] to restrict the shape of the objects returned from this call.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28ba8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28ba8-121">Request headers</span></span>
| <span data-ttu-id="28ba8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="28ba8-122">Name</span></span>          | <span data-ttu-id="28ba8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="28ba8-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="28ba8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28ba8-124">Authorization</span></span> | <span data-ttu-id="28ba8-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="28ba8-125">Bearer \{token\}.</span></span> <span data-ttu-id="28ba8-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28ba8-126">Required.</span></span> |
| <span data-ttu-id="28ba8-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="28ba8-127">if-none-match</span></span> | <span data-ttu-id="28ba8-128">тегом.</span><span class="sxs-lookup"><span data-stu-id="28ba8-128">eTag.</span></span> <span data-ttu-id="28ba8-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="28ba8-129">Optional.</span></span> <span data-ttu-id="28ba8-130">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) совпадает с текущим тегом файла, то возвращается отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="28ba8-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="28ba8-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28ba8-131">Request body</span></span>

<span data-ttu-id="28ba8-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28ba8-132">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="28ba8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="28ba8-133">Response</span></span>

<span data-ttu-id="28ba8-134">В случае успешного выполнения этот метод возвращает объект [driveItem][driveItem] resource with the [bundle][bundle] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28ba8-134">If successful, this method returns a [driveItem][driveItem] resource with the [bundle][bundle] in the response body.</span></span>

<span data-ttu-id="28ba8-135">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="28ba8-135">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="28ba8-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="28ba8-136">Examples</span></span>

### <a name="example-1-get-a-bundle"></a><span data-ttu-id="28ba8-137">Пример 1: получение пакета</span><span class="sxs-lookup"><span data-stu-id="28ba8-137">Example 1: Get a bundle</span></span>

#### <a name="request"></a><span data-ttu-id="28ba8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="28ba8-138">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="28ba8-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="28ba8-139">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-metadata" } -->

```http
GET https://graph.microsoft.com/beta/drive/bundles/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28ba8-140">C#</span><span class="sxs-lookup"><span data-stu-id="28ba8-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28ba8-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28ba8-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28ba8-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="28ba8-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="28ba8-143">Java</span><span class="sxs-lookup"><span data-stu-id="28ba8-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-metadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28ba8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="28ba8-144">Response</span></span>

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

<span data-ttu-id="28ba8-145">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="28ba8-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="28ba8-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28ba8-146">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-get-a-bundle-and-its-children-in-a-single-call"></a><span data-ttu-id="28ba8-147">Пример 2: получение пакета и его дочерних элементов в едином вызове</span><span class="sxs-lookup"><span data-stu-id="28ba8-147">Example 2: Get a bundle and its children in a single call</span></span>

<span data-ttu-id="28ba8-148">Можно использовать параметр строки [`expand`](/graph/query-parameters) запроса, чтобы включить дочерние элементы пакета в тот же вызов, что и получение метаданных пакета.</span><span class="sxs-lookup"><span data-stu-id="28ba8-148">You can use the [`expand`](/graph/query-parameters) query string parameter to include the children of a bundle in the same call as retrieving the metadata of a bundle.</span></span>

#### <a name="request"></a><span data-ttu-id="28ba8-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="28ba8-149">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="28ba8-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="28ba8-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-bundle-and-children" } -->

```http
GET https://graph.microsoft.com/beta/drive/items/{bundle-id}?expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28ba8-151">C#</span><span class="sxs-lookup"><span data-stu-id="28ba8-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bundle-and-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28ba8-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28ba8-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bundle-and-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28ba8-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="28ba8-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bundle-and-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="28ba8-154">Java</span><span class="sxs-lookup"><span data-stu-id="28ba8-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bundle-and-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28ba8-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="28ba8-155">Response</span></span>

<span data-ttu-id="28ba8-156">Этот вызов возвратит метаданные пакета и список дочерних элементов набора.</span><span class="sxs-lookup"><span data-stu-id="28ba8-156">This call will return the bundle metadata and a list of children of the bundle.</span></span>
<span data-ttu-id="28ba8-157">Если у пакета нет дочерних элементов, он возвратит пустую коллекцию.</span><span class="sxs-lookup"><span data-stu-id="28ba8-157">If the bundle has no children, it will return an empty collection.</span></span>

<span data-ttu-id="28ba8-158">Если количество дочерних элементов в пакете превышает размер страницы по умолчанию, свойство **Children @ OData. nextLink** будет возвращено с URL-адресом, который можно использовать для запроса следующей страницы дочерних элементов в пакете.</span><span class="sxs-lookup"><span data-stu-id="28ba8-158">If the number of children in the bundle is greater than the default page size, the **children@odata.nextLink** property will be returned with a URL that can be used to request the next page of children in the bundle.</span></span>

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

<span data-ttu-id="28ba8-159">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="28ba8-159">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="28ba8-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28ba8-160">All the properties will be returned from an actual call.</span></span>


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
