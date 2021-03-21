---
title: Get riskDetection
description: Извлечение свойств **объекта riskdetection.**
localization_priority: Normal
author: cloudhandler
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 84093741d434686a9957ca657978406fe6156da7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954230"
---
# <a name="get-riskdetection"></a><span data-ttu-id="0eef9-103">Get riskDetection</span><span class="sxs-lookup"><span data-stu-id="0eef9-103">Get riskDetection</span></span>

<span data-ttu-id="0eef9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eef9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eef9-105">Извлечение свойств **объекта riskDetection.**</span><span class="sxs-lookup"><span data-stu-id="0eef9-105">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="0eef9-106">Чтобы использовать API обнаружения рисков, необходимо иметь лицензию Azure AD Premium P1 или P2.</span><span class="sxs-lookup"><span data-stu-id="0eef9-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eef9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0eef9-107">Permissions</span></span>
<span data-ttu-id="0eef9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eef9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eef9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eef9-110">Permission type</span></span>      | <span data-ttu-id="0eef9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eef9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eef9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eef9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0eef9-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="0eef9-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="0eef9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eef9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eef9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eef9-115">Not supported.</span></span>    |
|<span data-ttu-id="0eef9-116">Application</span><span class="sxs-lookup"><span data-stu-id="0eef9-116">Application</span></span> | <span data-ttu-id="0eef9-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="0eef9-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eef9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eef9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
GET /identityProtection/riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0eef9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eef9-119">Request headers</span></span>
| <span data-ttu-id="0eef9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0eef9-120">Name</span></span>      |<span data-ttu-id="0eef9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0eef9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0eef9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0eef9-122">Authorization</span></span>  | <span data-ttu-id="0eef9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eef9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0eef9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0eef9-125">Content-Type</span></span> | <span data-ttu-id="0eef9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0eef9-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0eef9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eef9-127">Request body</span></span>
<span data-ttu-id="0eef9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0eef9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eef9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eef9-129">Response</span></span>

<span data-ttu-id="0eef9-130">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [riskDetection](../resources/riskdetection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0eef9-130">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0eef9-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0eef9-131">Examples</span></span>
### <a name="example-1-get-risk-detections"></a><span data-ttu-id="0eef9-132">Пример 1. Обнаружение рисков</span><span class="sxs-lookup"><span data-stu-id="0eef9-132">Example 1: Get risk detections</span></span>
#### <a name="request"></a><span data-ttu-id="0eef9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eef9-133">Request</span></span>
<span data-ttu-id="0eef9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eef9-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0eef9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0eef9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection_1",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="0eef9-136">C#</span><span class="sxs-lookup"><span data-stu-id="0eef9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0eef9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0eef9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0eef9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0eef9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0eef9-139">Java</span><span class="sxs-lookup"><span data-stu-id="0eef9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskdetection-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0eef9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eef9-140">Response</span></span>
<span data-ttu-id="0eef9-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0eef9-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskType": "unfamiliarFeatures",
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
    "userDisplayName": "Olivia Lack",
    "userPrincipalName": "olack@adatum.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
}
```
### <a name="example-2-get-risk-detections-for-specific-user"></a><span data-ttu-id="0eef9-142">Пример 2. Обнаружение рисков для определенного пользователя</span><span class="sxs-lookup"><span data-stu-id="0eef9-142">Example 2: Get risk detections for specific user</span></span>
#### <a name="request"></a><span data-ttu-id="0eef9-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eef9-143">Request</span></span>
<span data-ttu-id="0eef9-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eef9-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0eef9-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0eef9-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection_2",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="0eef9-146">C#</span><span class="sxs-lookup"><span data-stu-id="0eef9-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0eef9-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0eef9-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0eef9-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0eef9-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0eef9-149">Java</span><span class="sxs-lookup"><span data-stu-id="0eef9-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskdetection-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0eef9-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eef9-150">Response</span></span>
<span data-ttu-id="0eef9-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0eef9-151">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskType": "unfamiliarFeatures",
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
    "userDisplayName": "Olivia Lack",
    "userPrincipalName": "olack@adatum.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskDetection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



