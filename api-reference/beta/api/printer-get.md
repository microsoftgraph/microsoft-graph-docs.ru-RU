---
title: Получение принтера
description: Извлечение свойств и связей объекта принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 42804622f94207e304ada3a9538f860415ddbf53
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766254"
---
# <a name="get-printer"></a><span data-ttu-id="ec484-103">Получение принтера</span><span class="sxs-lookup"><span data-stu-id="ec484-103">Get printer</span></span>

<span data-ttu-id="ec484-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec484-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec484-105">Извлечение свойств и связей объекта [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="ec484-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec484-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec484-106">Permissions</span></span>
<span data-ttu-id="ec484-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ec484-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ec484-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="ec484-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="ec484-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ec484-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec484-111">Permission type</span></span> | <span data-ttu-id="ec484-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec484-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ec484-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec484-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ec484-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ec484-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="ec484-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec484-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec484-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec484-116">Not Supported.</span></span>|
|<span data-ttu-id="ec484-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ec484-117">Application</span></span>| <span data-ttu-id="ec484-118">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec484-118">Printer.Read.All, Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec484-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec484-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec484-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec484-120">Optional query parameters</span></span>
<span data-ttu-id="ec484-121">Этот метод поддерживает некоторые параметры запроса OData, включая $select, $expand, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="ec484-121">This method supports some of the OData query parameters including $select, $expand to help customize the response.</span></span> <span data-ttu-id="ec484-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ec484-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="ec484-123">например.</span><span class="sxs-lookup"><span data-stu-id="ec484-123">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
## <a name="request-headers"></a><span data-ttu-id="ec484-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec484-124">Request headers</span></span>
| <span data-ttu-id="ec484-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ec484-125">Name</span></span>      |<span data-ttu-id="ec484-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ec484-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec484-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec484-127">Authorization</span></span> | <span data-ttu-id="ec484-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec484-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec484-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec484-130">Request body</span></span>
<span data-ttu-id="ec484-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec484-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ec484-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec484-132">Response</span></span>
<span data-ttu-id="ec484-133">В случае успешного использования этот метод возвращает код отклика и `200 OK` объект [принтера](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec484-133">If successful, this method returns a `200 OK` response code and a [printer](../resources/printer.md) object in the response body.</span></span>
<span data-ttu-id="ec484-134">По умолчанию ответ не будет содержать [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="ec484-134">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="ec484-135">Чтобы получить **printerCapabilities,** используйте параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="ec484-135">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="example"></a><span data-ttu-id="ec484-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ec484-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec484-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec484-137">Request</span></span>
<span data-ttu-id="ec484-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec484-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec484-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec484-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="ec484-140">C#</span><span class="sxs-lookup"><span data-stu-id="ec484-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec484-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec484-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec484-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec484-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec484-143">Java</span><span class="sxs-lookup"><span data-stu-id="ec484-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ec484-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec484-144">Response</span></span>
<span data-ttu-id="ec484-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec484-145">The following is an example of the response.</span></span>
><span data-ttu-id="ec484-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec484-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "status": {
     "state": "stopped",
    "details": [
      "disconnected"
    ],
    "description": ""
  },
  "defaults": {
    "copiesPerJob": 1,
    "finishings": [
      "none"
    ],
    "mediaColor": "Unknown",
    "mediaType": "stationery",
    "mediaSize": "North America Letter",
    "pagesPerSheet": 1,
    "orientation": "portrait",
    "outputBin": "auto",
    "inputBin": "auto",
    "contentType": "application/oxps",
    "fitPdfToPage": false,
    "multipageLayout": null,
    "colorMode": "color",
    "quality": "medium",
    "duplexMode": "oneSided",
    "dpi": 600,
    "scaling": null
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
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
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

<span data-ttu-id="ec484-148">Ниже приводится пример ответа при использовании $select=id,displayName,capabilities</span><span class="sxs-lookup"><span data-stu-id="ec484-148">The following is an example of the response, when using $select=id,displayName,capabilities</span></span>
><span data-ttu-id="ec484-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec484-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "displayName": "PrinterName",
  "capabilities": {
    "isColorPrintingSupported": true,
    "supportsFitPdfToPage": false,
    "contentTypes": [
      "application/pdf",
      "image/pwg-raster",
      "application/PCLm"
    ],
    "isPageRangeSupported": false,
    "qualities": [
      "medium"
    ],
    "dpis": [
      600
    ],
    "duplexModes": [
      "oneSided",
      "flipOnLongEdge",
      "flipOnShortEdge"
    ],
    "finishings": [
      "none"
    ],
    "mediaTypes": [
      "stationery"
    ],
    "mediaSizes": [
      "North America Letter"
    ],
    "outputBins": [
      "tray-1"
    ],
    "colorModes": [
      "grayscale",
      "color"
    ],
    "inputBins": [
      "tray-1"
    ],
    "collation": true,
    "scalings": [
      "fill"
    ],
    "copiesPerJob": {
      "start": 1,
      "end": 38
    }
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
