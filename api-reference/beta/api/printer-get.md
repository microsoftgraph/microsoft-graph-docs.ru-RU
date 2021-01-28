---
title: Получение принтера
description: Извлечение свойств и связей объекта принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bfd3f6e71e8fd56c630cfcaa5b56cc32eff4e148
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034060"
---
# <a name="get-printer"></a><span data-ttu-id="f805b-103">Получение принтера</span><span class="sxs-lookup"><span data-stu-id="f805b-103">Get printer</span></span>

<span data-ttu-id="f805b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f805b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f805b-105">Извлечение свойств и связей объекта [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="f805b-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f805b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f805b-106">Permissions</span></span>
<span data-ttu-id="f805b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f805b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f805b-109">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть активная подписка универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="f805b-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="f805b-110">Пользователь, выписав его, должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="f805b-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f805b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f805b-111">Permission type</span></span> | <span data-ttu-id="f805b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f805b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f805b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f805b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f805b-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f805b-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="f805b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f805b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f805b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f805b-116">Not Supported.</span></span>|
|<span data-ttu-id="f805b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f805b-117">Application</span></span>| <span data-ttu-id="f805b-118">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f805b-118">Printer.Read.All, Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f805b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f805b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f805b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f805b-120">Optional query parameters</span></span>
<span data-ttu-id="f805b-121">Этот метод поддерживает некоторые параметры запроса OData, в том числе $select, $expand для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f805b-121">This method supports some of the OData query parameters including $select, $expand to help customize the response.</span></span> <span data-ttu-id="f805b-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f805b-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="f805b-123">например,</span><span class="sxs-lookup"><span data-stu-id="f805b-123">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
## <a name="request-headers"></a><span data-ttu-id="f805b-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f805b-124">Request headers</span></span>
| <span data-ttu-id="f805b-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f805b-125">Name</span></span>      |<span data-ttu-id="f805b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f805b-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f805b-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f805b-127">Authorization</span></span> | <span data-ttu-id="f805b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f805b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f805b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f805b-130">Request body</span></span>
<span data-ttu-id="f805b-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f805b-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f805b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f805b-132">Response</span></span>
<span data-ttu-id="f805b-133">В случае успеха этот метод возвращает код отклика и `200 OK` [объект](../resources/printer.md) принтера в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f805b-133">If successful, this method returns a `200 OK` response code and a [printer](../resources/printer.md) object in the response body.</span></span>
<span data-ttu-id="f805b-134">По умолчанию отклик не будет содержать [printerCapabilities.](../resources/printerCapabilities.md)</span><span class="sxs-lookup"><span data-stu-id="f805b-134">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="f805b-135">Чтобы получить **printerCapabilities,** используйте параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="f805b-135">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="example"></a><span data-ttu-id="f805b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f805b-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="f805b-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f805b-137">Request</span></span>
<span data-ttu-id="f805b-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f805b-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f805b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f805b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="f805b-140">C#</span><span class="sxs-lookup"><span data-stu-id="f805b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f805b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f805b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f805b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f805b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f805b-143">Java</span><span class="sxs-lookup"><span data-stu-id="f805b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f805b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f805b-144">Response</span></span>
<span data-ttu-id="f805b-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f805b-145">The following is an example of the response.</span></span>
><span data-ttu-id="f805b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f805b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="f805b-148">Ниже приводится пример ответа при использовании $select=id,displayName,capabilities</span><span class="sxs-lookup"><span data-stu-id="f805b-148">The following is an example of the response, when using $select=id,displayName,capabilities</span></span>
><span data-ttu-id="f805b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f805b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
