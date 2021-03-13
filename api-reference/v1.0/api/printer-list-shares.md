---
title: Список принтераShares для принтера
description: Извлечение списка принтеров, связанных с принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 122de94459a468371012f7480cd153c9f2c05597
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771962"
---
# <a name="list-printershares-for-a-printer"></a><span data-ttu-id="ff504-103">Список принтераShares для принтера</span><span class="sxs-lookup"><span data-stu-id="ff504-103">List printerShares for a printer</span></span>
<span data-ttu-id="ff504-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff504-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="ff504-105">Извлечение списка акций принтера, связанных с [принтером.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="ff504-105">Retrieve a list of printer shares associated with the [printer](../resources/printer.md).</span></span>
><span data-ttu-id="ff504-106">**Примечание:** В настоящее **время поддерживается** только одна доля принтера на принтере.</span><span class="sxs-lookup"><span data-stu-id="ff504-106">**Note:** Currently, only **one** printer share per printer is supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff504-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff504-107">Permissions</span></span>
<span data-ttu-id="ff504-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ff504-110">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="ff504-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="ff504-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff504-111">Permission type</span></span> | <span data-ttu-id="ff504-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff504-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ff504-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff504-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ff504-114">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff504-114">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="ff504-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff504-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff504-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff504-116">Not Supported.</span></span>|
|<span data-ttu-id="ff504-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ff504-117">Application</span></span>| <span data-ttu-id="ff504-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff504-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff504-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff504-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff504-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff504-120">Optional query parameters</span></span>
<span data-ttu-id="ff504-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ff504-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ff504-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ff504-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff504-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff504-123">Request headers</span></span>
|<span data-ttu-id="ff504-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ff504-124">Name</span></span>|<span data-ttu-id="ff504-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ff504-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ff504-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff504-126">Authorization</span></span>|<span data-ttu-id="ff504-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff504-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff504-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff504-129">Request body</span></span>
<span data-ttu-id="ff504-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff504-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff504-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff504-131">Response</span></span>

<span data-ttu-id="ff504-132">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff504-132">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>

><span data-ttu-id="ff504-133">**Примечание.** В ответе не будут содержаться **свойства** по умолчанию **и** возможности.</span><span class="sxs-lookup"><span data-stu-id="ff504-133">**Note**: The response will not contain the **defaults** and **capabilities** properties.</span></span> <span data-ttu-id="ff504-134">Эти свойства можно запрашивать с помощью [запроса Get printerShare.](printerShare-get.md)</span><span class="sxs-lookup"><span data-stu-id="ff504-134">These properties can be queried using a [Get printerShare](printerShare-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="ff504-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="ff504-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ff504-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff504-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ff504-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff504-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/shares
```
# <a name="c"></a>[<span data-ttu-id="ff504-138">C#</span><span class="sxs-lookup"><span data-stu-id="ff504-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff504-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff504-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff504-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff504-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff504-141">Java</span><span class="sxs-lookup"><span data-stu-id="ff504-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ff504-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff504-142">Response</span></span>
<span data-ttu-id="ff504-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ff504-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printerShare)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('2f3453b7-4686-4b5b-9575-4f1e5b909ba7')/shares",
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
  ]
}
```

