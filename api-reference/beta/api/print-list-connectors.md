---
title: PrintConnectors списка
description: Извлечение списка соединитений.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 36cf3775da6a2fbc5e721c6f8dc80be714e14851
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766520"
---
# <a name="list-printconnectors"></a><span data-ttu-id="3835b-103">PrintConnectors списка</span><span class="sxs-lookup"><span data-stu-id="3835b-103">List printConnectors</span></span>

<span data-ttu-id="3835b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3835b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3835b-105">Извлечение списка соединитений печати.</span><span class="sxs-lookup"><span data-stu-id="3835b-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="3835b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3835b-106">Permissions</span></span>
<span data-ttu-id="3835b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3835b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3835b-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="3835b-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="3835b-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="3835b-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="3835b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3835b-111">Permission type</span></span> | <span data-ttu-id="3835b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3835b-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3835b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3835b-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3835b-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3835b-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="3835b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3835b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3835b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3835b-116">Not Supported.</span></span>|
|<span data-ttu-id="3835b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3835b-117">Application</span></span>| <span data-ttu-id="3835b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3835b-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3835b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3835b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3835b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3835b-120">Optional query parameters</span></span>
<span data-ttu-id="3835b-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3835b-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3835b-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3835b-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="3835b-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="3835b-123">Exceptions</span></span>
<span data-ttu-id="3835b-124">Некоторые операторы не поддерживаются: `$count` , `$search` `$filter` .</span><span class="sxs-lookup"><span data-stu-id="3835b-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3835b-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3835b-125">Request headers</span></span>
| <span data-ttu-id="3835b-126">Имя</span><span class="sxs-lookup"><span data-stu-id="3835b-126">Name</span></span>      |<span data-ttu-id="3835b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3835b-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3835b-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3835b-128">Authorization</span></span> | <span data-ttu-id="3835b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3835b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3835b-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3835b-131">Request body</span></span>
<span data-ttu-id="3835b-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3835b-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3835b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3835b-133">Response</span></span>
<span data-ttu-id="3835b-134">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов printConnector](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3835b-134">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3835b-135">Пример</span><span class="sxs-lookup"><span data-stu-id="3835b-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="3835b-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3835b-136">Request</span></span>
<span data-ttu-id="3835b-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3835b-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3835b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3835b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="3835b-139">C#</span><span class="sxs-lookup"><span data-stu-id="3835b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3835b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3835b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3835b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3835b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3835b-142">Java</span><span class="sxs-lookup"><span data-stu-id="3835b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3835b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3835b-143">Response</span></span>
<span data-ttu-id="3835b-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3835b-144">The following is an example of the response.</span></span>
><span data-ttu-id="3835b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3835b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "Connector1",
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
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
