---
title: Получить принтеры
description: Извлечение списка принтеров, зарегистрированных в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 38f742b4013f01b150ee5b653d341dd2e8ca5991
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766513"
---
# <a name="list-printers"></a><span data-ttu-id="c0802-103">Перечисление принтеров</span><span class="sxs-lookup"><span data-stu-id="c0802-103">List printers</span></span>

<span data-ttu-id="c0802-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0802-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0802-105">Извлечение списка **принтеров,** зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c0802-105">Retrieve the list of **printers** that are registered in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0802-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0802-106">Permissions</span></span>
<span data-ttu-id="c0802-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c0802-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c0802-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c0802-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="c0802-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c0802-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0802-111">Permission type</span></span> | <span data-ttu-id="c0802-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0802-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c0802-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0802-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c0802-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="c0802-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="c0802-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0802-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0802-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0802-116">Not Supported.</span></span>|
|<span data-ttu-id="c0802-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c0802-117">Application</span></span>| <span data-ttu-id="c0802-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0802-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0802-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0802-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0802-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0802-120">Optional query parameters</span></span>
<span data-ttu-id="c0802-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c0802-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c0802-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c0802-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="c0802-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c0802-123">Exceptions</span></span>
* <span data-ttu-id="c0802-124">Свойство навигации поддерживается и поддерживается `$expand` `select` `share` операторами, но не `jobs` для .</span><span class="sxs-lookup"><span data-stu-id="c0802-124">The `$expand` and `select` operators are supported for the `share` navigation property, but not for `jobs`.</span></span>
* <span data-ttu-id="c0802-125">Некоторые операторы не поддерживаются: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="c0802-125">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0802-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0802-126">Request headers</span></span>
| <span data-ttu-id="c0802-127">Имя</span><span class="sxs-lookup"><span data-stu-id="c0802-127">Name</span></span>      |<span data-ttu-id="c0802-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c0802-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0802-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0802-129">Authorization</span></span> | <span data-ttu-id="c0802-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0802-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0802-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0802-132">Request body</span></span>
<span data-ttu-id="c0802-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0802-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c0802-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0802-134">Response</span></span>
<span data-ttu-id="c0802-135">В случае успешного использования этот метод возвращает код отклика и коллекцию объектов `200 OK` принтера в тексте [](../resources/printer.md) отклика.</span><span class="sxs-lookup"><span data-stu-id="c0802-135">If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0802-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c0802-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0802-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0802-137">Request</span></span>
<span data-ttu-id="c0802-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0802-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0802-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0802-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers
```
# <a name="c"></a>[<span data-ttu-id="c0802-140">C#</span><span class="sxs-lookup"><span data-stu-id="c0802-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0802-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0802-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0802-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0802-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0802-143">Java</span><span class="sxs-lookup"><span data-stu-id="c0802-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0802-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0802-144">Response</span></span>
<span data-ttu-id="c0802-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0802-145">The following is an example of the response.</span></span>
><span data-ttu-id="c0802-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0802-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List printers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
