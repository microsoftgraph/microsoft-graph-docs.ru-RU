---
title: Получение принтеров
description: Получение списка принтеров, зарегистрированных в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6e50017daad5734f85fa7c193d80a8e5a82cec54
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373939"
---
# <a name="list-printers"></a><span data-ttu-id="8a6aa-103">Перечисление принтеров</span><span class="sxs-lookup"><span data-stu-id="8a6aa-103">List printers</span></span>

<span data-ttu-id="8a6aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a6aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a6aa-105">Получение списка **принтеров** , зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-105">Retrieve the list of **printers** that are registered in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a6aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a6aa-106">Permissions</span></span>
<span data-ttu-id="8a6aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a6aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8a6aa-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="8a6aa-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="8a6aa-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="8a6aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a6aa-111">Permission type</span></span> | <span data-ttu-id="8a6aa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a6aa-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8a6aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a6aa-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8a6aa-114">Printer. Read. ALL, Printer. ReadWrite. ALL, Printer. FullControl. ALL.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="8a6aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a6aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a6aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-116">Not Supported.</span></span>|
|<span data-ttu-id="8a6aa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8a6aa-117">Application</span></span>| <span data-ttu-id="8a6aa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a6aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a6aa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a6aa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8a6aa-120">Optional query parameters</span></span>
<span data-ttu-id="8a6aa-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8a6aa-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8a6aa-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="8a6aa-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="8a6aa-123">Exceptions</span></span>
* <span data-ttu-id="8a6aa-124">`$expand`Операторы and `select` поддерживаются для `share` Свойства навигации, но не для `jobs` .</span><span class="sxs-lookup"><span data-stu-id="8a6aa-124">The `$expand` and `select` operators are supported for the `share` navigation property, but not for `jobs`.</span></span>
* <span data-ttu-id="8a6aa-125">Некоторые операторы не поддерживаются: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="8a6aa-125">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a6aa-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a6aa-126">Request headers</span></span>
| <span data-ttu-id="8a6aa-127">Имя</span><span class="sxs-lookup"><span data-stu-id="8a6aa-127">Name</span></span>      |<span data-ttu-id="8a6aa-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8a6aa-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8a6aa-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a6aa-129">Authorization</span></span> | <span data-ttu-id="8a6aa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a6aa-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a6aa-132">Request body</span></span>
<span data-ttu-id="8a6aa-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8a6aa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a6aa-134">Response</span></span>
<span data-ttu-id="8a6aa-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-135">If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a6aa-136">Пример</span><span class="sxs-lookup"><span data-stu-id="8a6aa-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a6aa-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a6aa-137">Request</span></span>
<span data-ttu-id="8a6aa-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a6aa-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a6aa-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers
```
# <a name="c"></a>[<span data-ttu-id="8a6aa-140">C#</span><span class="sxs-lookup"><span data-stu-id="8a6aa-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a6aa-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a6aa-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a6aa-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a6aa-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8a6aa-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a6aa-143">Response</span></span>
<span data-ttu-id="8a6aa-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-144">The following is an example of the response.</span></span>
><span data-ttu-id="8a6aa-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a6aa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
