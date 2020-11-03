---
title: Список Принтконнекторс
description: Получение списка соединителей.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ea33c5eb43bb008d39ec40f3b79f9be501cc4629
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849076"
---
# <a name="list-printconnectors"></a><span data-ttu-id="66999-103">Список Принтконнекторс</span><span class="sxs-lookup"><span data-stu-id="66999-103">List printConnectors</span></span>

<span data-ttu-id="66999-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66999-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66999-105">Получение списка соединителей печати.</span><span class="sxs-lookup"><span data-stu-id="66999-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="66999-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66999-106">Permissions</span></span>
<span data-ttu-id="66999-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="66999-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="66999-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="66999-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="66999-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="66999-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66999-111">Permission type</span></span> | <span data-ttu-id="66999-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66999-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="66999-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66999-113">Delegated (work or school account)</span></span>| <span data-ttu-id="66999-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="66999-114">User.Read</span></span> |
|<span data-ttu-id="66999-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66999-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66999-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66999-116">Not Supported.</span></span>|
|<span data-ttu-id="66999-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66999-117">Application</span></span>| <span data-ttu-id="66999-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66999-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66999-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66999-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66999-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66999-120">Optional query parameters</span></span>
<span data-ttu-id="66999-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="66999-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="66999-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="66999-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="66999-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="66999-123">Exceptions</span></span>
<span data-ttu-id="66999-124">Некоторые операторы не поддерживаются: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="66999-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66999-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66999-125">Request headers</span></span>
| <span data-ttu-id="66999-126">Имя</span><span class="sxs-lookup"><span data-stu-id="66999-126">Name</span></span>      |<span data-ttu-id="66999-127">Описание</span><span class="sxs-lookup"><span data-stu-id="66999-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66999-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66999-128">Authorization</span></span> | <span data-ttu-id="66999-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66999-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66999-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66999-131">Request body</span></span>
<span data-ttu-id="66999-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66999-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="66999-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="66999-133">Response</span></span>
<span data-ttu-id="66999-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтконнектор](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66999-134">If successful, this method returns a `200 OK` response code and collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66999-135">Пример</span><span class="sxs-lookup"><span data-stu-id="66999-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="66999-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="66999-136">Request</span></span>
<span data-ttu-id="66999-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66999-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66999-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="66999-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="66999-139">C#</span><span class="sxs-lookup"><span data-stu-id="66999-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66999-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66999-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66999-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66999-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="66999-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="66999-142">Response</span></span>
<span data-ttu-id="66999-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66999-143">The following is an example of the response.</span></span>
><span data-ttu-id="66999-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66999-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
