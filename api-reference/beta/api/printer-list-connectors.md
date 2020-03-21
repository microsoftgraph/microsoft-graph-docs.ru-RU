---
title: Список соединителей
description: Получение списка соединителей, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 162e6a186ac85ff3c7b2dfb28dccdb53089856fb
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896254"
---
# <a name="list-connectors"></a><span data-ttu-id="13630-103">Список соединителей</span><span class="sxs-lookup"><span data-stu-id="13630-103">List connectors</span></span>

<span data-ttu-id="13630-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13630-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13630-105">Получение списка **соединителей** , связанных с [принтером](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="13630-105">Retrieve a list of **connectors** associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13630-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13630-106">Permissions</span></span>
<span data-ttu-id="13630-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="13630-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="13630-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="13630-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13630-110">Permission type</span></span> | <span data-ttu-id="13630-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13630-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="13630-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13630-112">Delegated (work or school account)</span></span>| <span data-ttu-id="13630-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="13630-113">Users.Read.All</span></span> |
|<span data-ttu-id="13630-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13630-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13630-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13630-115">Not Supported.</span></span>|
|<span data-ttu-id="13630-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="13630-116">Application</span></span>|<span data-ttu-id="13630-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13630-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13630-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13630-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/connectors
```

## <a name="request-headers"></a><span data-ttu-id="13630-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13630-119">Request headers</span></span>
| <span data-ttu-id="13630-120">Имя</span><span class="sxs-lookup"><span data-stu-id="13630-120">Name</span></span>      |<span data-ttu-id="13630-121">Описание</span><span class="sxs-lookup"><span data-stu-id="13630-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13630-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13630-122">Authorization</span></span> | <span data-ttu-id="13630-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13630-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13630-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13630-125">Request body</span></span>
<span data-ttu-id="13630-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13630-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="13630-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="13630-127">Response</span></span>
<span data-ttu-id="13630-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтконнектор](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13630-128">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13630-129">Пример</span><span class="sxs-lookup"><span data-stu-id="13630-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13630-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="13630-130">Request</span></span>
<span data-ttu-id="13630-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13630-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/{id}/connectors
```
##### <a name="response"></a><span data-ttu-id="13630-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="13630-132">Response</span></span>
<span data-ttu-id="13630-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13630-133">The following is an example of the response.</span></span>
><span data-ttu-id="13630-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13630-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1373

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printConnector)",
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