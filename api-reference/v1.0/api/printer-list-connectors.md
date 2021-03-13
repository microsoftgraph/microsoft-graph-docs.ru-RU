---
title: Список printConnectors для принтера
description: Извлечение списка соединитений, связанных с принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 5176819d4d91e696a08c288e086fb237622c777b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771990"
---
# <a name="list-printconnectors-for-a-printer"></a><span data-ttu-id="29258-103">Список printConnectors для принтера</span><span class="sxs-lookup"><span data-stu-id="29258-103">List printConnectors for a printer</span></span>
<span data-ttu-id="29258-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29258-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="29258-105">Извлечение списка [printConnectors,](../resources/printconnector.md) связанных с [принтером.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="29258-105">Retrieve a list of [printConnectors](../resources/printconnector.md) associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29258-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29258-106">Permissions</span></span>
<span data-ttu-id="29258-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="29258-109">Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="29258-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="29258-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29258-110">Permission type</span></span> | <span data-ttu-id="29258-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29258-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="29258-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29258-112">Delegated (work or school account)</span></span>| <span data-ttu-id="29258-113">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29258-113">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="29258-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29258-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29258-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29258-115">Not Supported.</span></span>|
|<span data-ttu-id="29258-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29258-116">Application</span></span>| <span data-ttu-id="29258-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29258-117">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29258-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29258-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29258-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29258-119">Optional query parameters</span></span>
<span data-ttu-id="29258-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="29258-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="29258-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="29258-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="29258-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29258-122">Request headers</span></span>
|<span data-ttu-id="29258-123">Имя</span><span class="sxs-lookup"><span data-stu-id="29258-123">Name</span></span>|<span data-ttu-id="29258-124">Описание</span><span class="sxs-lookup"><span data-stu-id="29258-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="29258-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29258-125">Authorization</span></span>|<span data-ttu-id="29258-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29258-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29258-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29258-128">Request body</span></span>
<span data-ttu-id="29258-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29258-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29258-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="29258-130">Response</span></span>

<span data-ttu-id="29258-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printConnector](../resources/printconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="29258-131">If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29258-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="29258-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29258-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="29258-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="29258-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="29258-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/connectors
```
# <a name="c"></a>[<span data-ttu-id="29258-135">C#</span><span class="sxs-lookup"><span data-stu-id="29258-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29258-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29258-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29258-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29258-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29258-138">Java</span><span class="sxs-lookup"><span data-stu-id="29258-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="29258-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="29258-139">Response</span></span>
<span data-ttu-id="29258-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="29258-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printConnector)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('2f3453b7-4686-4b5b-9575-4f1e5b909ba7')/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "Connector1",
      "fullyQualifiedDomainName": "connector1@redmond.corp.microsoft.com",
      "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
      "appVersion": "0.19.7338.23496",
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

