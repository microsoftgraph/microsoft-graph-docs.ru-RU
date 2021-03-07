---
title: Получение принтера
description: Извлечение свойств и связей объекта принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7dd7cf1c261565407962f5b7034a469dd7aff4e8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517936"
---
# <a name="get-printer"></a><span data-ttu-id="2b468-103">Получение принтера</span><span class="sxs-lookup"><span data-stu-id="2b468-103">Get printer</span></span>
<span data-ttu-id="2b468-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b468-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2b468-105">Извлечение свойств и связей объекта [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="2b468-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b468-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b468-106">Permissions</span></span>
<span data-ttu-id="2b468-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b468-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2b468-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2b468-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="2b468-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="2b468-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2b468-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b468-111">Permission type</span></span> | <span data-ttu-id="2b468-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b468-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2b468-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b468-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2b468-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2b468-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="2b468-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b468-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b468-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b468-116">Not Supported.</span></span>|
|<span data-ttu-id="2b468-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b468-117">Application</span></span>| <span data-ttu-id="2b468-118">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b468-118">Printer.Read.All, Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b468-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b468-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b468-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b468-120">Optional query parameters</span></span>
<span data-ttu-id="2b468-121">Этот метод поддерживает некоторые параметры запроса OData, включая и , чтобы помочь `$select` `$expand` настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="2b468-121">This method supports some of the OData query parameters, including `$select` and `$expand`, to help customize the response.</span></span> <span data-ttu-id="2b468-122">Например:</span><span class="sxs-lookup"><span data-stu-id="2b468-122">For example:</span></span>

```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
<span data-ttu-id="2b468-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2b468-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b468-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b468-124">Request headers</span></span>
|<span data-ttu-id="2b468-125">Имя</span><span class="sxs-lookup"><span data-stu-id="2b468-125">Name</span></span>|<span data-ttu-id="2b468-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2b468-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2b468-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b468-127">Authorization</span></span>|<span data-ttu-id="2b468-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b468-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b468-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b468-130">Request body</span></span>
<span data-ttu-id="2b468-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b468-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b468-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b468-132">Response</span></span>
<span data-ttu-id="2b468-133">В случае успешного использования этот метод возвращает код отклика и `200 OK` объект [принтера](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b468-133">If successful, this method returns a `200 OK` response code and a [printer](../resources/printer.md) object in the response body.</span></span>
<span data-ttu-id="2b468-134">По умолчанию ответ не будет содержать [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="2b468-134">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="2b468-135">Чтобы получить **printerCapabilities,** используйте параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="2b468-135">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="examples"></a><span data-ttu-id="2b468-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b468-136">Examples</span></span>

### <a name="example-1-get-a-printer"></a><span data-ttu-id="2b468-137">Пример 1. Получить принтер</span><span class="sxs-lookup"><span data-stu-id="2b468-137">Example 1: Get a printer</span></span>

#### <a name="request"></a><span data-ttu-id="2b468-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b468-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printer"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}
```

#### <a name="response"></a><span data-ttu-id="2b468-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b468-139">Response</span></span>
<span data-ttu-id="2b468-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b468-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
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

### <a name="example-2-get-a-printer-and-its-capabilities"></a><span data-ttu-id="2b468-141">Пример 2. Получить принтер и его возможности</span><span class="sxs-lookup"><span data-stu-id="2b468-141">Example 2: Get a printer and its capabilities</span></span>

#### <a name="request"></a><span data-ttu-id="2b468-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b468-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printer_capabilities"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}?$select=id,displayName,capabilities
```

#### <a name="response"></a><span data-ttu-id="2b468-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b468-143">Response</span></span>

<span data-ttu-id="2b468-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b468-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
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

