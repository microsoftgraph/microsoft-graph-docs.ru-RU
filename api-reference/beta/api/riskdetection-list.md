---
title: Список Рискдетектион
description: Получение свойств коллекции объекта **рискдетектион** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da19ac0afc940b1a204940157cac3b8f78bcd17b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977702"
---
# <a name="list-riskdetection"></a><span data-ttu-id="3b880-103">Список Рискдетектион</span><span class="sxs-lookup"><span data-stu-id="3b880-103">List riskDetection</span></span>

<span data-ttu-id="3b880-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b880-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b880-105">Получение свойств коллекции объектов **рискдетектион** .</span><span class="sxs-lookup"><span data-stu-id="3b880-105">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="3b880-106">Для использования API обнаружения риска необходима лицензия Azure AD Premium P1 или P2.</span><span class="sxs-lookup"><span data-stu-id="3b880-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b880-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b880-107">Permissions</span></span>

<span data-ttu-id="3b880-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b880-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b880-110">Permission type</span></span>      | <span data-ttu-id="3b880-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b880-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b880-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b880-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b880-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b880-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="3b880-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b880-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b880-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b880-115">Not supported.</span></span>    |
|<span data-ttu-id="3b880-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3b880-116">Application</span></span> | <span data-ttu-id="3b880-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b880-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b880-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b880-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
GET /identityProtection/riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b880-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b880-119">Optional query parameters</span></span>

<span data-ttu-id="3b880-120">Этот метод поддерживает `$filter` и `$select` настраивает ответ на запрос.</span><span class="sxs-lookup"><span data-stu-id="3b880-120">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="3b880-121">Просмотрите пример, приведенный далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="3b880-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="3b880-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b880-122">Request headers</span></span>

| <span data-ttu-id="3b880-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3b880-123">Name</span></span>      |<span data-ttu-id="3b880-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3b880-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b880-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b880-125">Authorization</span></span>  | <span data-ttu-id="3b880-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b880-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b880-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b880-128">Content-Type</span></span> | <span data-ttu-id="3b880-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3b880-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b880-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b880-130">Request body</span></span>

<span data-ttu-id="3b880-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b880-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b880-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b880-132">Response</span></span>

<span data-ttu-id="3b880-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискдетектион](../resources/riskdetection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b880-133">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b880-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="3b880-134">Examples</span></span>


### <a name="example-1-list-risk-detections"></a><span data-ttu-id="3b880-135">Пример 1: список обнаруженных рисков</span><span class="sxs-lookup"><span data-stu-id="3b880-135">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="3b880-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b880-136">Request</span></span>

<span data-ttu-id="3b880-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b880-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b880-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b880-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="3b880-139">C#</span><span class="sxs-lookup"><span data-stu-id="3b880-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b880-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b880-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b880-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b880-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b880-142">Java</span><span class="sxs-lookup"><span data-stu-id="3b880-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b880-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b880-143">Response</span></span>

<span data-ttu-id="3b880-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b880-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskEventType": "unfamiliarFeatures",
    "riskState": "remediated",
    "riskLevel": "medium",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "source": "activeDirectory",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

### <a name="example-2-list-risk-detections-for-a-specific-user"></a><span data-ttu-id="3b880-145">Пример 2: список обнаруженных рисков для определенного пользователя</span><span class="sxs-lookup"><span data-stu-id="3b880-145">Example 2: List risk detections for a specific user</span></span>

#### <a name="request"></a><span data-ttu-id="3b880-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b880-146">Request</span></span>

<span data-ttu-id="3b880-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b880-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b880-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b880-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="3b880-149">C#</span><span class="sxs-lookup"><span data-stu-id="3b880-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b880-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b880-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b880-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b880-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b880-152">Java</span><span class="sxs-lookup"><span data-stu-id="3b880-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b880-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b880-153">Response</span></span>

<span data-ttu-id="3b880-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b880-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskEventType": "unfamiliarFeatures",
    "riskState": "remediated",
    "riskLevel": "medium",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "source": "activeDirectory",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

### <a name="example-3-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="3b880-155">Пример 3: список обнаруженных рисков и фильтрация результатов</span><span class="sxs-lookup"><span data-stu-id="3b880-155">Example 3: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="3b880-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b880-156">Request</span></span>

<span data-ttu-id="3b880-157">В приведенном ниже примере показано, как `$filter` получить коллекцию обнаружений рисков, в которой уровень риска является средним, или тип события риска — унфамиларфеатурес, что означает, что вход в систему был незнакомым или неизвестным расположением.</span><span class="sxs-lookup"><span data-stu-id="3b880-157">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b880-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b880-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections?$filter=riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```
# <a name="c"></a>[<span data-ttu-id="3b880-159">C#</span><span class="sxs-lookup"><span data-stu-id="3b880-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskdetections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b880-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b880-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskdetections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b880-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b880-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskdetections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b880-162">Java</span><span class="sxs-lookup"><span data-stu-id="3b880-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskdetections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b880-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b880-163">Response</span></span>

<span data-ttu-id="3b880-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b880-164">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
    "id": "1d68fc3d60d012ff80ad4b16818bf304df1bde295fdf1db31fa5389ba9532cd1",
    "requestId": "3295073e-04b1-4871-9d15-c1f871b41100",
    "correlationId": "f141d8e5-93e9-4fd0-9eb0-c40e5f8fc092",
    "riskEventType": "unfamiliarFeatures",
    "riskState": "atRisk",
    "riskLevel": "medium",
    "riskDetail": "none",
    "source": "Identity Protection",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskDetections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


