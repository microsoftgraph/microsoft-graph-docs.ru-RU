---
title: Список Намедлокатионс
description: Получение списка объектов Намедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 387e27b30fe9dae92b22855e0f5b6ff721b4019c
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747559"
---
# <a name="list-namedlocations"></a><span data-ttu-id="c56db-103">Список Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="c56db-103">List namedLocations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c56db-104">Получение списка объектов [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="c56db-104">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c56db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c56db-105">Permissions</span></span>

<span data-ttu-id="c56db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c56db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c56db-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c56db-108">Permission type</span></span>                        | <span data-ttu-id="c56db-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c56db-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c56db-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c56db-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c56db-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c56db-111">Policy.Read.All</span></span> |
| <span data-ttu-id="c56db-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c56db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c56db-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c56db-113">Not supported.</span></span> |
| <span data-ttu-id="c56db-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c56db-114">Application</span></span>                            | <span data-ttu-id="c56db-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c56db-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c56db-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c56db-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c56db-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c56db-117">Optional query parameters</span></span>

<span data-ttu-id="c56db-118">Этот метод поддерживает параметры `$count`запросов `$filter`, `$orderBy` `$select` `$skip`,,, и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c56db-118">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="c56db-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c56db-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c56db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c56db-120">Request headers</span></span>

| <span data-ttu-id="c56db-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c56db-121">Name</span></span>      |<span data-ttu-id="c56db-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c56db-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c56db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c56db-123">Authorization</span></span> | <span data-ttu-id="c56db-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c56db-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c56db-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c56db-126">Request body</span></span>

<span data-ttu-id="c56db-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c56db-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c56db-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c56db-128">Response</span></span>

<span data-ttu-id="c56db-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [намедлокатион](../resources/namedlocation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c56db-129">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c56db-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="c56db-130">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="c56db-131">Пример 1: List All ALL Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="c56db-131">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="c56db-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c56db-132">Request</span></span>

<span data-ttu-id="c56db-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c56db-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c56db-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c56db-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c56db-135">C#</span><span class="sxs-lookup"><span data-stu-id="c56db-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c56db-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c56db-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c56db-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c56db-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c56db-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c56db-138">Response</span></span>

<span data-ttu-id="c56db-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c56db-139">The following is an example of the response.</span></span>

> <span data-ttu-id="c56db-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c56db-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="c56db-142">Пример 2: список всех Ипнамедлокатионс</span><span class="sxs-lookup"><span data-stu-id="c56db-142">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="c56db-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c56db-143">Request</span></span>

<span data-ttu-id="c56db-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c56db-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c56db-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="c56db-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c56db-146">C#</span><span class="sxs-lookup"><span data-stu-id="c56db-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c56db-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c56db-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c56db-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c56db-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c56db-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c56db-149">Response</span></span>

<span data-ttu-id="c56db-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c56db-150">The following is an example of the response.</span></span>

> <span data-ttu-id="c56db-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c56db-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="c56db-153">Пример 3: список всех Намедлокатионс, созданных после определенной даты</span><span class="sxs-lookup"><span data-stu-id="c56db-153">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="c56db-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="c56db-154">Request</span></span>

<span data-ttu-id="c56db-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c56db-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c56db-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="c56db-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c56db-157">C#</span><span class="sxs-lookup"><span data-stu-id="c56db-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c56db-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c56db-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c56db-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c56db-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c56db-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c56db-160">Response</span></span>

<span data-ttu-id="c56db-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c56db-161">The following is an example of the response.</span></span>

> <span data-ttu-id="c56db-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c56db-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="c56db-164">Пример 4: список всех Каунтринамедлокатионс, содержащих определенную страну или регион</span><span class="sxs-lookup"><span data-stu-id="c56db-164">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="c56db-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="c56db-165">Request</span></span>

<span data-ttu-id="c56db-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c56db-166">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c56db-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="c56db-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c56db-168">C#</span><span class="sxs-lookup"><span data-stu-id="c56db-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c56db-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c56db-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c56db-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c56db-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c56db-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="c56db-171">Response</span></span>

<span data-ttu-id="c56db-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c56db-172">The following is an example of the response.</span></span>

> <span data-ttu-id="c56db-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c56db-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
