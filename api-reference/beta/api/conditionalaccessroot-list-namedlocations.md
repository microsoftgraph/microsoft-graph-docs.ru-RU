---
title: Список Намедлокатионс
description: Получение списка объектов Намедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a51aec675f0596eb5232f2f3d6160a22f03d0b7f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437947"
---
# <a name="list-namedlocations"></a><span data-ttu-id="1f950-103">Список Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="1f950-103">List namedLocations</span></span>

<span data-ttu-id="1f950-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1f950-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f950-105">Получение списка объектов [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="1f950-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f950-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f950-106">Permissions</span></span>

<span data-ttu-id="1f950-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f950-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f950-109">Permission type</span></span>                        | <span data-ttu-id="1f950-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f950-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f950-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f950-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f950-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f950-112">Policy.Read.All</span></span> |
| <span data-ttu-id="1f950-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f950-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f950-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f950-114">Not supported.</span></span> |
| <span data-ttu-id="1f950-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f950-115">Application</span></span>                            | <span data-ttu-id="1f950-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f950-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f950-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f950-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f950-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f950-118">Optional query parameters</span></span>

<span data-ttu-id="1f950-119">Этот метод поддерживает параметры `$count`запросов `$filter`, `$orderBy` `$select` `$skip`,,, и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1f950-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="1f950-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1f950-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f950-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f950-121">Request headers</span></span>

| <span data-ttu-id="1f950-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1f950-122">Name</span></span>      |<span data-ttu-id="1f950-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1f950-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f950-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f950-124">Authorization</span></span> | <span data-ttu-id="1f950-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f950-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f950-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f950-127">Request body</span></span>

<span data-ttu-id="1f950-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f950-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f950-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f950-129">Response</span></span>

<span data-ttu-id="1f950-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [намедлокатион](../resources/namedlocation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f950-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f950-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f950-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="1f950-132">Пример 1: List All ALL Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="1f950-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="1f950-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f950-133">Request</span></span>

<span data-ttu-id="1f950-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f950-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f950-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f950-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations
```
# <a name="c"></a>[<span data-ttu-id="1f950-136">C#</span><span class="sxs-lookup"><span data-stu-id="1f950-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f950-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f950-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f950-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f950-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f950-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f950-139">Response</span></span>

<span data-ttu-id="1f950-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f950-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1f950-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f950-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="1f950-143">Пример 2: список всех Ипнамедлокатионс</span><span class="sxs-lookup"><span data-stu-id="1f950-143">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="1f950-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f950-144">Request</span></span>

<span data-ttu-id="1f950-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f950-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f950-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f950-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="c"></a>[<span data-ttu-id="1f950-147">C#</span><span class="sxs-lookup"><span data-stu-id="1f950-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f950-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f950-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f950-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f950-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f950-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f950-150">Response</span></span>

<span data-ttu-id="1f950-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f950-151">The following is an example of the response.</span></span>

> <span data-ttu-id="1f950-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f950-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="1f950-154">Пример 3: список всех Намедлокатионс, созданных после определенной даты</span><span class="sxs-lookup"><span data-stu-id="1f950-154">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="1f950-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f950-155">Request</span></span>

<span data-ttu-id="1f950-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f950-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f950-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f950-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="1f950-158">C#</span><span class="sxs-lookup"><span data-stu-id="1f950-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f950-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f950-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f950-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f950-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f950-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f950-161">Response</span></span>

<span data-ttu-id="1f950-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f950-162">The following is an example of the response.</span></span>

> <span data-ttu-id="1f950-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f950-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="1f950-165">Пример 4: список всех Каунтринамедлокатионс, содержащих определенную страну или регион</span><span class="sxs-lookup"><span data-stu-id="1f950-165">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="1f950-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f950-166">Request</span></span>

<span data-ttu-id="1f950-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f950-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f950-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f950-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="c"></a>[<span data-ttu-id="1f950-169">C#</span><span class="sxs-lookup"><span data-stu-id="1f950-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f950-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f950-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f950-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f950-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1f950-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f950-172">Response</span></span>

<span data-ttu-id="1f950-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f950-173">The following is an example of the response.</span></span>

> <span data-ttu-id="1f950-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f950-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
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
