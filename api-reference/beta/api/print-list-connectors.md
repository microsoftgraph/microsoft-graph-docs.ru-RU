---
title: Получение соединителей
description: Получение списка соединителей.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8c83056853939cace3d1341d7a7b70cef066d49a
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812524"
---
# <a name="list-connectors"></a><span data-ttu-id="718b7-103">Список соединителей</span><span class="sxs-lookup"><span data-stu-id="718b7-103">List connectors</span></span>

<span data-ttu-id="718b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="718b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="718b7-105">Получение списка соединителей.</span><span class="sxs-lookup"><span data-stu-id="718b7-105">Retrieve a list of connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="718b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="718b7-106">Permissions</span></span>
<span data-ttu-id="718b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="718b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="718b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="718b7-109">Permission type</span></span> | <span data-ttu-id="718b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="718b7-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="718b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="718b7-111">Delegated (work or school account)</span></span>| <span data-ttu-id="718b7-112">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="718b7-112">Users.Read.All</span></span> |
|<span data-ttu-id="718b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="718b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="718b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="718b7-114">Not Supported.</span></span>|
|<span data-ttu-id="718b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="718b7-115">Application</span></span>|<span data-ttu-id="718b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="718b7-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="718b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="718b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="718b7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="718b7-118">Optional query parameters</span></span>
<span data-ttu-id="718b7-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="718b7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="718b7-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="718b7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="718b7-121">Исключения</span><span class="sxs-lookup"><span data-stu-id="718b7-121">Exceptions</span></span>
<span data-ttu-id="718b7-122">Некоторые операторы не поддерживаются: `$count`, `$orderby`, `$search`, `$filter`.</span><span class="sxs-lookup"><span data-stu-id="718b7-122">Some operators are not supported: `$count`, `$orderby`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="718b7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="718b7-123">Request headers</span></span>
| <span data-ttu-id="718b7-124">Имя</span><span class="sxs-lookup"><span data-stu-id="718b7-124">Name</span></span>      |<span data-ttu-id="718b7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="718b7-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="718b7-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="718b7-126">Authorization</span></span> | <span data-ttu-id="718b7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="718b7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="718b7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="718b7-129">Request body</span></span>
<span data-ttu-id="718b7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="718b7-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="718b7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="718b7-131">Response</span></span>
<span data-ttu-id="718b7-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Connector](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="718b7-132">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="718b7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="718b7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="718b7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="718b7-134">Request</span></span>
<span data-ttu-id="718b7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="718b7-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="718b7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="718b7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="718b7-137">C#</span><span class="sxs-lookup"><span data-stu-id="718b7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="718b7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="718b7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="718b7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="718b7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="718b7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="718b7-140">Response</span></span>
<span data-ttu-id="718b7-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="718b7-141">The following is an example of the response.</span></span>
><span data-ttu-id="718b7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="718b7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
