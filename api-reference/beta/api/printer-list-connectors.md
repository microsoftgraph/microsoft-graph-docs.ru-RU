---
title: Список printConnectors для принтера
description: Извлечение списка соединитений, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 97640840c7054037254073f9145e801e0faf0a24
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961484"
---
# <a name="list-printconnectors-for-printer"></a><span data-ttu-id="e4866-103">Список printConnectors для принтера</span><span class="sxs-lookup"><span data-stu-id="e4866-103">List printConnectors for printer</span></span>

<span data-ttu-id="e4866-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4866-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4866-105">Извлечение списка **соединитений,** связанных с [принтером.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="e4866-105">Retrieve a list of **connectors** associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4866-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4866-106">Permissions</span></span>
<span data-ttu-id="e4866-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4866-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e4866-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e4866-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="e4866-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="e4866-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e4866-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4866-111">Permission type</span></span> | <span data-ttu-id="e4866-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4866-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e4866-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4866-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e4866-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="e4866-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="e4866-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4866-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4866-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4866-116">Not Supported.</span></span>|
|<span data-ttu-id="e4866-117">Application</span><span class="sxs-lookup"><span data-stu-id="e4866-117">Application</span></span>| <span data-ttu-id="e4866-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4866-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4866-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4866-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4866-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4866-120">Optional query parameters</span></span>
<span data-ttu-id="e4866-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e4866-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e4866-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e4866-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4866-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4866-123">Request headers</span></span>
| <span data-ttu-id="e4866-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e4866-124">Name</span></span>      |<span data-ttu-id="e4866-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e4866-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4866-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4866-126">Authorization</span></span> | <span data-ttu-id="e4866-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4866-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4866-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4866-129">Request body</span></span>
<span data-ttu-id="e4866-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4866-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e4866-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4866-131">Response</span></span>
<span data-ttu-id="e4866-132">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов printConnector](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4866-132">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4866-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e4866-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4866-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4866-134">Request</span></span>
<span data-ttu-id="e4866-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4866-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4866-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4866-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/connectors
```
# <a name="c"></a>[<span data-ttu-id="e4866-137">C#</span><span class="sxs-lookup"><span data-stu-id="e4866-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4866-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4866-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4866-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4866-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4866-140">Java</span><span class="sxs-lookup"><span data-stu-id="e4866-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e4866-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4866-141">Response</span></span>
<span data-ttu-id="e4866-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e4866-142">The following is an example of the response.</span></span>
><span data-ttu-id="e4866-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4866-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1373

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printConnector)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "Connector1",
      "fullyQualifiedDomainName": "connector1@redmond.corp.microsoft.com",
      "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
      "appVersion": "0.19.7338.23496",
      "deviceHealth": {
        "lastConnectionTime": "2020-02-04T07:00:00.0000000"
      },
      "registeredDateTime": "2020-02-04T07:00:00.0000000",
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
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
