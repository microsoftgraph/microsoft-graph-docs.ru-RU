---
title: Получение printerShare
description: Извлечение свойств и связей совместной работы принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3e5bc385fb6e928ba82bb36660bb8af7bf794034
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518053"
---
# <a name="get-printershare"></a><span data-ttu-id="d0b9a-103">Получение printerShare</span><span class="sxs-lookup"><span data-stu-id="d0b9a-103">Get printerShare</span></span>
<span data-ttu-id="d0b9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0b9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d0b9a-105">Извлечение свойств и связей совместной работы принтера.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0b9a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b9a-106">Permissions</span></span>
<span data-ttu-id="d0b9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0b9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d0b9a-109">Помимо следующих разрешений, клиент или клиент приложения должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d0b9a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b9a-110">Permission type</span></span> | <span data-ttu-id="d0b9a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0b9a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d0b9a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0b9a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d0b9a-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0b9a-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="d0b9a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0b9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0b9a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-115">Not Supported.</span></span>|
|<span data-ttu-id="d0b9a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0b9a-116">Application</span></span>|<span data-ttu-id="d0b9a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0b9a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0b9a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}
GET /print/printers/{printerId}/shares/{printerShareId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0b9a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d0b9a-119">Optional query parameters</span></span>
<span data-ttu-id="d0b9a-120">Этот метод поддерживает некоторые параметры запроса OData, включая и , чтобы помочь `$select` `$expand` настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-120">This method supports some of the OData query parameters, including `$select` and `$expand`, to help customize the response.</span></span> <span data-ttu-id="d0b9a-121">Например:</span><span class="sxs-lookup"><span data-stu-id="d0b9a-121">For example:</span></span> 

<span data-ttu-id="d0b9a-122">например.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
<span data-ttu-id="d0b9a-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d0b9a-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="d0b9a-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="d0b9a-124">Exceptions</span></span>
* <span data-ttu-id="d0b9a-125">Оператор `$count` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-125">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0b9a-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0b9a-126">Request headers</span></span>
|<span data-ttu-id="d0b9a-127">Имя</span><span class="sxs-lookup"><span data-stu-id="d0b9a-127">Name</span></span>|<span data-ttu-id="d0b9a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d0b9a-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d0b9a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0b9a-129">Authorization</span></span>|<span data-ttu-id="d0b9a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0b9a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0b9a-132">Request body</span></span>
<span data-ttu-id="d0b9a-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d0b9a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b9a-134">Response</span></span>
<span data-ttu-id="d0b9a-135">В случае успешного использования этот метод возвращает код отклика и `200 OK` объект [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-135">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="d0b9a-136">По умолчанию ответ не будет содержать [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="d0b9a-136">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="d0b9a-137">Чтобы получить **printerCapabilities,** используйте параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-137">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="response"></a><span data-ttu-id="d0b9a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b9a-138">Response</span></span>

<span data-ttu-id="d0b9a-139">В случае успешного использования этот метод возвращает код отклика и `200 OK` объект [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-139">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0b9a-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="d0b9a-140">Examples</span></span>

### <a name="example-1-get-a-printershare"></a><span data-ttu-id="d0b9a-141">Пример 1. Получить принтерShare</span><span class="sxs-lookup"><span data-stu-id="d0b9a-141">Example 1: Get a printerShare</span></span>

#### <a name="request"></a><span data-ttu-id="d0b9a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0b9a-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```

#### <a name="response"></a><span data-ttu-id="d0b9a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b9a-143">Response</span></span>
<span data-ttu-id="d0b9a-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "PrinterShare Name",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
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
    "latitude": 47.6450,
    "longitude": -122.1409,
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

### <a name="example-2-get-a-printershare-and-its-capabilities"></a><span data-ttu-id="d0b9a-145">Пример 2. Получить принтерShare и его возможности</span><span class="sxs-lookup"><span data-stu-id="d0b9a-145">Example 2: Get a printerShare and its capabilities</span></span>

#### <a name="request"></a><span data-ttu-id="d0b9a-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0b9a-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printershare_capabilities"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}?$select=id,displayName,capabilities
```

#### <a name="response"></a><span data-ttu-id="d0b9a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b9a-147">Response</span></span>

<span data-ttu-id="d0b9a-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0b9a-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
--> 
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "PrinterShare Name",
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
