---
title: Получение Ипнамедлокатион
description: Получение свойств и связей объекта ипнамедлокатион.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3ca0aaafe1dd9a18507e8c20b7bffa941c0a71e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025720"
---
# <a name="get-ipnamedlocation"></a><span data-ttu-id="77dfe-103">Получение Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="77dfe-103">Get ipNamedLocation</span></span>

<span data-ttu-id="77dfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77dfe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77dfe-105">Получение свойств и связей объекта [ипнамедлокатион](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="77dfe-105">Retrieve the properties and relationships of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77dfe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77dfe-106">Permissions</span></span>

<span data-ttu-id="77dfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77dfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77dfe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77dfe-109">Permission type</span></span>                        | <span data-ttu-id="77dfe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77dfe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77dfe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77dfe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="77dfe-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="77dfe-112">Policy.Read.All</span></span> |
| <span data-ttu-id="77dfe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77dfe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77dfe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77dfe-114">Not supported.</span></span> |
| <span data-ttu-id="77dfe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77dfe-115">Application</span></span>                            | <span data-ttu-id="77dfe-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="77dfe-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77dfe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77dfe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77dfe-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77dfe-118">Optional query parameters</span></span>

<span data-ttu-id="77dfe-119">Этот метод поддерживает `select` параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77dfe-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="77dfe-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="77dfe-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="77dfe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77dfe-121">Request headers</span></span>

| <span data-ttu-id="77dfe-122">Имя</span><span class="sxs-lookup"><span data-stu-id="77dfe-122">Name</span></span>      |<span data-ttu-id="77dfe-123">Описание</span><span class="sxs-lookup"><span data-stu-id="77dfe-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77dfe-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77dfe-124">Authorization</span></span> | <span data-ttu-id="77dfe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77dfe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77dfe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77dfe-127">Request body</span></span>

<span data-ttu-id="77dfe-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77dfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77dfe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="77dfe-129">Response</span></span>

<span data-ttu-id="77dfe-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [ипнамедлокатион](../resources/ipnamedlocation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77dfe-130">If successful, this method returns a `200 OK` response code and the requested [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77dfe-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="77dfe-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77dfe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="77dfe-132">Request</span></span>

<span data-ttu-id="77dfe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77dfe-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="77dfe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="77dfe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ipnamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="77dfe-135">C#</span><span class="sxs-lookup"><span data-stu-id="77dfe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77dfe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77dfe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77dfe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77dfe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77dfe-138">Java</span><span class="sxs-lookup"><span data-stu-id="77dfe-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ipnamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77dfe-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="77dfe-139">Response</span></span>

<span data-ttu-id="77dfe-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77dfe-140">The following is an example of the response.</span></span>

> <span data-ttu-id="77dfe-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77dfe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "id": "0854951d-5fc0-4eb1-b392-9b2c9d7949c2",
    "displayName": "Untrusted IP named location",
    "modifiedDateTime": "2019-09-04T01:11:34.9387578Z",
    "createdDateTime": "2019-09-04T01:11:34.9387578Z",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ipNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

