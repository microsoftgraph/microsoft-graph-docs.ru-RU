---
title: Перечисление принтеров
description: Извлечение списка принтеров, зарегистрированных в клиенте.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ff93eb5c598458c57126f0e8edda2a4f440dfc65
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517529"
---
# <a name="list-printers"></a><span data-ttu-id="5ecf4-103">Перечисление принтеров</span><span class="sxs-lookup"><span data-stu-id="5ecf4-103">List printers</span></span>
<span data-ttu-id="5ecf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ecf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5ecf4-105">Извлечение списка **принтеров,** зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-105">Retrieve the list of **printers** that are registered in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ecf4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ecf4-106">Permissions</span></span>
<span data-ttu-id="5ecf4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ecf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5ecf4-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="5ecf4-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="5ecf4-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="5ecf4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ecf4-111">Permission type</span></span> | <span data-ttu-id="5ecf4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ecf4-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5ecf4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ecf4-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5ecf4-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="5ecf4-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="5ecf4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ecf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ecf4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-116">Not Supported.</span></span>|
|<span data-ttu-id="5ecf4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5ecf4-117">Application</span></span>| <span data-ttu-id="5ecf4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ecf4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ecf4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ecf4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ecf4-120">Optional query parameters</span></span>
<span data-ttu-id="5ecf4-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5ecf4-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5ecf4-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="5ecf4-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="5ecf4-123">Exceptions</span></span>
* <span data-ttu-id="5ecf4-124">Свойство навигации поддерживается и поддерживается `$expand` `select` `share` операторами, но не `jobs` для .</span><span class="sxs-lookup"><span data-stu-id="5ecf4-124">The `$expand` and `select` operators are supported for the `share` navigation property, but not for `jobs`.</span></span>
* <span data-ttu-id="5ecf4-125">Некоторые операторы не поддерживаются: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="5ecf4-125">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ecf4-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ecf4-126">Request headers</span></span>
|<span data-ttu-id="5ecf4-127">Имя</span><span class="sxs-lookup"><span data-stu-id="5ecf4-127">Name</span></span>|<span data-ttu-id="5ecf4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5ecf4-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ecf4-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ecf4-129">Authorization</span></span>|<span data-ttu-id="5ecf4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ecf4-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ecf4-132">Request body</span></span>
<span data-ttu-id="5ecf4-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ecf4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ecf4-134">Response</span></span>

<span data-ttu-id="5ecf4-135">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` принтера в тексте [](../resources/printer.md) отклика.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-135">If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.</span></span>

><span data-ttu-id="5ecf4-136">**Примечание.** В ответе не будут содержаться свойства "по умолчанию" и "возможности".</span><span class="sxs-lookup"><span data-stu-id="5ecf4-136">**Note**: The response will not contain 'defaults' and 'capabilities' properties.</span></span> <span data-ttu-id="5ecf4-137">Эти свойства можно запрашивать с помощью [запроса Get Printer.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="5ecf4-137">These properties can be queried using [Get Printer](printer-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="5ecf4-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="5ecf4-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ecf4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ecf4-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printer"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers
```


### <a name="response"></a><span data-ttu-id="5ecf4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ecf4-140">Response</span></span>
<span data-ttu-id="5ecf4-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5ecf4-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers",
  "value": [
    {
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
  ]
}
```

