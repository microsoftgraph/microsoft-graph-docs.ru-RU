---
title: Получение принтеров
description: Получение списка принтеров, зарегистрированных в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 33171e0878c05d044a1f0d4dbde181600e0605ed
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812536"
---
# <a name="list-printers"></a><span data-ttu-id="6564e-103">Список принтеров</span><span class="sxs-lookup"><span data-stu-id="6564e-103">List printers</span></span>

<span data-ttu-id="6564e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6564e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6564e-105">Получение списка **принтеров** , зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6564e-105">Retrieve the list of **printers** that are registered in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="6564e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6564e-106">Permissions</span></span>
<span data-ttu-id="6564e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6564e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6564e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6564e-109">Permission type</span></span> | <span data-ttu-id="6564e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6564e-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6564e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6564e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="6564e-112">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6564e-112">Users.Read.All</span></span> |
|<span data-ttu-id="6564e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6564e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6564e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6564e-114">Not Supported.</span></span>|
|<span data-ttu-id="6564e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6564e-115">Application</span></span>|<span data-ttu-id="6564e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6564e-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6564e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6564e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6564e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6564e-118">Optional query parameters</span></span>
<span data-ttu-id="6564e-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6564e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6564e-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6564e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="6564e-121">Исключения</span><span class="sxs-lookup"><span data-stu-id="6564e-121">Exceptions</span></span>
* <span data-ttu-id="6564e-122">Операторы `$expand` and `select` поддерживаются для свойства `share` навигации, но не для `jobs`.</span><span class="sxs-lookup"><span data-stu-id="6564e-122">The `$expand` and `select` operators are supported for the `share` navigation property, but not for `jobs`.</span></span>
* <span data-ttu-id="6564e-123">Некоторые операторы не поддерживаются: `$count`, `$orderby`, `$search`.</span><span class="sxs-lookup"><span data-stu-id="6564e-123">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6564e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6564e-124">Request headers</span></span>
| <span data-ttu-id="6564e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6564e-125">Name</span></span>      |<span data-ttu-id="6564e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6564e-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6564e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6564e-127">Authorization</span></span> | <span data-ttu-id="6564e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6564e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6564e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6564e-130">Request body</span></span>
<span data-ttu-id="6564e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6564e-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6564e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6564e-132">Response</span></span>
<span data-ttu-id="6564e-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6564e-133">If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6564e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6564e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6564e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6564e-135">Request</span></span>
<span data-ttu-id="6564e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6564e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6564e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6564e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers
```
# <a name="c"></a>[<span data-ttu-id="6564e-138">C#</span><span class="sxs-lookup"><span data-stu-id="6564e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6564e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6564e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6564e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6564e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6564e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6564e-141">Response</span></span>
<span data-ttu-id="6564e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6564e-142">The following is an example of the response.</span></span>
><span data-ttu-id="6564e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6564e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
