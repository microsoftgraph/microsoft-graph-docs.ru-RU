---
title: Список принтераShares для принтера
description: Извлечение списка принтеров, связанных с принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d719cc04c4b4bc0694f42e80ce7ae317bc8ef104
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956263"
---
# <a name="list-printershares-for-a-printer"></a><span data-ttu-id="c8fae-103">Список принтераShares для принтера</span><span class="sxs-lookup"><span data-stu-id="c8fae-103">List printerShares for a printer</span></span>
<span data-ttu-id="c8fae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8fae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c8fae-105">Извлечение списка акций принтера, связанных с [принтером.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="c8fae-105">Retrieve a list of printer shares associated with the [printer](../resources/printer.md).</span></span>
><span data-ttu-id="c8fae-106">**Примечание:** В настоящее **время поддерживается** только одна доля принтера на принтере.</span><span class="sxs-lookup"><span data-stu-id="c8fae-106">**Note:** Currently, only **one** printer share per printer is supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8fae-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8fae-107">Permissions</span></span>
<span data-ttu-id="c8fae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8fae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c8fae-110">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="c8fae-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="c8fae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8fae-111">Permission type</span></span> | <span data-ttu-id="c8fae-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8fae-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c8fae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8fae-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c8fae-114">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8fae-114">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="c8fae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8fae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8fae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8fae-116">Not Supported.</span></span>|
|<span data-ttu-id="c8fae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8fae-117">Application</span></span>| <span data-ttu-id="c8fae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8fae-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8fae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8fae-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8fae-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8fae-120">Optional query parameters</span></span>
<span data-ttu-id="c8fae-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c8fae-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c8fae-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c8fae-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8fae-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8fae-123">Request headers</span></span>
|<span data-ttu-id="c8fae-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c8fae-124">Name</span></span>|<span data-ttu-id="c8fae-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c8fae-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c8fae-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8fae-126">Authorization</span></span>|<span data-ttu-id="c8fae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8fae-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8fae-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8fae-129">Request body</span></span>
<span data-ttu-id="c8fae-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8fae-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8fae-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8fae-131">Response</span></span>

<span data-ttu-id="c8fae-132">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8fae-132">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>

><span data-ttu-id="c8fae-133">**Примечание.** В ответе не будут содержаться **свойства** по умолчанию **и** возможности.</span><span class="sxs-lookup"><span data-stu-id="c8fae-133">**Note**: The response will not contain the **defaults** and **capabilities** properties.</span></span> <span data-ttu-id="c8fae-134">Эти свойства можно запрашивать с помощью [запроса Get printerShare.](printerShare-get.md)</span><span class="sxs-lookup"><span data-stu-id="c8fae-134">These properties can be queried using a [Get printerShare](printerShare-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="c8fae-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8fae-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8fae-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8fae-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c8fae-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8fae-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printershare_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/shares
```
# <a name="c"></a>[<span data-ttu-id="c8fae-138">C#</span><span class="sxs-lookup"><span data-stu-id="c8fae-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printershare-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8fae-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8fae-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printershare-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8fae-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8fae-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printershare-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8fae-141">Java</span><span class="sxs-lookup"><span data-stu-id="c8fae-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printershare-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c8fae-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8fae-142">Response</span></span>
<span data-ttu-id="c8fae-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8fae-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

