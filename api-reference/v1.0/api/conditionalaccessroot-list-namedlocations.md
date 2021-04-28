---
title: Список namedLocations
description: Получите список объектов namedLocation.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 757a71f17aa2d42cbbe40c664fd4a30a3b308875
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054086"
---
# <a name="list-namedlocations"></a><span data-ttu-id="94bb4-103">Список namedLocations</span><span class="sxs-lookup"><span data-stu-id="94bb4-103">List namedLocations</span></span>

<span data-ttu-id="94bb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94bb4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94bb4-105">Получите список объектов [namedLocation.](../resources/namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="94bb4-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="94bb4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94bb4-106">Permissions</span></span>

<span data-ttu-id="94bb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94bb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94bb4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94bb4-109">Permission type</span></span>                        | <span data-ttu-id="94bb4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94bb4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94bb4-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94bb4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94bb4-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="94bb4-112">Policy.Read.All</span></span> |
| <span data-ttu-id="94bb4-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94bb4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94bb4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94bb4-114">Not supported.</span></span> |
| <span data-ttu-id="94bb4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94bb4-115">Application</span></span>                            | <span data-ttu-id="94bb4-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="94bb4-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94bb4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94bb4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94bb4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94bb4-118">Optional query parameters</span></span>

<span data-ttu-id="94bb4-119">Этот метод поддерживает `$count` параметры `$filter` запросов , , , , и `$orderBy` `$select` `$skip` `$top` OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="94bb4-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="94bb4-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="94bb4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="94bb4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94bb4-121">Request headers</span></span>

| <span data-ttu-id="94bb4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="94bb4-122">Name</span></span>      |<span data-ttu-id="94bb4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="94bb4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94bb4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94bb4-124">Authorization</span></span> | <span data-ttu-id="94bb4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94bb4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94bb4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94bb4-127">Request body</span></span>

<span data-ttu-id="94bb4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94bb4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94bb4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="94bb4-129">Response</span></span>

<span data-ttu-id="94bb4-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов namedLocation](../resources/namedlocation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="94bb4-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94bb4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="94bb4-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="94bb4-132">Пример 1. Список всех именных локаций</span><span class="sxs-lookup"><span data-stu-id="94bb4-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="94bb4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="94bb4-133">Request</span></span>

<span data-ttu-id="94bb4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94bb4-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94bb4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="94bb4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
```
# <a name="c"></a>[<span data-ttu-id="94bb4-136">C#</span><span class="sxs-lookup"><span data-stu-id="94bb4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94bb4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94bb4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94bb4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94bb4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94bb4-139">Java</span><span class="sxs-lookup"><span data-stu-id="94bb4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94bb4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="94bb4-140">Response</span></span>

<span data-ttu-id="94bb4-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94bb4-141">The following is an example of the response.</span></span>

> <span data-ttu-id="94bb4-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94bb4-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "06e4ff15-ca6b-4843-9c34-3fdd1ce8f739",
            "displayName": "IPv4 named location",
            "modifiedDateTime": "2019-07-26T18:00:43.5796446Z",
            "createdDateTime": "2018-06-22T11:56:12Z",
            "isTrusted": false,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "6.5.4.3/32"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "127.126.125.0/24"
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.countryNamedLocation",
            "id": "1b7f0916-7677-40d8-97a1-d606f4ed8fcf",
            "displayName": "Country named location",
            "modifiedDateTime": "2018-09-10T16:54:53.7238848Z",
            "createdDateTime": "2018-09-10T16:54:53.7238848Z",
            "countriesAndRegions": [
                "US",
                "CA"
            ],
            "includeUnknownCountriesAndRegions": false
        },
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="94bb4-143">Пример 2. Список всех ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="94bb4-143">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="94bb4-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="94bb4-144">Request</span></span>

<span data-ttu-id="94bb4-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94bb4-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94bb4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="94bb4-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="c"></a>[<span data-ttu-id="94bb4-147">C#</span><span class="sxs-lookup"><span data-stu-id="94bb4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94bb4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94bb4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94bb4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94bb4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94bb4-150">Java</span><span class="sxs-lookup"><span data-stu-id="94bb4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94bb4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="94bb4-151">Response</span></span>

<span data-ttu-id="94bb4-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94bb4-152">The following is an example of the response.</span></span>

> <span data-ttu-id="94bb4-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94bb4-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "06e4ff15-ca6b-4843-9c34-3fdd1ce8f739",
            "displayName": "IPv4 named location",
            "modifiedDateTime": "2019-07-26T18:00:43.5796446Z",
            "createdDateTime": "2018-06-22T11:56:12Z",
            "isTrusted": false,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "6.5.4.3/32"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "127.126.125.0/24"
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="94bb4-154">Пример 3. Список всех имен локаций, созданных после определенной даты</span><span class="sxs-lookup"><span data-stu-id="94bb4-154">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="94bb4-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="94bb4-155">Request</span></span>

<span data-ttu-id="94bb4-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94bb4-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94bb4-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="94bb4-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="94bb4-158">C#</span><span class="sxs-lookup"><span data-stu-id="94bb4-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94bb4-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94bb4-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94bb4-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94bb4-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94bb4-161">Java</span><span class="sxs-lookup"><span data-stu-id="94bb4-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94bb4-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="94bb4-162">Response</span></span>

<span data-ttu-id="94bb4-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94bb4-163">The following is an example of the response.</span></span>

> <span data-ttu-id="94bb4-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94bb4-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="94bb4-165">Пример 4. Список всех имен стран, содержащих определенную страну или регион</span><span class="sxs-lookup"><span data-stu-id="94bb4-165">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="94bb4-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="94bb4-166">Request</span></span>

<span data-ttu-id="94bb4-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94bb4-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94bb4-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="94bb4-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="c"></a>[<span data-ttu-id="94bb4-169">C#</span><span class="sxs-lookup"><span data-stu-id="94bb4-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94bb4-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94bb4-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94bb4-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94bb4-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94bb4-172">Java</span><span class="sxs-lookup"><span data-stu-id="94bb4-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94bb4-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="94bb4-173">Response</span></span>

<span data-ttu-id="94bb4-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94bb4-174">The following is an example of the response.</span></span>

> <span data-ttu-id="94bb4-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94bb4-175">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.countryNamedLocation",
            "id": "1b7f0916-7677-40d8-97a1-d606f4ed8fcf",
            "displayName": "Country named location",
            "modifiedDateTime": "2018-09-10T16:54:53.7238848Z",
            "createdDateTime": "2018-09-10T16:54:53.7238848Z",
            "countriesAndRegions": [
                "US",
                "CA"
            ],
            "includeUnknownCountriesAndRegions": false
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List namedLocations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

