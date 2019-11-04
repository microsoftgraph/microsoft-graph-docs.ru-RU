---
title: Получение Ипнамедлокатион
description: Получение свойств и связей объекта ипнамедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 77b276877c416aaf4cfc21b9a152ac84f5ac59a0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938488"
---
# <a name="get-ipnamedlocation"></a><span data-ttu-id="0a9b0-103">Получение Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="0a9b0-103">Get ipNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a9b0-104">Получение свойств и связей объекта [ипнамедлокатион](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="0a9b0-104">Retrieve the properties and relationships of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a9b0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a9b0-105">Permissions</span></span>

<span data-ttu-id="0a9b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a9b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a9b0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a9b0-108">Permission type</span></span>                        | <span data-ttu-id="0a9b0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a9b0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a9b0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a9b0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a9b0-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a9b0-111">Policy.Read.All</span></span> |
| <span data-ttu-id="0a9b0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a9b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a9b0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-113">Not supported.</span></span> |
| <span data-ttu-id="0a9b0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a9b0-114">Application</span></span>                            | <span data-ttu-id="0a9b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a9b0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a9b0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a9b0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a9b0-117">Optional query parameters</span></span>

<span data-ttu-id="0a9b0-118">Этот метод поддерживает параметр `select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-118">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="0a9b0-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0a9b0-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a9b0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a9b0-120">Request headers</span></span>

| <span data-ttu-id="0a9b0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0a9b0-121">Name</span></span>      |<span data-ttu-id="0a9b0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0a9b0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a9b0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a9b0-123">Authorization</span></span> | <span data-ttu-id="0a9b0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a9b0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a9b0-126">Request body</span></span>

<span data-ttu-id="0a9b0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a9b0-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a9b0-128">Response</span></span>

<span data-ttu-id="0a9b0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [ипнамедлокатион](../resources/ipnamedlocation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-129">If successful, this method returns a `200 OK` response code and the requested [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a9b0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0a9b0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a9b0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a9b0-131">Request</span></span>

<span data-ttu-id="0a9b0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a9b0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a9b0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ipnamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a9b0-134">C#</span><span class="sxs-lookup"><span data-stu-id="0a9b0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a9b0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a9b0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a9b0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a9b0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a9b0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a9b0-137">Response</span></span>

<span data-ttu-id="0a9b0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-138">The following is an example of the response.</span></span>

> <span data-ttu-id="0a9b0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a9b0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
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
