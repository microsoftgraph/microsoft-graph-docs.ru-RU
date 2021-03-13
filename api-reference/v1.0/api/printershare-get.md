---
title: Получение printerShare
description: Извлечение свойств и связей совместной работы принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e9a16d9d615b780d921ff49291d6b15edda2ed3f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771612"
---
# <a name="get-printershare"></a><span data-ttu-id="93b2a-103">Получение printerShare</span><span class="sxs-lookup"><span data-stu-id="93b2a-103">Get printerShare</span></span>
<span data-ttu-id="93b2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93b2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="93b2a-105">Извлечение свойств и связей совместной работы принтера.</span><span class="sxs-lookup"><span data-stu-id="93b2a-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="93b2a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93b2a-106">Permissions</span></span>
<span data-ttu-id="93b2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93b2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="93b2a-109">Помимо следующих разрешений, клиент или клиент приложения должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="93b2a-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="93b2a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93b2a-110">Permission type</span></span> | <span data-ttu-id="93b2a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93b2a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="93b2a-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93b2a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="93b2a-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93b2a-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="93b2a-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93b2a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93b2a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93b2a-115">Not Supported.</span></span>|
|<span data-ttu-id="93b2a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="93b2a-116">Application</span></span>|<span data-ttu-id="93b2a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93b2a-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93b2a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93b2a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}
GET /print/printers/{printerId}/shares/{printerShareId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93b2a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93b2a-119">Optional query parameters</span></span>
<span data-ttu-id="93b2a-120">Этот метод поддерживает некоторые параметры запроса OData, включая и , чтобы помочь `$select` `$expand` настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="93b2a-120">This method supports some of the OData query parameters, including `$select` and `$expand`, to help customize the response.</span></span> <span data-ttu-id="93b2a-121">Например:</span><span class="sxs-lookup"><span data-stu-id="93b2a-121">For example:</span></span> 

<span data-ttu-id="93b2a-122">например.</span><span class="sxs-lookup"><span data-stu-id="93b2a-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
<span data-ttu-id="93b2a-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="93b2a-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="93b2a-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="93b2a-124">Exceptions</span></span>
* <span data-ttu-id="93b2a-125">Оператор `$count` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93b2a-125">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93b2a-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93b2a-126">Request headers</span></span>
|<span data-ttu-id="93b2a-127">Имя</span><span class="sxs-lookup"><span data-stu-id="93b2a-127">Name</span></span>|<span data-ttu-id="93b2a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="93b2a-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="93b2a-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93b2a-129">Authorization</span></span>|<span data-ttu-id="93b2a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93b2a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93b2a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93b2a-132">Request body</span></span>
<span data-ttu-id="93b2a-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93b2a-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="93b2a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="93b2a-134">Response</span></span>
<span data-ttu-id="93b2a-135">В случае успешного использования этот метод возвращает код отклика и `200 OK` объект [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93b2a-135">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="93b2a-136">По умолчанию ответ не будет содержать [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="93b2a-136">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="93b2a-137">Чтобы получить **printerCapabilities,** используйте параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="93b2a-137">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="response"></a><span data-ttu-id="93b2a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="93b2a-138">Response</span></span>

<span data-ttu-id="93b2a-139">В случае успешного использования этот метод возвращает код отклика и `200 OK` объект [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93b2a-139">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93b2a-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="93b2a-140">Examples</span></span>

### <a name="example-1-get-a-printershare"></a><span data-ttu-id="93b2a-141">Пример 1. Получить принтерShare</span><span class="sxs-lookup"><span data-stu-id="93b2a-141">Example 1: Get a printerShare</span></span>

#### <a name="request"></a><span data-ttu-id="93b2a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="93b2a-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="93b2a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="93b2a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```
# <a name="c"></a>[<span data-ttu-id="93b2a-144">C#</span><span class="sxs-lookup"><span data-stu-id="93b2a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93b2a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93b2a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93b2a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93b2a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93b2a-147">Java</span><span class="sxs-lookup"><span data-stu-id="93b2a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93b2a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="93b2a-148">Response</span></span>
<span data-ttu-id="93b2a-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="93b2a-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-a-printershare-and-its-capabilities"></a><span data-ttu-id="93b2a-150">Пример 2. Получить принтерShare и его возможности</span><span class="sxs-lookup"><span data-stu-id="93b2a-150">Example 2: Get a printerShare and its capabilities</span></span>

#### <a name="request"></a><span data-ttu-id="93b2a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="93b2a-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="93b2a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="93b2a-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare_capabilities"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}?$select=id,displayName,capabilities
```
# <a name="c"></a>[<span data-ttu-id="93b2a-153">C#</span><span class="sxs-lookup"><span data-stu-id="93b2a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-capabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93b2a-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93b2a-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-capabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93b2a-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93b2a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-capabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93b2a-156">Java</span><span class="sxs-lookup"><span data-stu-id="93b2a-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-capabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="93b2a-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="93b2a-157">Response</span></span>

<span data-ttu-id="93b2a-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="93b2a-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
