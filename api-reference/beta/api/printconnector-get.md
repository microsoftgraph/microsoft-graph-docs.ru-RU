---
title: Get printConnector
description: Извлечение свойств и связей объекта соединители.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 898a7d5879f258fe80207a174f97d1622caa9e17
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942347"
---
# <a name="get-printconnector"></a><span data-ttu-id="55246-103">Get printConnector</span><span class="sxs-lookup"><span data-stu-id="55246-103">Get printConnector</span></span>

<span data-ttu-id="55246-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55246-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55246-105">Извлечение свойств и связей объекта **printConnector.**</span><span class="sxs-lookup"><span data-stu-id="55246-105">Retrieve the properties and relationships of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55246-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55246-106">Permissions</span></span>
<span data-ttu-id="55246-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55246-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="55246-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="55246-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="55246-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="55246-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="55246-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55246-111">Permission type</span></span> | <span data-ttu-id="55246-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55246-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="55246-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55246-113">Delegated (work or school account)</span></span>| <span data-ttu-id="55246-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55246-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="55246-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55246-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55246-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55246-116">Not Supported.</span></span>|
|<span data-ttu-id="55246-117">Application</span><span class="sxs-lookup"><span data-stu-id="55246-117">Application</span></span>|<span data-ttu-id="55246-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55246-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55246-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55246-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55246-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55246-120">Optional query parameters</span></span>
<span data-ttu-id="55246-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="55246-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="55246-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="55246-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="55246-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55246-123">Request headers</span></span>
| <span data-ttu-id="55246-124">Имя</span><span class="sxs-lookup"><span data-stu-id="55246-124">Name</span></span>      |<span data-ttu-id="55246-125">Описание</span><span class="sxs-lookup"><span data-stu-id="55246-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55246-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55246-126">Authorization</span></span> | <span data-ttu-id="55246-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55246-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55246-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55246-129">Request body</span></span>
<span data-ttu-id="55246-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55246-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="55246-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="55246-131">Response</span></span>
<span data-ttu-id="55246-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект printConnector](../resources/printconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="55246-132">If successful, this method returns a `200 OK` response code and [printConnector](../resources/printconnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55246-133">Пример</span><span class="sxs-lookup"><span data-stu-id="55246-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55246-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="55246-134">Request</span></span>
<span data-ttu-id="55246-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55246-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55246-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="55246-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="55246-137">C#</span><span class="sxs-lookup"><span data-stu-id="55246-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55246-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55246-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55246-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55246-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55246-140">Java</span><span class="sxs-lookup"><span data-stu-id="55246-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connector-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55246-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="55246-141">Response</span></span>
<span data-ttu-id="55246-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55246-142">The following is an example of the response.</span></span>
><span data-ttu-id="55246-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55246-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "displayName": "ConnectorName",
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
