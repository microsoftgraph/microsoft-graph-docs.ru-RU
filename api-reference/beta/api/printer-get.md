---
title: Получение принтера
description: Получение свойств и связей объекта Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 800dd2748cdd2a3866973670394f65f80f28a424
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896284"
---
# <a name="get-printer"></a><span data-ttu-id="42f3c-103">Получение принтера</span><span class="sxs-lookup"><span data-stu-id="42f3c-103">Get printer</span></span>

<span data-ttu-id="42f3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42f3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42f3c-105">Получение свойств и связей объекта [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="42f3c-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42f3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42f3c-106">Permissions</span></span>
<span data-ttu-id="42f3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="42f3c-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="42f3c-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="42f3c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42f3c-110">Permission type</span></span> | <span data-ttu-id="42f3c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42f3c-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="42f3c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42f3c-112">Delegated (work or school account)</span></span>| <span data-ttu-id="42f3c-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="42f3c-113">Users.Read.All</span></span> |
|<span data-ttu-id="42f3c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42f3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42f3c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f3c-115">Not Supported.</span></span>|
|<span data-ttu-id="42f3c-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="42f3c-116">Application</span></span>|<span data-ttu-id="42f3c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f3c-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42f3c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42f3c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/printerShares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42f3c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42f3c-119">Optional query parameters</span></span>
<span data-ttu-id="42f3c-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="42f3c-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="42f3c-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="42f3c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="42f3c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42f3c-122">Request headers</span></span>
| <span data-ttu-id="42f3c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="42f3c-123">Name</span></span>      |<span data-ttu-id="42f3c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="42f3c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42f3c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42f3c-125">Authorization</span></span> | <span data-ttu-id="42f3c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42f3c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42f3c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42f3c-128">Request body</span></span>
<span data-ttu-id="42f3c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42f3c-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="42f3c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="42f3c-130">Response</span></span>
<span data-ttu-id="42f3c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42f3c-131">If successful, this method returns a `200 OK` response code and [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42f3c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="42f3c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42f3c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="42f3c-133">Request</span></span>
<span data-ttu-id="42f3c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42f3c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/{id}
```
##### <a name="response"></a><span data-ttu-id="42f3c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="42f3c-135">Response</span></span>
<span data-ttu-id="42f3c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="42f3c-136">The following is an example of the response.</span></span>
><span data-ttu-id="42f3c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42f3c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "registeredBy": {},
  "status": {
    "processingState": "stopped",
    "processingStateReasons": ["disconnected"],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->