---
title: Перечисление общих ресурсов
description: Извлечение списка акций принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 52fa7ceebdfc425cff29c6f9a29a91a4cf796478
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517523"
---
# <a name="list-shares"></a><span data-ttu-id="53951-103">Перечисление общих ресурсов</span><span class="sxs-lookup"><span data-stu-id="53951-103">List shares</span></span>
<span data-ttu-id="53951-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53951-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="53951-105">Извлечение списка **printerShares**.</span><span class="sxs-lookup"><span data-stu-id="53951-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="53951-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53951-106">Permissions</span></span>
<span data-ttu-id="53951-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="53951-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="53951-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="53951-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53951-110">Permission type</span></span> | <span data-ttu-id="53951-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53951-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="53951-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53951-112">Delegated (work or school account)</span></span>| <span data-ttu-id="53951-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53951-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="53951-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53951-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53951-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53951-115">Not Supported.</span></span>|
|<span data-ttu-id="53951-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="53951-116">Application</span></span>|<span data-ttu-id="53951-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53951-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53951-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53951-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53951-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53951-119">Optional query parameters</span></span>
<span data-ttu-id="53951-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="53951-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="53951-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="53951-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="53951-122">Чтобы увидеть список возможностей каждой доли принтера, включайте параметр необязательный `$select=capabilities` запрос.</span><span class="sxs-lookup"><span data-stu-id="53951-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="53951-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="53951-123">Exceptions</span></span>
<span data-ttu-id="53951-124">Некоторые операторы не поддерживаются: `$count` , `$orderby` `$search` .</span><span class="sxs-lookup"><span data-stu-id="53951-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53951-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53951-125">Request headers</span></span>
|<span data-ttu-id="53951-126">Имя</span><span class="sxs-lookup"><span data-stu-id="53951-126">Name</span></span>|<span data-ttu-id="53951-127">Описание</span><span class="sxs-lookup"><span data-stu-id="53951-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53951-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53951-128">Authorization</span></span>|<span data-ttu-id="53951-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53951-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53951-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53951-131">Request body</span></span>
<span data-ttu-id="53951-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53951-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53951-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="53951-133">Response</span></span>

<span data-ttu-id="53951-134">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53951-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>

><span data-ttu-id="53951-135">**Примечание.** В ответе не будут содержаться **свойства** по умолчанию **и** возможности.</span><span class="sxs-lookup"><span data-stu-id="53951-135">**Note**: The response will not contain the **defaults** and **capabilities** properties.</span></span> <span data-ttu-id="53951-136">Эти свойства можно получить с помощью [запроса Get printerShare.](printershare-get.md)</span><span class="sxs-lookup"><span data-stu-id="53951-136">You can get these properties via a [Get printerShare](printershare-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="53951-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="53951-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53951-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="53951-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares
```


### <a name="response"></a><span data-ttu-id="53951-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="53951-139">Response</span></span>
<span data-ttu-id="53951-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="53951-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares",
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

