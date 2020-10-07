---
title: Получение принтера
description: Получение свойств и связей объекта Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1a08f664d4c3e92ed549a2c46b502acb6543985c
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372994"
---
# <a name="get-printer"></a><span data-ttu-id="a9921-103">Получение принтера</span><span class="sxs-lookup"><span data-stu-id="a9921-103">Get printer</span></span>

<span data-ttu-id="a9921-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9921-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9921-105">Получение свойств и связей объекта [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="a9921-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9921-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9921-106">Permissions</span></span>
<span data-ttu-id="a9921-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a9921-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a9921-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a9921-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="a9921-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a9921-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9921-111">Permission type</span></span> | <span data-ttu-id="a9921-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9921-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a9921-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9921-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a9921-114">Printer. Read. ALL, Printer. ReadWrite. ALL, Printer. FullControl. ALL.</span><span class="sxs-lookup"><span data-stu-id="a9921-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a9921-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9921-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9921-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9921-116">Not Supported.</span></span>|
|<span data-ttu-id="a9921-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a9921-117">Application</span></span>| <span data-ttu-id="a9921-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9921-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9921-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9921-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9921-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a9921-120">Optional query parameters</span></span>
<span data-ttu-id="a9921-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a9921-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a9921-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a9921-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9921-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9921-123">Request headers</span></span>
| <span data-ttu-id="a9921-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a9921-124">Name</span></span>      |<span data-ttu-id="a9921-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a9921-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9921-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9921-126">Authorization</span></span> | <span data-ttu-id="a9921-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9921-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9921-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9921-129">Request body</span></span>
<span data-ttu-id="a9921-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9921-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a9921-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9921-131">Response</span></span>
<span data-ttu-id="a9921-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9921-132">If successful, this method returns a `200 OK` response code and [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9921-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a9921-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9921-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9921-134">Request</span></span>
<span data-ttu-id="a9921-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9921-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9921-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9921-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="a9921-137">C#</span><span class="sxs-lookup"><span data-stu-id="a9921-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9921-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9921-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9921-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9921-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a9921-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9921-140">Response</span></span>
<span data-ttu-id="a9921-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a9921-141">The following is an example of the response.</span></span>
><span data-ttu-id="a9921-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9921-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
