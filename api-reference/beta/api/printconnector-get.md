---
title: Получение Принтконнектор
description: Получение свойств и связей объекта Connector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: bd0b111cfe5fb4b74c924db32524ea8d752d8a7f
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896313"
---
# <a name="get-printconnector"></a><span data-ttu-id="0353c-103">Получение Принтконнектор</span><span class="sxs-lookup"><span data-stu-id="0353c-103">Get printConnector</span></span>

<span data-ttu-id="0353c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0353c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0353c-105">Получение свойств и связей объекта **принтконнектор** .</span><span class="sxs-lookup"><span data-stu-id="0353c-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0353c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0353c-106">Permissions</span></span>
<span data-ttu-id="0353c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0353c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0353c-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="0353c-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0353c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0353c-110">Permission type</span></span> | <span data-ttu-id="0353c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0353c-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0353c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0353c-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0353c-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0353c-113">Users.Read.All</span></span> |
|<span data-ttu-id="0353c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0353c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0353c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0353c-115">Not Supported.</span></span>|
|<span data-ttu-id="0353c-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0353c-116">Application</span></span>|<span data-ttu-id="0353c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0353c-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0353c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0353c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0353c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0353c-119">Optional query parameters</span></span>
<span data-ttu-id="0353c-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0353c-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0353c-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0353c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0353c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0353c-122">Request headers</span></span>
| <span data-ttu-id="0353c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0353c-123">Name</span></span>      |<span data-ttu-id="0353c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0353c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0353c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0353c-125">Authorization</span></span> | <span data-ttu-id="0353c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0353c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0353c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0353c-128">Request body</span></span>
<span data-ttu-id="0353c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0353c-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0353c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0353c-130">Response</span></span>
<span data-ttu-id="0353c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтконнектор](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0353c-131">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0353c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0353c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0353c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0353c-133">Request</span></span>
<span data-ttu-id="0353c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0353c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```http
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="0353c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0353c-135">Response</span></span>
<span data-ttu-id="0353c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0353c-136">The following is an example of the response.</span></span>
><span data-ttu-id="0353c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0353c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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