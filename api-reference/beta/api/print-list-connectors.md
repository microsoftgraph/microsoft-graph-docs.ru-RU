---
title: Получение соединителей
description: Получение списка соединителей.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5d1ec9b66d815553af7118a8d256107150f5a8de
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948340"
---
# <a name="list-connectors"></a><span data-ttu-id="7f0b4-103">Список соединителей</span><span class="sxs-lookup"><span data-stu-id="7f0b4-103">List connectors</span></span>

<span data-ttu-id="7f0b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f0b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f0b4-105">Получение списка соединителей.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-105">Retrieve a list of connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f0b4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f0b4-106">Permissions</span></span>
<span data-ttu-id="7f0b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f0b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f0b4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f0b4-109">Permission type</span></span> | <span data-ttu-id="7f0b4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f0b4-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7f0b4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f0b4-111">Delegated (work or school account)</span></span>| <span data-ttu-id="7f0b4-112">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="7f0b4-112">Users.Read.All</span></span> |
|<span data-ttu-id="7f0b4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f0b4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f0b4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-114">Not Supported.</span></span>|
|<span data-ttu-id="7f0b4-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7f0b4-115">Application</span></span>|<span data-ttu-id="7f0b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f0b4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f0b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f0b4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f0b4-118">Optional query parameters</span></span>
<span data-ttu-id="7f0b4-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7f0b4-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7f0b4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="7f0b4-121">Исключения</span><span class="sxs-lookup"><span data-stu-id="7f0b4-121">Exceptions</span></span>
* <span data-ttu-id="7f0b4-122">Операторы `$count` and `$filter` не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-122">The `$count` and `$filter` operators are not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f0b4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f0b4-123">Request headers</span></span>
| <span data-ttu-id="7f0b4-124">Имя</span><span class="sxs-lookup"><span data-stu-id="7f0b4-124">Name</span></span>      |<span data-ttu-id="7f0b4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7f0b4-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f0b4-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f0b4-126">Authorization</span></span> | <span data-ttu-id="7f0b4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f0b4-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f0b4-129">Request body</span></span>
<span data-ttu-id="7f0b4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7f0b4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f0b4-131">Response</span></span>
<span data-ttu-id="7f0b4-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Connector](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-132">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f0b4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7f0b4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f0b4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f0b4-134">Request</span></span>
<span data-ttu-id="7f0b4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f0b4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f0b4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="7f0b4-137">C#</span><span class="sxs-lookup"><span data-stu-id="7f0b4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f0b4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f0b4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f0b4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f0b4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7f0b4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f0b4-140">Response</span></span>
<span data-ttu-id="7f0b4-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-141">The following is an example of the response.</span></span>
><span data-ttu-id="7f0b4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f0b4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "Connector1",
      "fullyQualifiedDomainName": "connector1@redmond.corp.microsoft.com",
      "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
      "appVersion": "0.19.7338.23496",
      "deviceHealth": {
        "lastConnectionTime": "2020-02-04T07:00:00.0000000"
      },
      "registeredDateTime": "2020-02-04T07:00:00.0000000",
      "registeredBy": {},
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
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
