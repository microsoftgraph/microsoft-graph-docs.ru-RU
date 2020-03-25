---
title: Получение Принтконнектор
description: Получение свойств и связей объекта Connector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8999a4371ea50b2d3438bcca20d2bf3c205f7bcf
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948159"
---
# <a name="get-printconnector"></a><span data-ttu-id="dd3a0-103">Получение Принтконнектор</span><span class="sxs-lookup"><span data-stu-id="dd3a0-103">Get printConnector</span></span>

<span data-ttu-id="dd3a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd3a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd3a0-105">Получение свойств и связей объекта **принтконнектор** .</span><span class="sxs-lookup"><span data-stu-id="dd3a0-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd3a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd3a0-106">Permissions</span></span>
<span data-ttu-id="dd3a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd3a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dd3a0-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="dd3a0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd3a0-110">Permission type</span></span> | <span data-ttu-id="dd3a0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd3a0-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="dd3a0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd3a0-112">Delegated (work or school account)</span></span>| <span data-ttu-id="dd3a0-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="dd3a0-113">Users.Read.All</span></span> |
|<span data-ttu-id="dd3a0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd3a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd3a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-115">Not Supported.</span></span>|
|<span data-ttu-id="dd3a0-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="dd3a0-116">Application</span></span>|<span data-ttu-id="dd3a0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd3a0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd3a0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd3a0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd3a0-119">Optional query parameters</span></span>
<span data-ttu-id="dd3a0-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dd3a0-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dd3a0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd3a0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd3a0-122">Request headers</span></span>
| <span data-ttu-id="dd3a0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="dd3a0-123">Name</span></span>      |<span data-ttu-id="dd3a0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dd3a0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd3a0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd3a0-125">Authorization</span></span> | <span data-ttu-id="dd3a0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd3a0-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd3a0-128">Request body</span></span>
<span data-ttu-id="dd3a0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dd3a0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd3a0-130">Response</span></span>
<span data-ttu-id="dd3a0-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтконнектор](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-131">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd3a0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="dd3a0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd3a0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd3a0-133">Request</span></span>
<span data-ttu-id="dd3a0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd3a0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd3a0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="dd3a0-136">C#</span><span class="sxs-lookup"><span data-stu-id="dd3a0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd3a0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd3a0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd3a0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd3a0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd3a0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd3a0-139">Response</span></span>
<span data-ttu-id="dd3a0-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-140">The following is an example of the response.</span></span>
><span data-ttu-id="dd3a0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd3a0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1097

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "name": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  },
  "registeredBy": {}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
