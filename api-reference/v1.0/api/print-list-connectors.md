---
title: PrintConnectors списка
description: Извлечение списка соединитений.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9ef3bb3f197f8c7f0122993c6ca8cb716ddce92b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948897"
---
# <a name="list-printconnectors"></a><span data-ttu-id="efbbf-103">PrintConnectors списка</span><span class="sxs-lookup"><span data-stu-id="efbbf-103">List printConnectors</span></span>
<span data-ttu-id="efbbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efbbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="efbbf-105">Извлечение списка соединитений печати.</span><span class="sxs-lookup"><span data-stu-id="efbbf-105">Retrieve a list of print connectors.</span></span>

## <a name="permissions"></a><span data-ttu-id="efbbf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efbbf-106">Permissions</span></span>
<span data-ttu-id="efbbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efbbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="efbbf-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="efbbf-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="efbbf-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="efbbf-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="efbbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efbbf-111">Permission type</span></span> | <span data-ttu-id="efbbf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efbbf-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="efbbf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efbbf-113">Delegated (work or school account)</span></span>| <span data-ttu-id="efbbf-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efbbf-114">PrintConnector.Read.All, PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="efbbf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efbbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efbbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efbbf-116">Not Supported.</span></span>|
|<span data-ttu-id="efbbf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efbbf-117">Application</span></span>| <span data-ttu-id="efbbf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efbbf-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="efbbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efbbf-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/connectors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efbbf-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="efbbf-120">Optional query parameters</span></span>
<span data-ttu-id="efbbf-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="efbbf-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="efbbf-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="efbbf-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="efbbf-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="efbbf-123">Exceptions</span></span>
<span data-ttu-id="efbbf-124">Некоторые операторы не поддерживаются: `$count` , `$search` `$filter` .</span><span class="sxs-lookup"><span data-stu-id="efbbf-124">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efbbf-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efbbf-125">Request headers</span></span>
| <span data-ttu-id="efbbf-126">Имя</span><span class="sxs-lookup"><span data-stu-id="efbbf-126">Name</span></span>      |<span data-ttu-id="efbbf-127">Описание</span><span class="sxs-lookup"><span data-stu-id="efbbf-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="efbbf-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efbbf-128">Authorization</span></span> | <span data-ttu-id="efbbf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efbbf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efbbf-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efbbf-131">Request body</span></span>
<span data-ttu-id="efbbf-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efbbf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efbbf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="efbbf-133">Response</span></span>

<span data-ttu-id="efbbf-134">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printConnector](../resources/printconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="efbbf-134">If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efbbf-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="efbbf-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efbbf-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="efbbf-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="efbbf-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="efbbf-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printconnector_1"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/connectors
```
# <a name="c"></a>[<span data-ttu-id="efbbf-138">C#</span><span class="sxs-lookup"><span data-stu-id="efbbf-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printconnector-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efbbf-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efbbf-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printconnector-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efbbf-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efbbf-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printconnector-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efbbf-141">Java</span><span class="sxs-lookup"><span data-stu-id="efbbf-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printconnector-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="efbbf-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="efbbf-142">Response</span></span>
<span data-ttu-id="efbbf-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="efbbf-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/connectors",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "Connector1",
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

