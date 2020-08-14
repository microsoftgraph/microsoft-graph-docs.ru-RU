---
title: Получение Принтконнектор
description: Получение свойств и связей объекта Connector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a5623027b625dfacdc21af5f5806a12f320b2ff1
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674031"
---
# <a name="get-printconnector"></a><span data-ttu-id="98a55-103">Получение Принтконнектор</span><span class="sxs-lookup"><span data-stu-id="98a55-103">Get printConnector</span></span>

<span data-ttu-id="98a55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98a55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98a55-105">Получение свойств и связей объекта **принтконнектор** .</span><span class="sxs-lookup"><span data-stu-id="98a55-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="98a55-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98a55-106">Permissions</span></span>
<span data-ttu-id="98a55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98a55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="98a55-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="98a55-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="98a55-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="98a55-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="98a55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98a55-111">Permission type</span></span> | <span data-ttu-id="98a55-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98a55-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="98a55-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98a55-113">Delegated (work or school account)</span></span>| <span data-ttu-id="98a55-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="98a55-114">User.Read</span></span> |
|<span data-ttu-id="98a55-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98a55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98a55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98a55-116">Not Supported.</span></span>|
|<span data-ttu-id="98a55-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98a55-117">Application</span></span>|<span data-ttu-id="98a55-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98a55-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98a55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98a55-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98a55-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98a55-120">Optional query parameters</span></span>
<span data-ttu-id="98a55-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="98a55-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="98a55-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="98a55-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="98a55-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98a55-123">Request headers</span></span>
| <span data-ttu-id="98a55-124">Имя</span><span class="sxs-lookup"><span data-stu-id="98a55-124">Name</span></span>      |<span data-ttu-id="98a55-125">Описание</span><span class="sxs-lookup"><span data-stu-id="98a55-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98a55-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98a55-126">Authorization</span></span> | <span data-ttu-id="98a55-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98a55-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98a55-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98a55-129">Request body</span></span>
<span data-ttu-id="98a55-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98a55-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="98a55-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="98a55-131">Response</span></span>
<span data-ttu-id="98a55-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтконнектор](../resources/printconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98a55-132">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98a55-133">Пример</span><span class="sxs-lookup"><span data-stu-id="98a55-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98a55-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="98a55-134">Request</span></span>
<span data-ttu-id="98a55-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98a55-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98a55-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="98a55-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="98a55-137">C#</span><span class="sxs-lookup"><span data-stu-id="98a55-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98a55-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98a55-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98a55-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98a55-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="98a55-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="98a55-140">Response</span></span>
<span data-ttu-id="98a55-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98a55-141">The following is an example of the response.</span></span>
><span data-ttu-id="98a55-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98a55-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1097

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "name": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
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
  "description": "Get printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
