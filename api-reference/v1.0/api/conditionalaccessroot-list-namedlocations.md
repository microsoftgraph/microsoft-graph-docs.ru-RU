---
title: Список Намедлокатионс
description: Получение списка объектов Намедлокатион.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cdec20fe4802bb71d410ddd019c8159f46c0cb75
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566047"
---
# <a name="list-namedlocations"></a><span data-ttu-id="a514b-103">Список Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="a514b-103">List namedLocations</span></span>

<span data-ttu-id="a514b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a514b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a514b-105">Получение списка объектов [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="a514b-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a514b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a514b-106">Permissions</span></span>

<span data-ttu-id="a514b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a514b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a514b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a514b-109">Permission type</span></span>                        | <span data-ttu-id="a514b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a514b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a514b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a514b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a514b-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a514b-112">Policy.Read.All</span></span> |
| <span data-ttu-id="a514b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a514b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a514b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a514b-114">Not supported.</span></span> |
| <span data-ttu-id="a514b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a514b-115">Application</span></span>                            | <span data-ttu-id="a514b-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a514b-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a514b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a514b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a514b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a514b-118">Optional query parameters</span></span>

<span data-ttu-id="a514b-119">Этот метод поддерживает `$count` параметры запросов,,,, `$filter` `$orderBy` `$select` `$skip` и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a514b-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a514b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a514b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a514b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a514b-121">Request headers</span></span>

| <span data-ttu-id="a514b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a514b-122">Name</span></span>      |<span data-ttu-id="a514b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a514b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a514b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a514b-124">Authorization</span></span> | <span data-ttu-id="a514b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a514b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a514b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a514b-127">Request body</span></span>

<span data-ttu-id="a514b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a514b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a514b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a514b-129">Response</span></span>

<span data-ttu-id="a514b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [намедлокатион](../resources/namedlocation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a514b-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a514b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a514b-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="a514b-132">Пример 1: List All ALL Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="a514b-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="a514b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a514b-133">Request</span></span>

<span data-ttu-id="a514b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a514b-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a514b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a514b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
```
# <a name="c"></a>[<span data-ttu-id="a514b-136">C#</span><span class="sxs-lookup"><span data-stu-id="a514b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a514b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a514b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a514b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a514b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a514b-139">Java</span><span class="sxs-lookup"><span data-stu-id="a514b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a514b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a514b-140">Response</span></span>

<span data-ttu-id="a514b-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a514b-141">The following is an example of the response.</span></span>

> <span data-ttu-id="a514b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a514b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="a514b-144">Пример 2: список всех Ипнамедлокатионс</span><span class="sxs-lookup"><span data-stu-id="a514b-144">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="a514b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="a514b-145">Request</span></span>

<span data-ttu-id="a514b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a514b-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a514b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="a514b-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="c"></a>[<span data-ttu-id="a514b-148">C#</span><span class="sxs-lookup"><span data-stu-id="a514b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a514b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a514b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a514b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a514b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a514b-151">Java</span><span class="sxs-lookup"><span data-stu-id="a514b-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a514b-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a514b-152">Response</span></span>

<span data-ttu-id="a514b-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a514b-153">The following is an example of the response.</span></span>

> <span data-ttu-id="a514b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a514b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="a514b-156">Пример 3: список всех Намедлокатионс, созданных после определенной даты</span><span class="sxs-lookup"><span data-stu-id="a514b-156">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="a514b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="a514b-157">Request</span></span>

<span data-ttu-id="a514b-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a514b-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a514b-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="a514b-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="a514b-160">C#</span><span class="sxs-lookup"><span data-stu-id="a514b-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a514b-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a514b-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a514b-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a514b-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a514b-163">Java</span><span class="sxs-lookup"><span data-stu-id="a514b-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a514b-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="a514b-164">Response</span></span>

<span data-ttu-id="a514b-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a514b-165">The following is an example of the response.</span></span>

> <span data-ttu-id="a514b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a514b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="a514b-168">Пример 4: список всех Каунтринамедлокатионс, содержащих определенную страну или регион</span><span class="sxs-lookup"><span data-stu-id="a514b-168">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="a514b-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="a514b-169">Request</span></span>

<span data-ttu-id="a514b-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a514b-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a514b-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="a514b-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="c"></a>[<span data-ttu-id="a514b-172">C#</span><span class="sxs-lookup"><span data-stu-id="a514b-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a514b-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a514b-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a514b-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a514b-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a514b-175">Java</span><span class="sxs-lookup"><span data-stu-id="a514b-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a514b-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="a514b-176">Response</span></span>

<span data-ttu-id="a514b-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a514b-177">The following is an example of the response.</span></span>

> <span data-ttu-id="a514b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a514b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
